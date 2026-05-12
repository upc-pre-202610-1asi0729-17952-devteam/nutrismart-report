# CAPÍTULO IV: PRODUCT DESIGN

## 4.1. Style Guidelines

### 4.1.1. General Style Guidelines

### 4.1.2. Web Style Guidelines

## 4.2. Information Architecture

### 4.2.1. Organization Systems

### 4.2.2. Labeling Systems

### 4.2.3. SEO Tags and Meta Tags

### 4.2.4. Searching Systems

### 4.2.5. Navigation Systems

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe

### 4.3.2. Landing Page Mock-up

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes

### 4.4.2. Web Applications Wireflow Diagrams

### 4.4.2. Web Applications Mock-ups

### 4.4.3. Web Applications User Flow Diagrams

## 4.5. Web Applications Prototyping

## 4.6. Domain-Driven Software Architecture

La arquitectura de NutriSmart se basa en Domain-Driven Design (DDD), centrando el diseño en los procesos críticos de salud y nutrición. El sistema se organiza en 7 Bounded Contexts independientes, lo que garantiza una separación clara de responsabilidades y un lenguaje común entre el equipo técnico y el negocio. Este enfoque modular permite que funcionalidades clave, como el análisis de imágenes y el motor de recomendaciones, sean altamente escalables, facilitando un mantenimiento eficiente y una evolución alineada con los requerimientos del dominio.

A continuación, se identifican y describen los contextos delimitados que componen la solución:
| Bounded Context | Descripción | Módulos incluidos |
| :--- | :--- | :--- |
| **Identity & Access** | Gestión de autenticación, autorización y perfiles de usuario. | User & Auth, Onboarding |
| **Subscriptions & Billing** | Gestión de planes, facturación y control de features Premium. | Subscriptions, Stripe Integration |
| **Metabolic Adaptation** | Cálculo de métricas corporales (BMI, BMR, TDEE), metas calóricas y sincronización con wearables. | Body Tracking, Wearable Sync, Activity Log |
| **Nutrition Tracking** | Registro y análisis de alimentos mediante logs y Smart Scan. | Nutrition Log, Smart Scan, Dietary Restrictions |
| **Behavioral Consistency** | Seguimiento de adherencia, detección de caídas conductuales y gestión de rachas. | Adherence Tracking, Streak Engine |
| **Restaurant Intelligence** | Análisis de menús físicos mediante foto y ranking de platos compatibles con el perfil del usuario. | Menu Scan, Dish Ranking |
| **Smart Recommendations** | Motor de sugerencias personalizadas según contexto, clima, despensa y estado conductual. | Recommendations Engine, Travel Mode, Pantry |
| **Analytics & Reporting** | Generación de dashboards, progreso visual y reportes en PDF. | Dashboard & Analytics |

### 4.6.1. Design-Level EventStorming

En esta sección se presenta el modelado del comportamiento del sistema mediante la técnica de EventStorming a nivel de diseño. Este proceso permitió identificar los eventos de dominio, los comandos que disparan la lógica de negocio y las políticas automáticas que rigen la reactividad del sistema en cada Bounded Context.

---
 
## Nivel Core
 
---
 
### Metabolic Adaptation
 
Este contexto calcula y mantiene actualizados los targets metabólicos del usuario. Consta de 5 swimlanes.
 
#### Initial Metabolic Calculation
 
Disparado por `OnboardingCompleted` (desde IAM), el sistema ejecuta `CalculateInitialTargets`. El cálculo sigue la secuencia: **BMI → BMR (Mifflin-St Jeor) → TDEE**. Según el objetivo:
 
- `lose_weight` → `SetCaloricDeficitTarget`: `TDEE - 500 kcal`, macros P30%/C40%/F30%
- `gain_muscle` → `SetCaloricSurplusTarget`: `TDEE + 300 kcal`, macros P35%/C45%/F20%
El evento `MetabolicTargetSet` notifica a **Nutrition Tracking** para inicializar los objetivos diarios.
 
#### Body Metrics Update
 
El usuario ejecuta `UpdateBodyMetrics` (nuevo peso/talla). Las políticas de validación de entrada preceden la emisión de `BodyMetricsUpdated`, que recalcula BMI, BMR y TDEE. El evento `MetabolicTargetsRecalculated` propaga actualizaciones hacia **Nutrition Tracking** y **Behavioral Consistency**.
 
#### Stagnation Detection
 
