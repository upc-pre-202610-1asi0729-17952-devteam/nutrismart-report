# CAPÍTULO II: REQUIREMENTS ELICITATION & ANALYSIS

## 2.1. Competidores

### 2.1.1. Análisis competitivo

### 2.1.2. Estrategias y tácticas frente a competidores

## 2.2. Entrevistas

### 2.2.1. Diseño de entrevistas

### 2.2.2. Registro de entrevistas

### 2.2.3. Análisis de entrevistas

## 2.3. Needfinding

Para comprender de manera integral las necesidades, comportamientos y motivaciones de los usuarios de nuestra plataforma, se realizaron entrevistas cualitativas y análisis de experiencias relacionadas con el seguimiento nutricional y hábitos de salud. Estas interacciones permiten explorar las dificultades en el registro de alimentos, la interpretación de datos nutricionales y la falta de personalización en las recomendaciones. Asimismo, se identificaron barreras como la desmotivación, la complejidad de uso de aplicaciones existentes y la escasa retroalimentación en tiempo real. Este proceso permitió reconocer tanto necesidades explícitas como implícitas, estableciendo una base sólida para el diseño de una solución centrada en el usuario, eficiente y alineada con sus objetivos de bienestar. 

### 2.3.1. User Personas

**Segmento 1: Pérdida de peso**

![nombre](../assets/img/chapter2-neeedfinding-images/JorgeDelAguilaVacalla(2).png)

**Segmento 2: Ganancia de masa muscular**

![nombre](../assets/img/chapter2-neeedfinding-images/DaphneFaustorVergaray(1).png)


### 2.3.2. User Task Matrix

**Segmento 1: Pérdida de peso**
<table>
  <thead>
    <tr>
      <th rowspan="2">Task</th>
      <th colspan="2">Jorge Del Aguila</th>
      <th colspan="2">Anthony López</th>
      <th colspan="2">Evelyn Díaz</th>
    </tr>
    <tr>
      <th>Frequency</th>
      <th>Importance</th>
      <th>Frequency</th>
      <th>Importance</th>
      <th>Frequency</th>
      <th>Importance</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Control the amount of food consumed daily</td>
      <td>Normally</td>
      <td>High</td>
      <td>Sometimes</td>
      <td>Medium</td>
      <td>Normally</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Estimate the calories of food before consuming them</td>
      <td>Normally</td>
      <td>High</td>
      <td>Sometimes</td>
      <td>Medium</td>
      <td>Normally</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Decide what to eat when away from home</td>
      <td>Sometimes</td>
      <td>Medium</td>
      <td>Normally</td>
      <td>High</td>
      <td>Sometimes</td>
      <td>Medium</td>
    </tr>
    <tr>
      <td>Evaluate progress in relation to weight</td>
      <td>Normally</td>
      <td>High</td>
      <td>Sometimes</td>
      <td>Medium</td>
      <td>Normally</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Avoid foods perceived as unhealthy</td>
      <td>Normally</td>
      <td>High</td>
      <td>Sometimes</td>
      <td>Medium</td>
      <td>Normally</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Adapt eating habits according to daily routine</td>
      <td>Normally</td>
      <td>High</td>
      <td>Normally</td>
      <td>High</td>
      <td>Normally</td>
      <td>High</td>
    </tr>
  </tbody>
</table>

<br>

**Segmento 2: Ganancia de masa muscular**

