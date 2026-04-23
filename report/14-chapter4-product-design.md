# CAPÍTULO IV: PRODUCT DESIGN

## 4.1. Style Guidelines

### 4.1.1. General Style Guidelines

### 4.1.2. Web Style Guidelines

## 4.2. Information Architecture

### 4.2.1. Organization Systems


La organización del contenido en NutriSmart responde a dos contextos distintos: el Landing Page, dirigido a visitantes que aún evalúan la plataforma, y la Web Application, usada por usuarios registrados con metas nutricionales activas.

**Landing Page**

Se aplica una organización jerárquica (visual hierarchy) como criterio principal. La página ordena sus secciones de mayor a menor relevancia decisional:

1. Héroe con propuesta de valor
2. Funcionalidades destacadas
3. Segmentos de usuario (Perder peso / Ganar músculo)
4. Planes de suscripción
5. FAQ
6. Contacto

Esta disposición expone primero la información que impulsa la conversión y delega los detalles al desplazamiento progresivo. La categorización del contenido sigue un esquema por tópicos, agrupando bloques temáticamente independientes (features, pricings) a los que el usuario puede llegar desde el menú de navegación directamente.

**Web Application**

Dentro de la aplicación se combinan tres esquemas según la naturaleza de cada módulo. Se aplica organización secuencial (step-by-step) en los flujos de onboarding:

1. Configuración de meta
2. Datos físicos
3. Restricciones alimentarias
4. Confirmación

Y en el registro de comidas:

1. Selección de momento del día
2. Búsqueda del alimento
3. Confirmación de porción
4. Guardado en el log

Ambos flujos guían al usuario paso a paso para evitar errores y reducir la carga cognitiva. Se aplica organización jerárquica en el Dashboard principal, donde los indicadores más críticos (calorías consumidas vs. meta, macros del día) se presentan de forma prominente y los módulos secundarios (historial, recomendaciones, sincronización wearable) se acceden desde secciones subsiguientes. Se aplica organización matricial en la pantalla de comparación de planes de suscripción (Basic / Pro / Premium), donde las características se disponen en filas y los planes en columnas, y en el módulo de Analytics, donde múltiples métricas se presentan en paralelo. La categorización del contenido de la aplicación sigue además un esquema según audiencia: usuarios del segmento Perder peso ven recomendaciones orientadas a déficit calórico, mientras que los del segmento Ganar músculo visualizan objetivos de superávit y mayor peso en proteína.

### 4.2.2. Labeling Systems


Las etiquetas empleadas en NutriSmart priorizan la brevedad y la claridad, evitando tecnicismos que puedan confundir a usuarios no especializados.

**Landing Page**

| Etiqueta | Contenido que representa |
|---|---|
| About Us | Misión, visión y equipo de NutriSmart |
| Features | Catálogo completo de funcionalidades |
| Contact | Formulario y canales de contacto |
| Log In | Acceso a la Web Application |

**Web Application**

| Etiqueta | Contenido que representa |
|---|---|
| Dashboard | Resumen diario de calorías y macros |
| Nutrition Log | Registro de comidas por momento del día |
| Smart Scan | Análisis visual de platos y menús |
| Recommendations | Sugerencias contextuales (clima, viaje) |
| Pantry | Ingredientes disponibles y recetas |
| Body Tracking | Registro de peso, talla, BMI y TDEE |
| Wearable| Conexión con Google Fit |
| Analytics | Historial y reportes de progreso |
| Profile| Datos personales, restricciones, suscripción |
| Subscriptions | Planes y facturación |

Las etiquetas de encabezado dentro de cada módulo siguen la misma lógica de concisión: "Today's Summary", "Log a Meal", "Scan a Dish", "My Pantry", "Weekly Report". En todas las vistas se usan atributos `alt` descriptivos en imágenes e íconos para garantizar accesibilidad con lectores de pantalla.

### 4.2.3. SEO Tags and Meta Tags


A continuación se detallan los valores asignados a las principales páginas de la experiencia.

**Landing Page**

| Tag | Valor |
|---|---|
| Title | NutriSmart: Smart Nutrition, Your Way |
| Description | NutriSmart is the smart nutrition platform that adapts meal recommendations to your location, weather, and health profile. Lose weight or gain muscle, on your terms. |
| Keywords | nutrition app, calorie tracker, smart nutrition, weight loss, muscle gain, meal planner, food tracker, NutriSmart, diet app, healthy eating |
| Author | NutriSmart Team |