El sistema evalúa diariamente el progreso. Si transcurren **14 días consecutivos sin avance**, ejecuta `DetectWeightPlateau`, emitiendo `StagnationDetected`, que activa en **Smart Recommendation** el comando `SuggestStrategyAdjustment`.
 
#### Wearable Sync *(requiere Premium)*
 
Habilitado por `BenefitsEnabled` (Premium), el usuario conecta Google Fit con `ConnectGoogleFit`. Una vez activo, el sistema sincroniza cada hora mediante `SyncWearableActivity`, emitiendo `ActivitySynced`. La política subsecuente ejecuta `AdjustDailyCalorieTarget`, que emite `CaloricTargetAdjusted` y actualiza el objetivo neto en **Nutrition Tracking**.
 
#### Manual Activity Log
 
El usuario registra actividad manualmente con `LogManualActivity`. La política calcula las calorías activas con la fórmula `MET × peso_kg × horas`, emitiendo `ActiveCaloriesCalculated`, y ajusta el balance calórico diario del mismo modo que el wearable.
 
---

### Nutrition Tracking
 
Este contexto centraliza el registro de alimentos y la validación diaria de macros. Consta de 8 swimlanes.
 
#### Dietary Restrictions Registration
 
Disparado por `OnboardingCompleted`, el sistema ejecuta `RegisterDietaryRestrictions`, activando la lista de restricciones que filtrará todo registro posterior.
 
#### Food Search
 
El usuario busca alimentos con `SearchFoodItem`, consultando las APIs **Open Food Facts** y **USDA FoodData Central**. El evento `FoodSearchExecuted` presenta la vista **Food Results List** con valores nutricionales por ítem.
 
#### Meal Logging
 
El usuario registra una comida con `LogMealEntry`. La política **CheckDietaryRestrictions** bloquea el registro si el alimento contiene algún ingrediente restringido, emitiendo `RestrictedItemBlocked` con notificación push. Si pasa la validación, se emite `MealRecorded`, actualizando el **Daily Macro Summary** y notificando a **Behavioral Consistency**.
 
#### Daily Macro Validation
 
Cada vez que se emite `MealRecorded`, la política **ValidateDailyMacros** compara el consumo total contra el objetivo:
 
- Consumo ≤ objetivo → `DailyProgressUpdated` (estado: `on_track`)
- Consumo > objetivo → `DailyGoalExceeded` con notificación push y desvío reportado a **Behavioral Consistency**
#### End of Day Evaluation
 
A las 23:59, el sistema evalúa si el usuario completó el día dentro del ±10% de su objetivo calórico. Si se cumple, emite `DailyGoalMet`, propagándose hacia **Behavioral Consistency** y **Analytics**. Si una ventana horaria de comida (desayuno 06-10h / almuerzo 11-15h / cena 18-22h) pasa sin registro, se emite `MealSkipped` con notificación push y se notifica a **Behavioral Consistency**.
 
#### Edit and Delete Meal Entry
 
El usuario puede corregir un registro con `EditMealEntry` (emite `MealEntryUpdated`) o eliminarlo con `DeleteMealEntry` (emite `MealEntryRemoved`). Ambos eventos relanzan automáticamente la política **ValidateDailyMacros**.
 
#### Smart Scan — Food Plate Photo *(Pro / Premium)*
 
El usuario escanea un plato con `ScanMealPhoto`. La imagen se procesa mediante **Google Cloud Vision API** y **Open Food Facts API**. La política **Image Valid** rechaza imágenes que no sean de comida. El evento `MealPhotoAnalyzed` presenta la vista **Scan Preview Card** con ítems y macros estimados. El usuario confirma con `ConfirmScanResult`, emitiendo `MealRecorded` (fuente: `smart_scan`), que sigue el mismo flujo que el log manual.
 
#### Incoming Events *(receptores)*
 
Este swimlane recibe eventos de otros contextos:
 
| Evento entrante | Origen | Comando disparado |
| :--- | :--- | :--- |
| `MetabolicTargetSet` | Metabolic Adaptation | `SetDailyNutritionalTargets` |
| `CaloricTargetAdjusted` | Metabolic Adaptation | `UpdateNetDailyTarget` |
| `CompatibleDishesRanked` | Restaurant Intelligence | [Read Model] Menu Analysis Result |
 
---

### Behavioral Consistency
 
Este contexto evalúa la adherencia conductual del usuario y escala respuestas ante desviaciones. Consta de 7 swimlanes.
 
