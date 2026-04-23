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

### 4.6.1. Design-Level EventStorming

### 4.6.2. Software Architecture Context Diagram

### 4.6.3. Software Architecture Container Diagrams

### 4.6.4. Software Architecture Components Diagrams

## 4.7. Software Object-Oriented Design
 
En total se presentan catorce diagramas, siete por cada capa, uno por cada Bounded Context definido en la arquitectura DDD del producto.
 
**Características principales**

**Arquitectura DDD en capas**
 
El backend estructura cada Bounded Context en cuatro paquetes:
 
- `domain`: contiene aggregates, entities, value objects y domain events.
- `application`: aloja los command services y query services junto con sus respectivos commands y queries.
- `infrastructure`: implementa los repositorios JPA y los adaptadores hacia APIs externas.
- `interfaces`: expone los REST controllers, los assemblers y los recursos de entrada/salida.
El frontend replica esta separación en las capas `domain/model`, `application/services`, `infrastructure/http` y `presentation/components`.
 
**Aggregates como raíz de consistencia**
 
Cada Bounded Context define uno o más aggregates raíz que encapsulan la lógica de negocio y controlan el acceso a sus entidades internas. Por ejemplo:
 
- `NutritionLog` en el contexto de *Nutrition Tracking*
- `BodyProfile` en *Body & Health Metrics*
- `Subscription` en *Subscriptions & Billing*
Ninguna entidad interna es accesible directamente desde fuera del aggregate.
 
**Value Objects inmutables**
 
Los conceptos del dominio que se identifican por su valor y no por su identidad se modelan como value objects: `Email`, `Weight`, `Height`, `MacroNutrients`, `Money`, `RecommendationContext`, entre otros. Su inmutabilidad se refleja en la ausencia de setters y en constructores que validan su estado inicial.
 
**Domain Events**
 
Cada aggregate publica eventos de dominio que representan hechos significativos del negocio:
 
- `UserRegistered`
- `ConsumptionUpdated`
- `CaloricBalanceAdjusted`
- `SubscriptionActivated`
Estos eventos habilitan la integración reactiva entre contextos, tal como se definió en el Event Storming de diseño.
 
**Interfaces de repositorio en el dominio**
 
Siguiendo el principio de inversión de dependencias, las interfaces de repositorio se declaran en la capa de dominio (por ejemplo, `UserRepository`, `NutritionLogRepository`) y sus implementaciones concretas residen en la capa de infraestructura (por ejemplo, `UserRepositoryImpl`). Esto garantiza que el dominio no dependa de tecnologías de persistencia específicas.
 
**Command/Query Separation**
 
Los application services se dividen en:
 
- **Command services:** modifican el estado del sistema.
- **Query services:** solo consultan el estado.
Siguiendo el patrón CQRS ligero adoptado en el proyecto, los commands y queries son objetos inmutables con los datos necesarios para cada operación.

**Angular Signals en el frontend**
 
Los servicios del frontend utilizan `WritableSignal` y `Signal` de Angular para gestionar el estado reactivo de forma eficiente. Los componentes consumen estos signals directamente o mediante `InputSignal` para los inputs declarativos, en línea con el patrón enseñado en los ejemplos de clase.
 
**Integración con APIs externas**
 
Los adaptadores de infraestructura modelan la comunicación con servicios externos, manteniéndolos aislados del dominio mediante interfaces:
 
- **Open Food Facts**
- **USDA FoodData Central**
- **OpenWeatherMap**
- **Google Fit**

### 4.7.1. Class Diagrams

**FrontEnd**

**Identity & Access Management**

![IAM Frontend](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-report/feature/chapter4-class-diagrams/docs/class-diagrams/frontend/iam.puml)

**Nutrition**

![Nutrition Frontend](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-report/feature/chapter4-class-diagrams/docs/class-diagrams/frontend/nutrition.puml)

**Body-metrics**

![Body-metrics Frontend](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-report/feature/chapter4-class-diagrams/docs/class-diagrams/frontend/body-metrics.puml)

**Recommendations**

![Recommendations Frontend](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-report/feature/chapter4-class-diagrams/docs/class-diagrams/frontend/recommendations.puml)

**Activity**

![Activity Frontend](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-report/feature/chapter4-class-diagrams/docs/class-diagrams/frontend/activity.puml)

**Analytics**

![Analytics Frontend](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-report/feature/chapter4-class-diagrams/docs/class-diagrams/frontend/analytics.puml)

**Billing**

![Activity Frontend](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-report/feature/chapter4-class-diagrams/docs/class-diagrams/frontend/billing.puml)

## 4.8. Database Design

### 4.8.1. Database Diagrams