<table>
  <thead>
    <tr>
      <th rowspan="2">Task</th>
      <th colspan="2">Daphne Vergaray</th>
      <th colspan="2">David Ramos</th>
      <th colspan="2">Maria Roque</th>
    </tr>
    <tr>
      <th>Frequency</th>
      <th>Importance</th>
      <th>Frequency</th>
      <th>Importance</th>
      <th>Frequency</th>
      <th>Importance</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Calculate the amount of protein consumed daily</td>
      <td>Normally</td>
      <td>High</td>
      <td>Sometimes</td>
      <td>Medium</td>
      <td>Normally</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Plan meals according to muscle gain physical goals</td>
      <td>Normally</td>
      <td>High</td>
      <td>Normally</td>
      <td>High</td>
      <td>Normally</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Adjust nutrition according to physical activity</td>
      <td>Normally</td>
      <td>High</td>
      <td>Normally</td>
      <td>High</td>
      <td>Normally</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Search for suitable options when eating away from home</td>
      <td>Normally</td>
      <td>High</td>
      <td>Normally</td>
      <td>High</td>
      <td>Sometimes</td>
      <td>Medium</td>
    </tr>
    <tr>
      <td>Maintain consistency in nutrition over time</td>
      <td>Sometimes</td>
      <td>Medium</td>
      <td>Normally</td>
      <td>High</td>
      <td>Normally</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Evaluate if foods meet nutritional requirements</td>
      <td>Normally</td>
      <td>High</td>
      <td>Normally</td>
      <td>High</td>
      <td>Sometimes</td>
      <td>Medium</td>
    </tr>
  </tbody>
</table>

**Análisis de User Task Matrix**

El análisis de las matrices permite identificar patrones clave en el comportamiento de los usuarios y extraer información relevante para el desarrollo de nuestra plataforma.
En el segmento de pérdida de peso, las tareas con mayor frecuencia e importancia se centran en el control de la ingesta alimentaria y la toma de decisiones en contextos cotidianos. Destacan especialmente controlar la cantidad de alimentos consumidos y decidir qué comer fuera de casa, lo que evidencia que los principales desafíos no radican únicamente en el conocimiento nutricional, sino en la incertidumbre al momento de elegir en situaciones reales.

En el segmento de ganancia de masa muscular, las tareas críticas están orientadas a la optimización nutricional, principalmente en el cálculo de proteínas y la evaluación de requerimientos nutricionales. Esto refleja un comportamiento más analítico, donde la precisión y la consistencia son determinantes para alcanzar los objetivos físicos.

Al comparar ambos segmentos, se identifican similitudes relevantes: en ambos casos, existe una alta importancia en el control de la alimentación y en la toma de decisiones fuera del entorno controlado. Sin embargo, difieren en su enfoque: el segmento de pérdida de peso tiende a ser más reactivo y contextual, mientras que el de ganancia muscular es más planificado y orientado a métricas específicas.

A partir de ello, se derivan insights clave para nuestra plataforma. En primer lugar, es fundamental diseñar soluciones que brinden soporte en la toma de decisiones en tiempo real, especialmente en contextos como restaurantes o situaciones variables. En segundo lugar, la plataforma debe ofrecer niveles diferenciados de profundidad, combinando simplicidad para usuarios que buscan orientación rápida y precisión para aquellos que requieren control detallado de nutrientes. Finalmente, se valida que el uso de datos contextuales como la ubicación, clima y la disponibilidad que representan un factor crítico para mejorar la relevancia de las recomendaciones y la adherencia del usuario.

En conjunto, estos hallazgos orientan el desarrollo de nuestra plataforma hacia una solución adaptativa, contextual y centrada en el usuario, capaz de responder a necesidades reales y mejorar la toma de decisiones alimenticias de manera efectiva.

### 2.3.3. User Journey Mapping

**Segmento 1: Pérdida de peso**

![nombre](../assets/img/chapter2-neeedfinding-images/JorgeDelAguila_UJM(4).png)

**Segmento 2: Ganancia de masa muscular**

![nombre](../assets/img/chapter2-neeedfinding-images/DaphneFaustorVergaray_UJM(1).png)

### 2.3.4. Empathy Mapping

**Segmento 1: Pérdida de peso**

![nombre](../assets/img/chapter2-neeedfinding-images/JorgeDelAguila_EM(1).png)

**Segmento 2: Ganancia de masa muscular**

![nombre](../assets/img/chapter2-neeedfinding-images/DaphneFaustorVergaray_EM(1).png)

## 2.4. Big Picture EventStorming

