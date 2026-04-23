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
| **Identity & Access** | Gestión de autenticación, autorización y perfiles de usuario. | User & Auth |
| **Nutrition Tracking** | Registro y análisis de alimentos mediante logs y Smart Scan. | Nutrition Log, Smart Scan |
| **Body & Health Metrics** | Seguimiento de indicadores corporales (IMC, TDEE) y metas. | Body Tracking |
| **Smart Recommendations** | Motor de sugerencias personalizadas según contexto y clima. | Recommendations Engine |
| **Activity & Wearable Sync** | Integración y sincronización con dispositivos físicos (Google Fit). | Wearable Sync |
| **Analytics & Reporting** | Generación de dashboards, progreso visual y reportes. | Dashboard & Analytics |
| **Subscriptions & Billing** | Gestión de planes, facturación y control de features Premium. | Subscriptions |

### 4.6.1. Design-Level EventStorming

En esta sección se presenta el modelado del comportamiento del sistema mediante la técnica de EventStorming a nivel de diseño. Este proceso permitió identificar los eventos de dominio y los comandos que disparan la lógica de negocio en cada Bounded Context, estableciendo las reglas de reacción del sistema ante acciones del usuario o políticas automaticas.

A continuación, se detalla la matriz de interdependencias que asegura la reactividad y sincronización de datos entre los distintos módulos:
| Origen (Evento) | Destino (Comando) | Descripción |
| :--- | :--- | :--- |
| **Identity:** User Registered | **Body Metrics:** Register Body Metrics | Inicializa el perfil de salud y metas al crear la cuenta. |
| **Nutrition:** Consumption Updated (Created/Updated/Deleted) | **Analytics:** Generate Progress Insights | Sincroniza indicadores y gráficas de consumo diario ante cualquier cambio en el log. |
| **Nutrition:** Consumption Updated (Created/Updated/Deleted) | **Smart Recs:** Generate Recommendation | Ajusta las sugerencias alimenticias en tiempo real según los macros consumidos y el déficit calórico del día. |
| **Activity:** Caloric Balance Adjusted | **Analytics:** Generate Progress Insights | Refleja el gasto energético por actividad física o sincronización con wearable en los reportes de progreso. |
| **Body Metrics:** TDEE Calculated | **Analytics:** Generate Progress Insights | Compara objetivos metabólicos teóricos frente al progreso real registrado. |
| **Body Metrics:** TDEE Calculated | **Smart Recs:** Generate Recommendation | Personaliza las porciones y sugerencias de comida según el perfil físico y la meta calórica actualizada del usuario. |
| **Subscriptions:** Benefits Enabled | **Smart Recs:** Unlock Premium Features | Habilita el acceso a algoritmos de recomendación avanzada y análisis detallado por IA. |
| **Subscriptions:** Benefits Disabled | **Smart Recs:** Lock Premium Features | Restringe el acceso a funcionalidades avanzadas tras la expiración o cancelación del plan. |

**EventStorming**

![EventStorming Diagram](../assets/img/artifacts/eventStorming.png)

Para poder apreciar mejor el EventStorming le recomendamos ingresar al siguiente link:
<br>[Visualizar EventStorming en Miro](https://miro.com/welcomeonboard/ZGpHbU1hMVZnYmpjUWg4NFQzOGcyVllGYndBSGRLa2dNcFErY0RnMVJKMWt5ekRVbUhQWXBQV2RFVTFZYzdwTVFnUmJYVHRwN2ZuanhYcDhGaHFFdXpqSXhvNThQV28wWnlBTXZDMFE5SXBGVTBCWk9SdmtWR3dDT0Q3WU82eXN0R2lncW1vRmFBVnlLcVJzTmdFdlNRPT0hdjE=?share_link_id=642611168323)

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

![Context Diagram]()

### 4.6.3. Software Architecture Container Diagrams

El Diagrama de Contenedores (Nivel 2 del modelo C4) desglosa el sistema NutriSmart en sus principales unidades lógicas de ejecución. En este nivel, se especifican las responsabilidades de cada contenedor, las tecnologías elegidas para su implementación y los protocolos de comunicación que permiten la interacción entre ellos y con los sistemas externos.

**Elementos:**

 - **Web Application:** Servidor web que entrega los archivos estáticos al navegador del usuario para inicializar la aplicación.
    - **Tecnología:** `Nginx`.
 - **Single Page Application:** Frontend donde los usuarios interactúan con la plataforma, gestionan sus metas y visualizan sus progresos. Se ejecuta completamente en el navegador del usuario.
    - **Tecnología:** `Angular (con Angular Material para UI y RxJS para la gestión de servicios)`.
 - **API Application:** Backend que maneja la lógica de negocio, el motor de recomendaciones, el procesamiento de imágenes y la integración con servicios externos.
    - **Tecnología:** `Spring Boot (Java)`.
 - **Database:** Almacena la información de usuarios, registros nutricionales, historial de métricas y datos de facturación.
    - **Tecnología:** `PostgreSQL`.
 - **External Systems:** APIs de terceros que se integran con el backend para extender las capacidades del sistema.
    - **Tecnología:** `JSON/HTTPS (REST)`.

![Container Diagram]()

![Container Diagram Summarized]()

### 4.6.4. Software Architecture Components Diagrams

El Diagrama de Componentes (Nivel 3 del modelo C4) describe la estructura interna de los contenedores principales de NutriSmart. En esta sección se detallan los módulos lógicos, sus responsabilidades específicas y las tecnologías utilizadas para la implementación de cada componente.

**A. Single Page Application Components (Frontend)**

Este contenedor se organiza para garantizar una interfaz reactiva siguiendo el patrón de arquitectura de Angular.

**Elementos:**

 - **UI Components:** Biblioteca de vistas y elementos visuales basados en Material Design.
    - **Tecnología:** `Angular Material`.
 - **Angular Router:** Componente encargado de la navegación y el enrutamiento del lado del cliente.
    - **Tecnología:** `Angular Router`.
 - **Data Services:** Servicios encargados de la lógica de negocio del lado del cliente y el manejo de flujos de datos asíncronos.
    - **Tecnología:** `RxJS`.
 - **HTTP Client:** Encargado de orquestar las peticiones asíncronas y la comunicación con el servidor de API.
    - **Tecnología:** `HttpClient (Angular)`.

![Web Component Diagram]()

![Web Component Diagram Summarized]()

**B. API Application Components (Backend)**

El backend se divide en módulos que representan los 7 Bounded Contexts del dominio, asegurando una arquitectura desacoplada y escalable. Adicionalmente, cuenta con un Data Access Layer que centraliza la persistencia de datos mediante el patrón Repository, gestionando todas las operaciones de lectura y escritura hacia la base de datos.

**Elementos:**

 - **Modulos de Dominio (Identity, Nutrition, Health, Recs, Activity, Analytics, Billing):** Implementan las reglas de negocio específicas para cada contexto identificado.
    - **Tecnología:** `Java / Spring Boot (Services & Controllers)`.
 - **Data Access Layer (Repository):** Componente que centraliza la persistencia de la información mediante el uso de abstracciones de datos.
    - **Tecnología:** `Spring Data JPA / Hibernate`.

![API Component Diagram]()

![API Component Diagram Summarized]()

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams

## 4.8. Database Design

### 4.8.1. Database Diagrams