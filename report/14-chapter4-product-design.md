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

Tras definir la estructura arquitectónica de contenedores y componentes, se procede al diseño orientado a objetos del software. En esta etapa, se detallan las clases, sus responsabilidades y las relaciones que darán vida a NutriSmart, permitiendo una transición fluida desde la arquitectura lógica hacia la implementación técnica.

El diseño se fundamenta en los pilares fundamentales de la Programación Orientada a Objetos (POO) para garantizar un sistema modular, escalable y de fácil mantenimiento:

- **Encapsulamiento:** Para proteger la integridad de los datos sensibles de salud, asegurando que el estado de los objetos solo sea accesible mediante modificadores de acceso.
- **Abstracción:** Para simplificar procesos complejos, como la integración con múltiples APIs externas de visión artificial y clima, mediante el uso de interfaces de Spring y clases abstractas.
- **Herencia y Polimorfismo:** Para promover la reutilización de código y la flexibilidad del sistema, permitiendo que diferentes tipos de registros nutricionales o planes de suscripción compartan comportamientos base pero se especialicen según sus reglas de negocio.
- **Modularidad:** Estructurando las clases de acuerdo con los 7 Bounded Contexts identificados, asegurando que el diseño esté estrictamente alineado con los requerimientos funcionales del dominio.

A continuación, se presentan los diagramas de clases que reflejan la estructura lógica del software, incluyendo sus atributos, métodos y multiplicidad de relaciones.

### 4.7.1. Class Diagrams

## 4.8. Database Design

### 4.8.1. Database Diagrams