#### Behavioral Tracking Initialization
 
Disparado por `OnboardingCompleted`, el sistema ejecuta `InitializeBehavioralTracking`, estableciendo el estado inicial: `adherence_status: ON_TRACK`, `streak: 0`, `consecutive_misses: 0`.
 
#### Daily Adherence Evaluation
 
Ante cada `MealRecorded` o `DailyGoalMet` desde Nutrition Tracking, el sistema evalúa el estado de adherencia. Si todo está en orden, emite `AdherenceUpdated` (`status: ON_TRACK`, `streak +1`).
 
#### Behavioral Drop Detection
 
Si `MealSkipped` o `DailyGoalExceeded` ocurren durante **3 días consecutivos**, la política dispara `DetectBehavioralDrop`, emitiendo `BehavioralDropDetected` (`status: AT_RISK`). Se envía una notificación push motivacional y se activa en **Smart Recommendation** el comando `GeneratePreventiveRecommendation`.
 
#### Abandonment Risk Escalation
 
Si tras `BehavioralDropDetected` no hay recuperación en los siguientes **4 días** (total: 7 días sin adherencia), el sistema ejecuta `EscalateAbandonmentRisk`, emitiendo `NutritionalAbandonmentRisk` (`status: DROPPED`). Se envía una notificación push empática y se activa `RequestInterventionRecommendation` en **Smart Recommendation**.
 
#### Consistency Recovery
 
Cuando el usuario vuelve a registrar una comida luego de estar en estado `AT_RISK` o `DROPPED`, la política detecta la recuperación y ejecuta `RegisterConsistencyRecovery`, emitiendo `ConsistencyRecovered`. Se envía notificación positiva y se notifica a **Analytics** para actualizar el historial de adherencia.
 
#### Streak Milestone
 
Cuando `DailyGoalMet` se acumula **7 días consecutivos**, el sistema ejecuta `RegisterStreakMilestone`, emitiendo `StreakMilestoneReached` (hitos: 7 / 14 / 21 / 30 días). El usuario recibe una notificación de celebración y se actualiza la vista **Streak Badge**.
 
#### Strategy Consistency Evaluation
 
Disparado por `MetabolicTargetsRecalculated` (desde Metabolic Adaptation), el sistema evalúa si el nuevo objetivo es compatible con el historial de adherencia del usuario:
 
- Compatible → `StrategyConsistencyConfirmed`
- Muy agresivo → `StrategyMismatchDetected` → **Smart Recommendation**: `SuggestGradualAdjustment`

---


**EventStorming**

![EventStorming Diagram](../assets/img/artifacts/eventStorming.jpg)