En esta sección se desarrolla el modelado del dominio del sistema mediante la técnica de Big Picture Event Storming, con el propósito de construir una visión integral del negocio de nuestra plataforma bajo los principios de Domain Driven Design. Este proceso permitió identificar los eventos de dominio más relevantes, estableciendo su secuencia temporal y las relaciones de causalidad que definen el comportamiento del sistema a nivel global.

El análisis realizado permitió, además, delimitar los actores que interactúan con el dominio, así como los comandos que representan las intenciones de cambio de estado y los sistemas externos que participan en la ejecución de los procesos de negocio. Esto evidencia una arquitectura orientada a eventos, caracterizada por un alto nivel de desacoplamiento y consistencia eventual entre los distintos componentes del sistema. 

Asimismo, se identificaron eventos de alta relevancia que actúan como mecanismos de propagación, especialmente aquellos asociados al registro de consumo nutricional, los cuales desencadenan procesos en múltiples bounded contexts como analítica, recomendaciones inteligentes y gestión de métricas de salud.

Finalmente, la estructuración del Big Picture Event Storming organiza los elementos del dominio en flujos de negocio coherentes, permitiendo visualizar las interdependencias entre bounded contexts, la secuencia lógica de ejecución y los principales puntos de integración. Este enfoque contribuye a la alineación entre el modelo de dominio y los procesos del negocio, además de facilitar la identificación de oportunidades de mejora en la arquitectura del sistema.


**Big Picture Event Storming**

![Big Picture Event Storming](../assets/img/chapter2-neeedfinding-images/BigPictureEventStorming.jpg)

