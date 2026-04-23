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

### 4.7.1. Class Diagrams

## 4.8. Database Design

Los diagramas de base de datos de NutriSmart se presentan a nivel físico, detallando la estructura completa de cada tabla junto con sus columnas, tipos de datos nativos de PostgreSQL, restricciones de integridad referencial y relaciones entre entidades. El diseño está organizado por Bounded Context, de modo que cada contexto delimitado agrupa sus propias tablas bajo un prefijo de esquema consistente con el lenguaje ubicuo del dominio.

**Características principales consideradas en los diagramas**

**Prefijos de esquema por Bounded Context.** Cada contexto agrupa sus tablas bajo un prefijo propio: `iam_` para Identity & Access Management, `nutrition_` para Nutrition Tracking, `body_` para Body & Health Metrics, `recs_` para Smart Recommendations, `activity_` para Activity & Wearable Sync, `analytics_` para Analytics & Reporting, y `billing_` para Subscriptions & Billing. Esto refleja los límites del dominio directamente en la capa de persistencia y evita colisiones de nombres entre contextos.

**Primary Keys con UUID.** Todas las tablas utilizan `UUID` como tipo de dato para sus claves primarias, generadas mediante `gen_random_uuid()`. Esta decisión es consistente con los Value Objects de identidad definidos en el dominio (`UserId`, `NutritionLogId`, `BodyProfileId`, etc.) y permite la generación distribuida de identificadores sin dependencia de secuencias de base de datos.

**Foreign Keys e integridad referencial.** Las relaciones entre tablas se establecen mediante `FOREIGN KEY`, aplicando `ON DELETE CASCADE` cuando los registros hijos no tienen sentido sin su padre (por ejemplo, `nutrition_food_entries` respecto a `nutrition_logs`), y `ON DELETE RESTRICT` implícito en casos donde la eliminación debe bloquearse para proteger la integridad del negocio.

**Normalización en tercera forma normal (3NF).** El diseño evita la redundancia de datos. Los Value Objects compuestos como `MacroNutrients` se persisten como columnas individuales dentro de la tabla de su entidad contenedora, dado que no tienen identidad propia y su ciclo de vida está ligado al aggregate raíz.

**Columnas de auditoría.** Todas las tablas raíz de aggregate incluyen `created_at TIMESTAMP NOT NULL DEFAULT now()` y `updated_at TIMESTAMP NOT NULL DEFAULT now()` para trazabilidad temporal de cada registro.

**Tipos de datos PostgreSQL.** Se utilizan tipos nativos: `UUID` para identificadores, `NUMERIC(p,s)` para valores monetarios y medidas con precisión decimal, `TEXT` para cadenas sin límite fijo, `VARCHAR(n)` para cadenas con restricción de longitud conocida, `DATE` para fechas sin componente horario, `TIMESTAMP` para marcas de tiempo completas, `INTEGER` para conteos enteros y `BOOLEAN` para flags binarios.

**Índices.** Se definen índices sobre las columnas de búsqueda más frecuentes: `user_id` en todas las tablas asociadas a un usuario, `email` en `iam_users`, y la combinación `(user_id, date)` en tablas de registros diarios como `nutrition_logs` y `activity_logs`, optimizando las consultas de dashboard y reportes.

**`iam_users` como tabla central.** La tabla `iam_users` del contexto Identity & Access Management actúa como referencia central del sistema. Todos los demás contextos referencian a esta tabla mediante `user_id`, respetando el principio de que la identidad del usuario es gestionada exclusivamente por el contexto IAM.

### 4.8.1. Database Diagrams

El diagrama a continuación presenta el modelo entidad-relación físico general de NutriSmart, consolidando las tablas de los siete Bounded Contexts y sus relaciones de integridad referencial.

![NutriSmart ERD](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-report/main/docs/database-diagrams/nutrismart-erd.puml)