**Features Page**

| Tag | Valor |
|---|---|
| Title | Features: NutriSmart |
| Description | Explore all NutriSmart features: Smart Scan food analysis, weather-based recommendations, travel mode, pantry recipes, wearable sync, and more. |
| Keywords | NutriSmart features, smart scan, calorie tracker, travel mode, weather nutrition, meal logging, wearable sync, recipe ideas, menu analysis |
| Author | NutriSmart Team |

**About Us Page**

| Tag | Valor |
|---|---|
| Title | About Us: NutriSmart |
| Description | Learn about the NutriSmart team and our mission to empower people to eat better through visual food analysis and context-aware smart recommendations. |
| Keywords | NutriSmart team, about NutriSmart, nutrition mission, healthy eating platform, Latin America nutrition app |
| Author | NutriSmart Team |

**Contact Page**

| Tag | Valor |
|---|---|
| Title | Contact: NutriSmart |
| Description | Get in touch with the NutriSmart team. Send us a message for questions, feedback, or partnership inquiries. |
| Keywords | NutriSmart contact, nutrition app support, feedback, partnership, customer service |
| Author | NutriSmart Team |

**Web Application**

| Tag | Valor |
|---|---|
| Title | NutriSmart App – Your Smart Nutrition Assistant |
| Description | Log your meals, analyze dishes with your camera, and receive personalized recommendations based on your weather and location. Reach your goal with NutriSmart. |
| Keywords | nutrition log, calorie tracking, smart scan, weather recommendations, travel mode, wearable sync, NutriSmart app, meal tracker, healthy eating assistant |
| Author | NutriSmart Team |

Todas las páginas incluyen `charset="UTF-8"`, `robots: index, follow`, etiqueta canónica (`rel="canonical"`) y Open Graph tags para compartir en redes sociales.

### 4.2.4. Searching Systems

El sistema de búsqueda de NutriSmart está presente principalmente dentro de la Web Application, en los módulos donde el volumen de datos podría abrumar al usuario si no se ofrecen medios de filtrado eficientes.

**Nutrition Log**

Al registrar una comida, el usuario accede a una barra de búsqueda con las siguientes capacidades:

- *Búsqueda por nombre*: el usuario escribe el nombre del alimento y el sistema muestra resultados en tiempo real desde la base de datos nutricional.
- *Historial de recientes*: los últimos alimentos registrados se muestran debajo del campo de búsqueda para agilizar el reingreso de comidas habituales.

Tras la búsqueda, cada resultado muestra: nombre del alimento, calorías por porción estándar, macros principales (P / C / G) y una opción para ajustar la cantidad antes de guardar.

**Pantry**

El usuario puede buscar ingredientes disponibles en su despensa. El sistema cruza los ingredientes registrados con la base de recetas y filtra las sugerencias por: restricciones alimentarias del perfil (aplicadas automáticamente) y objetivo nutricional (alto en proteína, bajo en carbohidratos, equilibrado).

Los resultados se presentan como tarjetas con: nombre de la receta, imagen referencial, tiempo estimado de preparación, calorías por porción y compatibilidad con el perfil del usuario.

**Analytics**

En la pantalla de análisis, el usuario puede filtrar su historial por: rango de fechas (última semana, último mes, rango personalizado), métrica a visualizar (calorías, proteínas, carbohidratos, grasas, peso corporal) y tipo de vista (gráfico de líneas, gráfico de barras, tabla de datos). Los filtros aplicados se muestran como chips activos sobre el gráfico, con opción de eliminarlos individualmente.

### 4.2.5. Navigation Systems


La navegación del Landing Page se articula mediante una barra fija en la parte superior (sticky navbar) que permanece visible durante el scroll, con las secciones principales (About Us, Features, Contact) y el acceso directo a Log In.

<div align="center">
  <img src="../assets/img/information-architecture/landing.png" alt="nav-system of landing"/>
</div>

La Web Application utiliza una barra lateral de navegación persistente (sidebar) que organiza los módulos en dos bloques: acciones principales en la parte superior (Dashboard, Nutrition Log, Smart Scan, Recommendations, Pantry, Body Tracking) y configuración en la parte inferior (Analytics, Wearable, Profile, Subscriptions), permitiendo al usuario acceder a cualquier módulo en un solo clic desde cualquier pantalla. 

<div align="center">
  <img src="../assets/img/information-architecture/webapp.png" alt="nav-system of webapp"/>
</div>

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

### 4.8.1. Database Diagrams