Para poder apreciar mejor el Big Picture Event Storming, le recomendamos ingresar al siguiente link: [Tablero de Miro: Big Picture Event Storming](https://miro.com/app/board/uXjVGnTlN0E=/?share_link_id=736747337916)


## 2.5. Ubiquitous Language

El presente Ubiquitous Language establece un conjunto estructurado de términos y conceptos clave propios del dominio de nuestra plataforma, con el propósito de definir un lenguaje común, preciso y libre de ambigüedades entre los distintos stakeholders y el equipo de desarrollo. Este glosario se fundamenta en los principios de Domain Driven Design, permitiendo alinear la comprensión del negocio de la nutrición personalizada, el seguimiento de métricas de salud y la generación de recomendaciones contextuales. Cada término ha sido definido considerando su significado específico dentro del dominio, garantizando consistencia semántica, trazabilidad conceptual y una comunicación efectiva que facilite el análisis, diseño e implementación de la solución.



**User & Profile**

| Term                                                    | Definition                                                                                                                              |
|---------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| User (Usuario)                                          | The person using the platform to manage their nutrition, physical activity, and health goals.                                            |
| User Profile (Perfil de Usuario)                        | The set of personal and health data for the user, such as age, sex, weight, height, activity level, and dietary restrictions.           |
| Goal (Meta)                                             | The user's primary objective related to their physical state: losing weight, gaining muscle mass, or maintaining their current condition. |
| Dietary Restrictions (Restricciones Alimentarias)       | Limitations on the user's diet due to allergies, intolerances, or medical conditions.                                                   |
| Subscription Plan (Plan de Suscripción)                 | Access level contracted by the user (Basic, Pro, Premium) that determines available features.                                           |

---

**Body & Health Metrics**

| Term                                                    | Definition                                                                                                                              |
|---------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Weight (Peso)                                           | Body measurement of the user recorded periodically to evaluate progress.                                                                |
| Height (Altura)                                         | Physical measurement used alongside weight to calculate health indicators.                                                              |
| BMI / Body Mass Index (IMC / Índice de Masa Corporal)   | An indicator that relates weight and height to estimate the user's physical status.                                                     |
| BMR / Basal Metabolic Rate (TMB / Tasa Metabólica Basal)| The amount of calories the body needs at rest for vital functions.                                                                      |
| TDEE / Total Daily Energy Expenditure (Gasto Calórico Diario Total) | The total calories the user burns in a day, considering their physical activity.                                              |
| Daily Calorie Target (Objetivo Calórico Diario)         | The number of calories the user should consume daily according to their goal.                                                           |

---

**Nutrition Tracking**

| Term                                                    | Definition                                                                                                                              |
|---------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Meal (Comida)                                           | Food intake recorded at specific times of the day: breakfast, lunch, dinner, or snack.                                                  |
| Food Item (Alimento)                                    | Individual product consumed by the user with associated nutritional information.                                                         |
| Nutrition Log (Registro Nutricional)                    | History of food consumed by the user, organized by day.                                                                                 |
| Calories (Calorías)                                     | The unit of energy provided by the consumed food.                                                                                       |
| Macronutrients / Macros (Macronutrientes)               | The primary components of food: proteins, carbohydrates, and fats.                                                                      |
| Daily Intake (Consumo Diario)                           | Total calories and macronutrients consumed by the user in a day.                                                                        |

---

**Smart Scan**

| Term                                                    | Definition                                                                                                                              |
|---------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Smart Scan (Escaneo Inteligente)                        | A feature that analyzes images of food or menus to estimate their nutritional value.                                                    |
| Dish Photo (Foto de Plato)                              | An image of food taken by the user to identify its components and calories.                                                             |
| Menu Photo (Foto de Menú)                               | An image of a restaurant menu used to recommend healthy options.                                                                        |
| Food Analysis (Análisis de Alimento)                    | The process of estimating calories and macronutrients from an image.                                                                    |
| Manual Confirmation (Confirmación Manual)               | User validation of the analysis results before saving them.                                                                             |

---

**Recommendations**

| Term                                                    | Definition                                                                                                                              |
|---------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Recommendation (Recomendación)                          | Personalized suggestion of foods or meals based on the user's profile.                                                                  |
| Context Aware Recommendation (Recomendación Contextual) | A recommendation that considers factors such as weather, location, and user status.                                                     |
| Weather Condition (Condición Climática)                 | The state of the weather (heat, cold, etc.) that influences dietary recommendations.                                                    |
| Travel Mode (Modo Viaje)                                | A feature that adapts recommendations based on the city or country where the user is located.                                           |
| Pantry (Despensa)                                       | A list of ingredients available at home as recorded by the user.                                                                        |
| Recipe Suggestion (Sugerencia de Receta)                | A recommendation for food preparation based on available ingredients and nutritional needs.                                             |
| Macro Deficit (Déficit de Macronutrientes)              | The difference between the macronutrients consumed and those required for the day.                                                      |

---

**Activity & Energy Balance**

| Term                                                    | Definition                                                                                                                              |
|---------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Physical Activity (Actividad Física)                    | Exercise performed by the user that contributes to daily caloric expenditure.                                                           |
| Active Calories (Calorías Activas)                      | Calories burned through physical activity.                                                                                              |
| Energy Balance (Balance Calórico)                       | The relationship between calories consumed and calories burned in a day.                                                                |

---

**Progress & Analytics**

| Term                                                    | Definition                                                                                                                              |
|---------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Progress (Progreso)                                     | The user's evolution regarding their goal, based on body metrics and consumption.                                                       |
| Daily Summary (Resumen Diario)                          | An overview of calorie and macronutrient consumption against the daily target.                                                          |
| Streak (Racha)                                          | The number of consecutive days in which the user records their full information.                                                        |
| Alert (Alerta)                                          | A notification when the user exceeds or falls short of their nutritional goals.                                                         |
| Trend (Tendencia)                                       | The pattern of change in metrics such as weight or consumption over time.                                                               |

---

**Domain Concepts Clave**

| Term                                                    | Definition                                                                                                                              |
|---------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Personalized Nutrition (Nutrición Personalizada)        | An approach that adapts dietary recommendations to the user's characteristics and context.                                              |
| Health Goal Achievement (Logro de Objetivos de Salud)   | The fulfillment of physical goals through monitoring and recommendations.                                                               |
| Contextual Awareness (Conciencia Contextual)            | The system's ability to consider external factors such as weather and location.                                                         |