Para poder apreciar mejor el EventStorming le recomendamos ingresar al siguiente link:
<br>[Visualizar EventStorming en Miro](https://miro.com/app/live-embed/uXjVHXMvsmU=/?embedMode=view_only_without_ui&moveToViewport=-66936%2C-26975%2C145750%2C52483&embedId=331104344485)

### 4.6.2. Software Architecture Context Diagram

El Diagrama de Contexto (Nivel 1 del modelo C4) representa a NutriSmart como un sistema centralizado y detalla su interacción con los actores principales y sistemas externos. Este diagrama permite visualizar el alcance global de la solución y los límites del sistema con servicios de terceros que alimentan la lógica de nutrición y salud.

**Elementos:**

 - **NutriSmart:** Sistema central que provee las funcionalidades de seguimiento nutricional, escaneo de comidas y recomendaciones inteligentes.
 - **User:** Persona que utiliza la plataforma para gestionar sus objetivos de salud, registrar sus comidas y monitorear su actividad física.
 - **External Systems:**
	- `Google Cloud Vision API:` Procesa las imágenes para el análisis de alimentos.
	- `Nutrition Data Providers:` Fuentes de consulta para información calórica y macronutrientes.
	- `Google Fit API:` Sincroniza datos de actividad física y gasto energético.
	- `OpenWeatherMap:` Provee datos climáticos para ajustar las sugerencias de comidas.
	- `Stripe:` Gestiona de forma segura los pagos y el estado de las suscripciones.
	- `Geolocation API:` Provee la ubicación actual del usuario para el Modo Viaje y las recomendaciones contextuales(plan Pro/Premium).

![Context Diagram](../assets/img/artifacts/1nutrismart-SystemContext.png)

### 4.6.3. Software Architecture Container Diagrams

El Diagrama de Contenedores (Nivel 2 del modelo C4) desglosa el sistema NutriSmart en sus principales unidades lógicas de ejecución. En este nivel, se especifican las responsabilidades de cada contenedor, las tecnologías elegidas para su implementación y los protocolos de comunicación que permiten la interacción entre ellos y con los sistemas externos.

**Elementos:**

 - **Web Application:** Servidor web que entrega los archivos estáticos al navegador del usuario para inicializar la aplicación.
    - **Tecnología:** `Nginx`.
 - **Landing Page:** Sitio web estático que presenta la propuesta de valor de NutriSmart y redirige a los usuarios hacia la aplicación web.
    - **Tecnología:** `HTML5 + CSS3 + JavaScript`.
 - **Single Page Application:** Frontend donde los usuarios interactúan con la plataforma, gestionan sus metas y visualizan sus progresos. Se ejecuta completamente en el navegador del usuario.
    - **Tecnología:** `Angular (con Angular Material para UI y RxJS para la gestión de servicios)`.
 - **API Application:** Backend que maneja la lógica de negocio, el motor de recomendaciones, el procesamiento de imágenes y la integración con servicios externos.
    - **Tecnología:** `Spring Boot (Java)`.
 - **Database:** Almacena la información de usuarios, registros nutricionales, historial de métricas y datos de facturación.
    - **Tecnología:** `PostgreSQL`.
 - **External Systems:** APIs de terceros que se integran con el backend para extender las capacidades del sistema.
    - **Tecnología:** `JSON/HTTPS (REST)`.

![Container Diagram](../assets/img/artifacts/2nutrismart-ContainerDiagram.png)

![Container Diagram Summarized](../assets/img/artifacts/3nutrismart-ContainerDiagram1.png)

### 4.6.4. Software Architecture Components Diagrams

El Diagrama de Componentes (Nivel 3 del modelo C4) describe la estructura interna de los contenedores principales de NutriSmart. En esta sección se detallan los módulos lógicos, sus responsabilidades específicas y las tecnologías utilizadas para la implementación de cada componente.

**A. Single Page Application Components (Frontend)**

El Single Page Application se organiza en 7 Bounded Contexts, cada uno con 4 capas siguiendo el patrón de arquitectura del Domain-Driven Design.

El diagrama a continuación muestra todos los componentes de la arquitectura en un único bloque, dado que Structurizr no soporta la agrupación visual por Bounded Context en las vistas de componentes.

![Web Component Diagram](../assets/img/artifacts/4nutrismart-WebComponentsDiagram.png)

Cada Bounded Context contiene una capa de Presentation con las vistas Angular, una capa de Application con los servicios TypeScript que orquestan la lógica del cliente, una capa de Domain con los modelos e interfaces, y una capa de Infrastructure con el cliente HTTP Angular que se comunica con el API Application.

Para apreciar la separación por capas Domain-Driven Design de cada Bounded Context, se presenta a continuación un diagrama de detalle individual por cada uno.

**Bounded Contexts:**

 - **Identity & Access:** Gestiona las vistas de login, registro y perfil del usuario.

   ![IAM Frontend Diagram](../assets/img/artifacts/5nutrismart-IAMFrontendDiagram.png)

 - **Nutrition Tracking:** Gestiona las vistas de registro de comidas, Smart Scan y  búsqueda de alimentos.

   ![Nutrition Frontend Diagram](../assets/img/artifacts/6nutrismart-NutritionFrontendDiagram.png)

 - **Metabolic Adaptation:** Gestiona las vistas de métricas corporales, historial de peso, objetivos metabólicos y registro de actividad.

   ![Metabolic Frontend Diagram](../assets/img/artifacts/7nutrismart-MetabolicFrontendDiagram.png)

- **Behavioral Consistency:** Gestiona las vistas de estado de adherencia, rachas y resumen de progreso conductual.

   ![Behavioral Frontend Diagram](../assets/img/artifacts/8nutrismart-BehavioralFrontendDiagram.png)

- **Restaurant Intelligence:** Gestiona las vistas de escaneo de menú, platos compatibles y mejor plato sugerido.

   ![Restaurant Frontend Diagram](../assets/img/artifacts/9nutrismart-RestaurantFrontendDiagram.png)

 - **Smart Recommendations:** Gestiona las vistas de recomendaciones personalizadas, Modo Viaje, Despensa y recomendaciones por clima.

   ![Recs Frontend Diagram](../assets/img/artifacts/10nutrismart-RecsFrontendDiagram.png)

 - **Analytics & Reporting:** Gestiona las vistas del dashboard, gráficas de progreso y rachas.

   ![Analytics Frontend Diagram](../assets/img/artifacts/11nutrismart-AnalyticsFrontendDiagram.png)

 - **Subscriptions & Billing:** Gestiona las vistas de planes de suscripción y pagos.

   ![Billing Frontend Diagram](../assets/img/artifacts/12nutrismart-BillingFrontendDiagram.png)

**B. API Application Components (Backend)**

El API Application se organiza en 7 Bounded Contexts y un Shared Kernel, cada uno siguiendo el patrón de arquitectura del Domain-Driven Design.

El diagrama a continuación muestra todos los componentes de la arquitectura en un único bloque, dado que Structurizr no soporta la agrupación visual por Bounded Context en las vistas de componentes.

![API Component Diagram](../assets/img/artifacts/13nutrismart-APIComponentsDiagram.png)

Cada Bounded Context contiene una capa de Interfaces con los Controllers de Spring Boot que reciben las peticiones HTTP, una capa de Application con los servicios y comandos que orquestan los casos de uso, una capa de Domain con los agregados y entidades del dominio, y una capa de Infrastructure con los repositorios de Spring Data JPA y los clientes de APIs externas cuando corresponda.

Para apreciar la separación por capas Domain-Driven Design de cada Bounded Context, se presenta a continuación un diagrama de detalle individual por cada uno.

**Bounded Contexts:**

 - **Identity & Access:** Maneja la autenticación, autorización y perfiles de usuario.

   ![IAM Backend Diagram](../assets/img/artifacts/14nutrismart-IAMBackendDiagram.png)

 - **Nutrition Tracking:** Gestiona el registro de comidas y el procesamiento de Smart Scan. Se integra con Google Cloud Vision y Nutrition Data Providers.

   ![Nutrition Backend Diagram](../assets/img/artifacts/15nutrismart-NutritionBackendDiagram.png)

 - **Metabolic Adaptation:** Calcula BMI, BMR y TDEE, gestiona los objetivos calóricos y sincroniza datos de actividad desde Google Fit (Premium).

   ![Metabolic Backend Diagram](../assets/img/artifacts/16nutrismart-MetabolicBackendDiagram.png)

- **Behavioral Consistency:** Evalúa la adherencia diaria, detecta caídas conductuales y gestiona el sistema de rachas.

   ![Behavioral Backend Diagram](../assets/img/artifacts/17nutrismart-BehavioralBackendDiagram.png)

- **Restaurant Intelligence:** Procesa fotos de menús, filtra platos por restricciones y rankea las opciones más compatibles con el perfil del usuario. Se integra con Google Cloud Vision API y Nutritional Data Providers.

   ![Restaurant Backend Diagram](../assets/img/artifacts/18nutrismart-RestaurantBackendDiagram.png)

 - **Smart Recommendations:** Procesa datos contextuales para generar sugerencias personalizadas. Se integra con OpenWeatherMap y Geolocation API.

   ![Recs Backend Diagram](../assets/img/artifacts/19nutrismart-RecsBackendDiagram.png)

 - **Analytics & Reporting:** Genera gráficas de progreso, rachas y reportes del usuario.

   ![Analytics Backend Diagram](../assets/img/artifacts/20nutrismart-AnalyticsBackendDiagram.png)

 - **Subscriptions & Billing:** Gestiona los niveles de suscripción e integra con Stripe para el procesamiento de pagos.

   ![Billing Backend Diagram](../assets/img/artifacts/21nutrismart-BillingBackendDiagram.png)

**Shared Kernel:**

Componente transversal utilizado por todos los Bounded Contexts que agrupa clases base, interfaces compartidas y objetos de valor reutilizables. No contiene lógica de negocio propia ni acceso a base de datos.

Incluye los siguientes sub-componentes:
 
- **Base Domain:** Clases abstractas base para agregados, entidades y objetos de valor.
- **Common Interfaces:** Interfaces compartidas como `IRepository` y `IDomainEvent`.
- **Common Value Objects:** Objetos de valor reutilizables como `Money`, `DateRange` y `Pagination`.

![Shared Kernel Diagram](../assets/img/artifacts/22nutrismart-SharedKernelDiagram.png)

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams

## 4.8. Database Design

### 4.8.1. Database Diagrams