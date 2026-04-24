# CAPÍTULO IV: PRODUCT DESIGN

## 4.1. Style Guidelines

### 4.1.1. General Style Guidelines


NutriSmart busca un tono equilibrado entre lo motivador y lo accesible, con un lenguaje claro, empático y alentador, orientado a personas que desean mejorar sus hábitos alimenticios sin sentirse abrumadas. La comunicación es entusiasta pero serena, formal en la información nutricional y casual en los mensajes de acompañamiento al usuario. Se evita el tono intimidante o clínico, priorizando cercanía y confianza.

**Branding**

La identidad visual de NutriSmart busca transmitir bienestar, modernidad y confianza. El nombre combina "Nutrición" y "Smart" (tecnología), reflejando la propuesta de una plataforma inteligente que adapta las recomendaciones al contexto del usuario. El logo, acompañado del nombre en tipografía Poppins, transmite una imagen limpia y contemporánea, apta tanto para interfaces digitales como para materiales de comunicación.

<p align="center">
  <img src="../assets/img/nutrismart-logo.png" alt="NutriSmart Logo" />
</p>

**Typography**

Para mantener la legibilidad y la personalidad visual de NutriSmart se establecen dos tipografías complementarias: Poppins como fuente primaria y Questrial como fuente secundaria, ambas provenientes de Google Fonts y con alta compatibilidad en entornos digitales.

Poppins es una sans-serif geométrica de corte moderno, utilizada en títulos y encabezados. Sus variantes de peso (400, 500, 600, 700 y 800) permiten establecer jerarquías visuales claras. Su geometría transmite energía, precisión y modernidad, valores centrales de la marca.

Questrial es una sans-serif de trazo amigable y legible, utilizada para cuerpos de texto, párrafos y elementos secundarios. Su diseño redondeado complementa a Poppins aportando calidez y accesibilidad en la lectura extendida.

Los tamaños base definidos son: H1 en 48px, H2 en 36px, H3 en 28px, H4 en 24px, cuerpo de texto en 16px y caption en 13px. 

<p align="center">
  <img src="../assets/img/style-guidelines/poppins.png" alt="Poppins" /> <img src="../assets/img/style-guidelines/questrial.png" alt="Questrial" />
</p>

**Colors**

La paleta de NutriSmart fue diseñada para evocar salud, naturaleza y bienestar digital, con tonos cálidos y orgánicos que contrastan con un color principal de acento tecnológico.

El color principal es el verde azulado (`#508B89`), que transmite calma, salud y equilibrio. Se emplea en el header, botones primarios, íconos activos y elementos de navegación. Su variante oscura (`#3A6A68`) se utiliza en estados hover y énfasis de interacción.

Como color de fondo predominante se usa el melocotón muy claro (`#FFE9DE`), que aporta calidez y diferencia a NutriSmart de plataformas de salud de estética clínica. El color de llamada a la acción es un melocotón medio (`#F4C5AE`), complementado por su variante activa (`#E0A98E`), que se aplica en botones secundarios y elementos interactivos.

Los colores neutros incluyen blanco (`#FFFFFF`) para fondos limpios, negro (`#000000`) para textos de alto contraste y dos tonos de texto: gris oscuro (`#1A1A1A`) para texto principal y gris medio (`#5C5C5C`) para texto secundario. El color de bordes y separadores es un gris cálido (`#E0D6D0`) que armoniza con el fondo melocotón.

<p align="center">
  <img src="../assets/img/style-guidelines/colors.png" alt="Colors" />
</p>

**Spacing**

Se establece una unidad base de 8px para el espaciado interno de componentes. Los márgenes mínimos entre secciones son de 16px en mobile y 24px en desktop. Para los contenedores principales se define un ancho máximo de 1200px con padding lateral de 24px. Los radios de borde siguen tres niveles: 8px para elementos pequeños (botones, inputs), 16px para tarjetas y módulos, y 24px para modales y secciones destacadas.

### 4.1.2. Web Style Guidelines

La interfaz web de NutriSmart adopta un enfoque mobile-first, utilizando un sistema de grid de 12 columnas en escritorio y 4 columnas en móvil. Se garantiza que todos los componentes escalen adecuadamente entre breakpoints, priorizando la legibilidad y la usabilidad táctil en pantallas pequeñas antes de enriquecer la experiencia en pantallas más grandes.

**Tipografía**

Se utiliza Poppins para títulos y encabezados de sección, con tamaños responsivos que emplean `clamp()` para escalar fluidamente. Questrial se aplica en párrafos, etiquetas, descripciones de funcionalidades y textos de apoyo. El interlineado base es de 1.6 para asegurar comodidad de lectura en bloques de texto extendido. La jerarquía tipográfica establece que H1 y H2 se reservan para héroes y títulos de sección respectivamente, mientras que H3 y H4 organizan subsecciones y tarjetas de contenido.

**Colores**

La selección de colores para la interfaz web refleja el sistema definido en la guía general. El verde azulado (`#508B89`) actúa como color de marca en la barra de navegación, botones primarios y elementos de énfasis. El fondo principal de las páginas utiliza blanco puro (`#FFFFFF`), mientras que secciones alternadas emplean el melocotón claro (`#FFE9DE`) para generar ritmo visual sin recurrir a sombras agresivas. Los botones de llamada a la acción combinan el melocotón medio (`#F4C5AE`) con texto en negro, garantizando contraste accesible. Los estados de error o alerta se reservan para colores rojizos que no forman parte de la paleta principal, evitando confusión con los tonos cálidos de la marca.

**Interacción y responsividad**

Los botones cuentan con transiciones de 0.3 segundos en hover y focus, proporcionando retroalimentación visual clara al usuario. La barra de navegación es fija con una altura de 68px, colapsando en un menú hamburguesa para viewports móviles. EL formulario de contacto utiliza inputs con radio de borde de 8px y etiquetas flotantes para maximizar el espacio disponible. El scroll entre secciones en la página principal utiliza `scroll-snap` para una experiencia fluida y estructurada. Todos los elementos interactivos cuentan con atributos ARIA y contraste suficiente para cumplir con criterios básicos de accesibilidad web.

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


**Desktop Landing Page**

**Main and Features**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/wireframe/landing/desktop/main.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/landing/desktop/features.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Shape** | Las tarjetas de funcionalidades usan esquinas redondeadas de manera consistente, generando una forma orgánica y amigable que contrasta con el fondo rectangular del canvas. Esto comunica suavidad y accesibilidad visual en ambas páginas. |
| **Space** | En la página de funcionalidades se utiliza un grid de 3 columnas con espaciado uniforme entre tarjetas, mientras que en la landing las secciones alternan entre layouts de 1 y 2 columnas. El espacio negativo entre secciones permite respiración visual y delimita jerárquicamente cada bloque de contenido. |
| **Direction** | En la landing, la alternancia de bloques texto-imagen (izquierda-derecha) genera un ritmo diagonal que guía al usuario hacia abajo. En la página de funcionalidades, la dirección es vertical y descendente: de tarjetas a FAQ a Footer, orientando la lectura de forma clara. |
| **Size** | Los títulos de sección son notablemente más grandes que el texto de las tarjetas, estableciendo jerarquía tipográfica que permite al usuario escanear el contenido rápidamente sin necesidad de leer cada bloque completo. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Consistencia y estándares (H4)** | El navbar con logo a la izquierda y links a la derecha se repite en ambas páginas, siguiendo la convención web estándar. El footer mantiene la misma estructura (columnas con links, redes sociales y selector de idioma) en ambas vistas, reduciendo la carga cognitiva del usuario. |
| **Diseño estético y minimalista (H8)** | Cada tarjeta de funcionalidad contiene únicamente un ícono, un título en negrita y una descripción breve. No hay elementos decorativos adicionales que compitan con la información relevante, manteniendo el foco en la función descrita. |
| **Reconocer antes que recordar (H6)** | La sección FAQ repite las mismas preguntas en ambas páginas, permitiendo que el usuario las reconozca sin necesidad de navegar hacia atrás. Las etiquetas de los planes (Basic, Pro, Premium) son visualmente diferenciadas, especialmente el plan recomendado, facilitando la comparación inmediata. |
| **Libertad y control del usuario (H3)** | El navbar persistente en la parte superior de ambas vistas actúa como salida constante, permitiendo al usuario redirigirse a cualquier sección en cualquier momento sin quedar atrapado en un flujo no deseado. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Disclosure** | Cada tarjeta de funcionalidad muestra solo el nombre y una descripción corta, sin desplegar detalles técnicos. Esto aplica el principio de mostrar suficiente información para que el usuario entienda qué encontrará si profundiza, sin saturarlo desde el primer vistazo. |
| **Choices** | La sección "Join us and transform your life" en la landing ofrece dos caminos significativos: "I want to gain muscle mass" e "I want to lose weight". Esto crea bifurcaciones con intención, orientando al usuario según su objetivo real. |
| **Front Doors** | El botón "Go to app" en el hero, el botón "Log In" en el navbar y los botones "Subscribe now!" en los planes son múltiples puertas de entrada a la conversión, asegurando que usuarios que lleguen desde distintas rutas encuentren siempre un punto de acción claro. |
| **Growth** | El grid de 3 columnas con una tarjeta solitaria en la última fila evidencia que el diseño está pensado para escalar: agregar nuevas funcionalidades no rompe la estructura, simplemente se incorporan al grid existente sin rediseñar la página. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Priorizar el contenido (P6)** | El nombre de cada funcionalidad aparece en negrita antes que la descripción, permitiendo que el usuario escanee rápidamente los títulos para decidir cuáles le interesan sin leer el texto completo. El contenido clave siempre encabeza la tarjeta. |
| **Ofrecer opciones (P5)** | El footer incluye un selector de idioma, permitiendo al usuario adaptar el idioma de la interfaz. Esto amplía el acceso a personas de distintas lenguas maternas, ofreciendo una vía alternativa de interacción. |
| **Ser consistente (P3)** | Los componentes de tarjeta siguen el mismo patrón ícono → título → descripción en todas las funcionalidades de ambas páginas. Esta consistencia estructural hace predecible la lectura y reduce la fricción para usuarios con distintos niveles de familiaridad digital. |
| **Considera la situación del usuario (P2)** | La sección FAQ al final de ambas páginas responde dudas contextuales frecuentes como alergias, viajes y sincronización de ejercicio, anticipando distintos contextos de uso y demostrando consideración por usuarios con necesidades y situaciones de vida diversas. |


**Contact, About-us & Terms**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/wireframe/landing/desktop/contact.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/landing/desktop/about-us.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/landing/desktop/terms.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Shape** | Las tarjetas de Misión y Visión en la página About Us utilizan esquinas redondeadas combinadas con íconos circulares superpuestos en la parte superior, creando una forma orgánica que transmite cercanía. En la página de Contacto, el formulario y el hero mantienen bordes rectos, generando una sensación más formal y estructurada acorde al contexto. |
| **Space** | La página de Términos y Condiciones concentra todo el contenido dentro de una sola tarjeta blanca con márgenes amplios respecto al fondo gris, usando el espacio para aislar el bloque legal y facilitar su lectura. En About Us, el espacio entre el hero, el bloque de texto y las tarjetas de Misión/Visión separa visualmente cada sección de contenido. |
| **Direction** | En About Us, la alternancia texto-imagen (izquierda-derecha) genera un flujo diagonal descendente que guía al usuario de forma natural. En la página de Contacto, el layout de dos columnas (imagen izquierda, formulario derecha) dirige la mirada horizontalmente hacia el área de acción. |
| **Size** | El título "We are NutriSmart!" en About Us ocupa un tamaño notablemente mayor al resto del texto, estableciendo jerarquía inmediata. En Términos y Condiciones, los títulos de sección numerados son más grandes que el cuerpo del texto, permitiendo escanear las secciones legales sin leer el documento completo. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Consistencia y estándares (H4)** | El navbar y el footer mantienen la misma estructura en las tres páginas (Contacto, About Us, Términos), siguiendo el patrón establecido en la landing. El selector de idioma y los íconos de redes sociales aparecen siempre en las mismas posiciones del footer. |
| **Prevención de errores (H5)** | El formulario de contacto separa los campos con etiquetas explícitas (Name, Email, Phone, Message) y campos de texto individuales, reduciendo la posibilidad de que el usuario ingrese información incorrecta o en el campo equivocado. |
| **Diseño estético y minimalista (H8)** | La página de Términos y Condiciones concentra todo el contenido legal en un único bloque blanco sin elementos decorativos adicionales. Esto evita distracciones en una página cuyo único objetivo es la lectura comprensiva de información legal. |
| **Visibilidad del estado del sistema (H1)** | El botón "Submit" en el formulario de contacto es el único elemento de acción de la página, comunicando claramente al usuario cuándo ha completado el flujo. El hero de Contacto muestra el número de teléfono de forma prominente como canal alternativo e inmediato. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Disclosure** | La página About Us muestra primero el propósito general de NutriSmart en un párrafo introductorio, y solo después profundiza en Misión y Visión como tarjetas separadas. Esto aplica el principio de revelar información progresivamente sin abrumar al usuario desde el inicio. |
| **Objects** | Las tarjetas de Misión y Visión tratan cada concepto como un objeto independiente con su propio ícono, título y descripción. Esto les otorga identidad visual propia, haciendo que cada bloque de contenido funcione como una entidad con atributos diferenciados. |
| **Focused Navigation** | El navbar define sus ítems por contenido (About Us, Features, Contact, Links) y no por su posición. Cada etiqueta comunica claramente el tipo de información que el usuario encontrará, sin depender del contexto visual para su interpretación. |
| **Front Doors** | La página de Contacto ofrece dos vías de entrada al mismo objetivo: el formulario escrito y el número de teléfono visible en el hero. Esto asume que distintos usuarios preferirán distintos canales para comunicarse con NutriSmart. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Proporciona experiencias comparables (P1)** | El formulario de contacto está estructurado con campos individuales y etiquetas explícitas, lo que permite que usuarios que navegan con teclado o lectores de pantalla puedan completar la tarea de contacto de manera equivalente a usuarios que usan mouse. |
| **Priorizar el contenido (P6)** | En Términos y Condiciones, los títulos de sección numerados (Service Description, Medical and Ethical Responsibility, etc.) destacan visualmente sobre el cuerpo del texto, ayudando al usuario a ubicarse dentro del documento y acceder directamente a la sección de su interés. |
| **Ofrecer opciones (P5)** | La página de Contacto ofrece múltiples canales de comunicación: formulario escrito y número telefónico. Esto contempla distintos perfiles de usuario, desde quienes prefieren comunicación asíncrona hasta quienes necesitan respuesta inmediata. |
| **Ser consistente (P3)** | La estructura de las tarjetas de Misión y Visión replica el mismo patrón visual: ícono circular en la parte superior, título en negrita y descripción en cuerpo de texto. Esta consistencia hace que el usuario entienda el patrón de lectura sin necesidad de aprenderlo nuevamente. |

**Mobile Web Browser**

**Main & Features**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/wireframe/landing/mobile/main.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/landing/mobile/features.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/landing/mobile/main-menu.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Shape** | El navbar móvil abandona el menú horizontal y adopta un ícono de hamburguesa (≡) que despliega un panel lateral con esquinas rectas y fondo oscuro. Las tarjetas de funcionalidades mantienen esquinas redondeadas consistentes con la versión desktop, preservando la identidad visual entre plataformas. |
| **Space** | Al pasar a mobile, el layout de 3 columnas del desktop se convierte en una sola columna vertical con tarjetas apiladas. Esto maximiza el uso del ancho reducido de pantalla y evita que el contenido se comprima o resulte ilegible. |
| **Direction** | En la landing mobile, los bloques de contenido siguen una dirección estrictamente vertical y descendente, alternando imagen y texto en filas independientes. Esto se adapta al patrón de scroll natural del usuario móvil, que consume contenido de arriba hacia abajo. |
| **Size** | El título "Smart Nutrition" ocupa casi el ancho completo de la pantalla en dos líneas, estableciendo una jerarquía visual inmediata y dominante. Los botones de acción como "Go to app" tienen un tamaño generoso para facilitar el toque con el dedo, siguiendo las recomendaciones de área mínima táctil. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Consistencia y estándares (H4)** | El menú hamburguesa con panel deslizante es el patrón estándar de navegación móvil. Su uso sigue la convención esperada por el usuario, reduciendo la curva de aprendizaje. Los ítems del menú (About Us, Features, Contact, Links, Log in) son los mismos que en desktop. |
| **Libertad y control del usuario (H3)** | El panel de navegación desplegable incluye un botón "✕" en la esquina superior derecha para cerrarlo, ofreciendo al usuario una salida clara sin necesidad de navegar a otra página o usar el botón físico del dispositivo. |
| **Reconocer antes que recordar (H6)** | Cada tarjeta de funcionalidad en mobile combina ícono placeholder y título en negrita en la misma fila, permitiendo que el usuario identifique visualmente la función sin necesidad de leer la descripción completa. El patrón ícono-título se repite de forma predecible en todas las tarjetas. |
| **Diseño estético y minimalista (H8)** | La versión mobile elimina elementos secundarios presentes en desktop, como subtítulos adicionales y columnas paralelas, conservando únicamente el contenido esencial: ícono, título y descripción breve. Esto respeta las limitaciones de espacio sin sacrificar la comprensión del contenido. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Focused Navigation** | El menú hamburguesa agrupa todos los ítems de navegación en un panel dedicado, definido por su contenido y no por su posición visual. El usuario accede a la navegación como una acción explícita, manteniendo el foco en el contenido de la página mientras no la necesita. |
| **Disclosure** | En la landing mobile, cada sección principal (Smart Scan, Global Nutrition, Your weather your diet) muestra solo el título y una descripción corta antes de la sección de conversión. No se despliegan detalles técnicos hasta que el usuario decide explorar más. |
| **Choices** | La sección "Join us and transform your life" presenta dos opciones de objetivo ("I want to gain muscle mass" e "I want to lose weight") como botones apilados verticalmente, adaptando la bifurcación de decisión al formato de una sola columna sin perder su función de segmentación. |
| **Growth** | El layout de tarjetas apiladas en la página de funcionalidades permite agregar nuevas funcionalidades simplemente añadiendo tarjetas al final de la lista, sin necesidad de rediseñar la estructura. La columna única escala de forma natural con contenido adicional. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Considera la situación del usuario (P2)** | El diseño mobile asume que el usuario puede estar en movimiento, con una sola mano disponible. El botón "Go to app" y los botones de objetivo ("I want to gain muscle mass") están dimensionados para ser accionables con el pulgar sin requerir precisión. |
| **Proporciona experiencias comparables (P1)** | El contenido disponible en desktop (funcionalidades, planes, FAQ, footer con idiomas) está completamente presente en la versión mobile, reorganizado en una sola columna. El usuario móvil accede a la misma información sin versiones reducidas o simplificadas. |
| **Priorizar el contenido (P6)** | En mobile, el hero coloca el título "Smart Nutrition" y el botón "Go to app" en la parte superior visible sin necesidad de scroll, priorizando el mensaje principal y la acción de conversión antes que cualquier otro contenido. |
| **Ser consistente (P3)** | El patrón de tarjeta en la página de funcionalidades mobile (ícono a la izquierda, título a la derecha, descripción abajo) se repite de forma idéntica en todas las entradas, estableciendo un modelo de lectura predecible que el usuario solo necesita aprender una vez. |

**Contact, About-us & Terms**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/wireframe/landing/mobile/contact.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/landing/mobile/about-us.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/landing/mobile/terms.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Shape** | Las tarjetas de Misión y Visión en About Us mantienen las esquinas redondeadas y el ícono circular superpuesto en la parte superior, adaptando fielmente la forma orgánica de la versión desktop al formato de una sola columna. El formulario de contacto conserva bordes rectos en los campos de texto, transmitiendo formalidad y estructura. |
| **Space** | En Términos y Condiciones, el contenido legal ocupa casi todo el ancho de la pantalla con márgenes mínimos, priorizando la legibilidad del texto extenso en pantalla pequeña. En About Us, se preserva espacio vertical generoso entre el bloque introductorio y las tarjetas de Misión/Visión para separar visualmente las secciones. |
| **Direction** | En About Us, las tarjetas de Misión y Visión se apilan verticalmente una debajo de la otra, adaptando el layout de dos columnas del desktop a una dirección de lectura descendente natural para el usuario móvil. En Contacto, el formulario ocupa toda la columna sin elementos paralelos, dirigiendo la atención exclusivamente al llenado de campos. |
| **Size** | En Términos y Condiciones, los títulos de sección numerados son visualmente más grandes que el cuerpo del texto, permitiendo que el usuario escanee rápidamente las secciones legales sin necesidad de leer el documento completo en una pantalla reducida. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Consistencia y estándares (H4)** | El navbar hamburguesa y el footer de dos columnas se repiten de forma idéntica en las tres páginas móviles (Contacto, About Us, Términos), manteniendo la coherencia estructural establecida en la landing mobile y reduciendo la desorientación del usuario al navegar entre vistas. |
| **Prevención de errores (H5)** | El formulario de contacto en mobile presenta los campos apilados verticalmente con etiquetas explícitas encima de cada input, eliminando ambigüedad sobre qué información ingresar en cada campo. El campo de mensaje tiene una altura generosa que reduce el riesgo de enviar mensajes incompletos. |
| **Diseño estético y minimalista (H8)** | La página de Términos y Condiciones en mobile elimina cualquier elemento decorativo adicional, presentando únicamente el bloque de texto legal sobre fondo blanco. Esto respeta el principio de no añadir información que compita con el contenido relevante en una pantalla de espacio reducido. |
| **Visibilidad del estado del sistema (H1)** | El hero de la página de Contacto muestra el número de teléfono de forma visible e inmediata sobre la imagen de fondo, comunicando al usuario desde el primer momento que existe un canal de contacto directo antes de que llegue al formulario. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Disclosure** | En About Us mobile, el párrafo introductorio aparece primero como contexto general, y solo después se revelan las tarjetas de Misión y Visión como profundización. Esto aplica el principio de mostrar información suficiente para orientar al usuario antes de presentar el detalle. |
| **Objects** | Las tarjetas de Misión y Visión en mobile tratan cada concepto como un objeto independiente con ícono, título y descripción propios, preservando su identidad visual incluso al reorganizarse en columna única. Cada tarjeta funciona como una entidad autónoma con atributos diferenciados. |
| **Front Doors** | La página de Contacto ofrece dos puntos de entrada al mismo objetivo: el número telefónico visible en el hero y el formulario escrito debajo. Esto garantiza que usuarios que lleguen directamente a esta página desde cualquier canal encuentren siempre una vía de acción inmediata. |
| **Focused Navigation** | El panel hamburguesa agrupa los ítems de navegación (Features, Contact, Terms and Conditions, About Us) definidos por su contenido y no por su posición en pantalla. El usuario accede a la navegación como una acción deliberada, manteniendo el foco en el contenido mientras no la necesita. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Proporciona experiencias comparables (P1)** | Los campos del formulario de contacto en mobile están dimensionados con altura suficiente para ser accionables con el dedo, ofreciendo una experiencia de llenado equivalente a la versión desktop sin requerir precisión de cursor. |
| **Priorizar el contenido (P6)** | En About Us mobile, el título "We are NutriSmart!" ocupa la parte superior visible de la pantalla sin necesidad de scroll, priorizando el mensaje de identidad de marca antes que cualquier otro contenido. Las tarjetas de Misión y Visión destacan sus títulos en negrita sobre fondo oscuro para facilitar el escaneo. |
| **Ser consistente (P3)** | El footer mantiene la misma estructura de dos columnas en las tres páginas móviles, con los mismos enlaces (Features, Contact, Terms and Conditions, About Us) y el selector de idioma en la misma posición. Esta consistencia permite al usuario ubicar recursos secundarios sin esfuerzo cognitivo adicional. |
| **Considera la situación del usuario (P2)** | La página de Términos y Condiciones en mobile adapta el texto legal a columna única con interlineado generoso, reconociendo que el usuario puede estar leyendo en condiciones de movilidad o con pantalla de tamaño reducido, donde la densidad de texto dificulta la lectura. |

### 4.3.2. Landing Page Mock-up

**Desktop Web Browser**

**Main & Features**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/mockup/landing/desktop/main.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/landing/desktop/features.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Colour** | Se aplica una paleta de tonos cálidos con fondo salmón/rosado como color dominante en ambas páginas, complementado con un verde oscuro en el navbar y footer. Esta combinación transmite salud, calidez y naturalidad, alineada con el propósito nutricional de la plataforma. Las tarjetas de funcionalidades usan fondo blanco para generar contraste sobre el fondo salmón y destacar el contenido. |
| **Texture** | En la landing, las secciones de Smart Scan, Global Nutrition y Your Weather usan imágenes fotográficas reales de alimentos y dispositivos móviles como fondo, introduciendo textura orgánica que contrasta con las secciones de fondo plano. Esto genera profundidad visual y contextualiza cada funcionalidad con evidencia visual real. |
| **Shape** | Los íconos de cada funcionalidad son ilustraciones de línea fina con estilo outline consistente, reemplazando los placeholders del wireframe. Las tarjetas mantienen esquinas redondeadas. Los botones de objetivo ("I want to gain muscle mass") adoptan formas redondeadas con fondo gris oscuro que los distingue como elementos interactivos. |
| **Colour (contraste)** | El plan Premium incluye un fondo verde oscuro que lo diferencia visualmente de los planes Basic y Pro en fondo blanco, reforzando su etiqueta "Recommended" y dirigiendo la atención del usuario hacia la opción de mayor valor sin necesidad de texto adicional. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Consistencia y estándares (H4)** | El navbar verde oscuro con logo a la izquierda y links a la derecha se mantiene idéntico en ambas páginas. El footer replica la misma estructura de columnas con enlaces, redes sociales reales (Gmail, Facebook, Instagram, LinkedIn) y selector de idioma, estableciendo un patrón reconocible en toda la plataforma. |
| **Reconocer antes que recordar (H6)** | Los íconos outline de cada funcionalidad son metáforas visuales directas de su función: una cámara para Smart Scan, un avión para Travel Mode, un tenedor y plato para Meal Logging. El usuario reconoce la funcionalidad por el ícono antes de leer el título, reduciendo la carga cognitiva. |
| **Relación entre el sistema y el mundo real (H2)** | Las imágenes fotográficas reales de alimentos frescos, dispositivos móviles con la app activa y fondos con salpicaduras de color conectan el sistema con el mundo real del usuario. Esto hace que la plataforma se perciba como una herramienta tangible y no como un producto abstracto. |
| **Diseño estético y minimalista (H8)** | La sección de funcionalidades en la landing muestra solo 6 tarjetas con ícono, nombre y descripción breve, redirigiendo al usuario a la página de funcionalidades para ver el listado completo. Esto evita saturar la landing con información que compite con el llamado a la acción principal. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Exemplars** | Las secciones de Smart Scan, Global Nutrition y Your Weather usan imágenes reales de la app en uso sobre dispositivos móviles como ejemplos concretos de cada funcionalidad. Esto aplica el principio de mostrar ejemplares que ilustren el contenido de cada categoría antes de que el usuario profundice. |
| **Choices** | La sección "Join us and transform your life" presenta dos opciones de objetivo con íconos ilustrativos (figura muscular vs. figura delgada), haciendo que la elección sea visualmente significativa y no solo textual, facilitando la toma de decisión del usuario. |
| **Disclosure** | La landing muestra una vista previa de 6 funcionalidades en la sección "Features to enjoy" sin detallar todas las capacidades de cada una. El usuario que quiera profundizar puede navegar a la página de funcionalidades, donde encuentra las 10 tarjetas completas con descripciones detalladas. |
| **Objects** | El logo de NutriSmart en navbar y footer incorpora un ícono de hoja y el tagline "Smart Nutrition Platform", tratando la marca como un objeto vivo con identidad visual propia. Esto refuerza la coherencia entre todas las páginas y hace que la marca sea reconocible como entidad independiente. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Agrega valor (P7)** | Los íconos outline temáticos reemplazan los placeholders genéricos del wireframe, agregando valor semántico real a cada tarjeta. Un ícono de cámara para Smart Scan o un avión para Travel Mode comunica la función de forma inmediata, mejorando la experiencia de usuarios con distintos niveles de alfabetización digital. |
| **Priorizar el contenido (P6)** | El plan Premium se distingue visualmente con fondo verde oscuro y la etiqueta "Recommended" destacada, priorizando la opción más completa sin ocultar las alternativas. El usuario puede comparar los tres planes de forma simultánea sin necesidad de navegar entre páginas. |
| **Ofrecer opciones (P5)** | El footer incluye íconos de redes sociales reales (Gmail, Facebook, Instagram, LinkedIn) como canales alternativos de contacto e información. El selector de idioma permite cambiar el idioma de la interfaz, ampliando el acceso a usuarios hispanohablantes y angloparlantes. |
| **Proporciona experiencias comparables (P1)** | Los íconos outline de línea fina tienen un estilo visual consistente y reconocible que funciona correctamente en distintas resoluciones de pantalla. Esto garantiza que la experiencia de reconocimiento visual de funcionalidades sea equivalente para usuarios en monitores de alta y baja densidad de píxeles. |

**Contact, About-us & Terms**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/mockup/landing/desktop/contact.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/landing/desktop/about-us.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/landing/desktop/terms.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Colour** | La paleta salmón/rosado como fondo dominante se extiende consistentemente en las tres páginas, unificando la identidad visual de toda la plataforma. En Contacto, los bordes de los campos del formulario usan un tono rosado que los diferencia sutilmente del fondo blanco. El botón "Submit" adopta el mismo tono salmón, integrándolo como elemento de acción dentro de la paleta general. |
| **Texture** | En About Us, el hero incorpora manchas de acuarela en tonos rosado y verde azulado como elementos decorativos de fondo, introduciendo una textura orgánica y artesanal que humaniza la marca. En Contacto, la fotografía de una mano sosteniendo un teléfono retro sobre fondo azul verdoso aporta textura fotográfica real que contrasta con el fondo blanco del formulario. |
| **Shape** | Las tarjetas de Misión y Visión en About Us usan esquinas redondeadas con fondo verde oscuro y un ícono circular superpuesto en la parte superior, con ilustraciones outline temáticas: una diana para Misión y un foco para Visión. Esto reemplaza los placeholders del wireframe con formas con significado semántico directo. En Contacto, el bloque "Contact Us" en el hero adopta forma rectangular con fondo rosado pastel, destacándolo sobre la fotografía de personas. |
| **Colour (contraste tipográfico)** | En Términos y Condiciones, el título de la página y los títulos de sección numerados son negros sobre fondo salmón y blanco respectivamente, generando contraste suficiente para la lectura de texto legal extenso. El texto dentro de la tarjeta blanca usa negro sobre blanco, la combinación de mayor legibilidad disponible. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Consistencia y estándares (H4)** | El navbar verde oscuro con logo NutriSmart a la izquierda y links a la derecha se replica de forma idéntica en las tres páginas. El footer mantiene la misma estructura de cuatro columnas con logo, enlaces, redes sociales con íconos de color real y selector de idioma, estableciendo un patrón reconocible en toda la plataforma. |
| **Relación entre el sistema y el mundo real (H2)** | La fotografía del hero en Contacto muestra un grupo de personas diversas sonrientes, comunicando cercanía y accesibilidad humana antes de llegar al formulario. La imagen de la mano con teléfono retro refuerza la metáfora de comunicación de forma visual e inmediata, sin necesidad de texto explicativo. |
| **Prevención de errores (H5)** | Los campos del formulario de contacto tienen bordes rosados visibles que los delimitan claramente, reduciendo el riesgo de que el usuario interactúe con el área incorrecta. Las etiquetas (Name, Email, Phone, Message) están posicionadas fuera de los campos, evitando que desaparezcan al comenzar a escribir. |
| **Diseño estético y minimalista (H8)** | La página de Términos y Condiciones concentra todo el contenido legal en una sola tarjeta blanca sobre fondo salmón, sin imágenes decorativas ni elementos visuales adicionales. La decisión de eliminar todo ornamento en esta página respeta el principio de no añadir elementos que compitan con la lectura comprensiva de información legal. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Objects** | El logo de NutriSmart en navbar y footer es ahora un objeto visual completo: ilustración de manos sosteniendo una hoja, nombre de marca y tagline "Smart Nutrition Platform". Este objeto se comporta de forma consistente en todas las páginas como elemento de identidad vivo, no como un simple placeholder. |
| **Exemplars** | En About Us, el ícono circular que acompaña el bloque introductorio muestra la ilustración del logo de NutriSmart a color, funcionando como un ejemplar visual de la identidad de marca antes de que el usuario llegue a las tarjetas de Misión y Visión. |
| **Disclosure** | La página de Términos y Condiciones organiza el contenido en cinco secciones numeradas y claramente tituladas (Service Description, Medical and Ethical Responsibility, Plans and Billing, Privacy and Technology, Limitations), permitiendo al usuario identificar rápidamente la sección de su interés sin leer el documento completo. |
| **Front Doors** | En Contacto, el número de teléfono real (+51 984231995) aparece en el hero de forma prominente junto al ícono de llamada, actuando como puerta de entrada directa para usuarios que prefieren contacto inmediato sobre el formulario escrito. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Agrega valor (P7)** | Las manchas de acuarela en el hero de About Us agregan valor estético que humaniza la página institucional, diferenciándola de un bloque de texto corporativo genérico. Los íconos temáticos de diana (Misión) y foco (Visión) agregan valor semántico que refuerza el significado de cada concepto más allá del título. |
| **Proporciona experiencias comparables (P1)** | Los íconos de redes sociales en el footer usan sus colores de marca oficiales (rojo para Gmail, azul para Facebook, gradiente para Instagram, azul para LinkedIn), permitiendo que usuarios con distintos niveles de familiaridad digital identifiquen los canales por color y forma sin depender únicamente del texto. |
| **Priorizar el contenido (P6)** | En About Us, las tarjetas de Misión y Visión usan fondo verde oscuro con texto blanco, destacándolas visualmente sobre el fondo blanco de la página. Esto prioriza el contenido institucional más relevante de la página mediante contraste cromático deliberado. |
| **Considera la situación del usuario (P2)** | La fotografía del hero en Contacto muestra personas de distintas etnias y géneros, reconociendo que NutriSmart es una plataforma dirigida a una audiencia diversa. Esta decisión visual comunica inclusión desde el primer elemento visible de la página de contacto. |

**Mobile Web Browser**

**Main & Features**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/mockup/landing/mobile/main.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/landing/mobile/features.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/landing/mobile/main-menu.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Colour** | La paleta salmón/rosado como fondo dominante y el verde oscuro del navbar se mantienen consistentes con la versión desktop, garantizando coherencia de identidad visual entre plataformas. El panel de navegación hamburguesa adopta el mismo verde oscuro del navbar, y los círculos decorativos del fondo del panel combinan el rosado y el blanco de la paleta general. |
| **Texture** | El hero de la landing mobile incorpora una fotografía de alimentos frescos como banda superior y manchas de acuarela en verde azulado como elementos decorativos alrededor de las imágenes de producto. Esta textura orgánica se adapta al ancho reducido de pantalla sin perder la riqueza visual presente en la versión desktop. |
| **Shape** | Las tarjetas de funcionalidades en la página de features adoptan el mismo patrón ícono-título-descripción con esquinas redondeadas, pero en layout de columna única que ocupa el ancho completo de la pantalla. El botón "Go to app" usa forma de píldora con fondo rosado pastel, diferenciándolo del texto circundante como elemento de acción primaria. |
| **Size** | El título "Smart Nutrition" ocupa casi el ancho completo de la pantalla en dos líneas con una jerarquía tipográfica dominante. Los íconos outline en las tarjetas de funcionalidades tienen un tamaño generoso respecto al ancho de la tarjeta, haciéndolos reconocibles en pantallas de densidad variable sin necesidad de ampliar. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Consistencia y estándares (H4)** | El menú hamburguesa despliega un panel con el mismo conjunto de ítems de navegación (About Us, Features, Contact, Links, Log in) que la versión desktop, manteniendo consistencia en el contenido accesible independientemente del dispositivo. El botón "✕" para cerrar el panel sigue la convención estándar de cierre en interfaces móviles. |
| **Relación entre el sistema y el mundo real (H2)** | Las imágenes de la app activa sobre dispositivos móviles reales en las secciones Smart Scan y Global Nutrition muestran el producto en su contexto de uso natural. Las manchas de acuarela y fotografías de alimentos conectan la plataforma con el mundo real de la nutrición cotidiana del usuario. |
| **Reconocer antes que recordar (H6)** | Los íconos outline temáticos en las tarjetas de funcionalidades mobile (cámara para Smart Scan, avión para Travel Mode, gorro de chef para Recipe Suggestions) permiten al usuario identificar la función visualmente antes de leer el título, reduciendo la carga de memoria en una interfaz de consumo vertical y rápido. |
| **Diseño estético y minimalista (H8)** | La versión mobile de la página de funcionalidades presenta las tarjetas en columna única con solo ícono, título en negrita y una línea de descripción, eliminando cualquier elemento visual que no aporte información funcional directa. El fondo salmón liso entre tarjetas actúa como separador neutro sin añadir ruido visual. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Disclosure** | En la landing mobile, cada sección de funcionalidad principal (Smart Scan, Global Nutrition) muestra la imagen del producto en contexto y una descripción breve antes de invitar al usuario a profundizar. La información se revela progresivamente a medida que el usuario hace scroll, sin sobrecargar la pantalla inicial. |
| **Objects** | Las imágenes de la app activa sobre smartphones tratan el producto como un objeto vivo con comportamientos propios: el teléfono muestra la interfaz de Smart Scan en uso real, comunicando que la app es un objeto funcional y no una representación abstracta. |
| **Focused Navigation** | El panel hamburguesa agrupa la navegación como una acción deliberada del usuario, manteniendo los ítems definidos por su contenido. Los indicadores de carrusel (puntos) debajo de la banda de imagen del hero comunican que existe contenido navegable horizontalmente, orientando al usuario sobre las posibilidades de exploración disponibles. |
| **Growth** | El layout de tarjetas apiladas en la página de funcionalidades mobile permite incorporar nuevas funcionalidades simplemente añadiendo tarjetas al final de la lista sin rediseñar la estructura, escalando de forma natural con el crecimiento del producto. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Considera la situación del usuario (P2)** | El botón "Go to app" tiene forma de píldora con área táctil generosa, diseñado para ser accionable con el pulgar en una sola mano. Las tarjetas de funcionalidades tienen altura suficiente para evitar toques accidentales en elementos adyacentes, reconociendo que el usuario móvil interactúa con el dedo en condiciones de movimiento. |
| **Proporciona experiencias comparables (P1)** | La versión mobile presenta el mismo contenido disponible en desktop (funcionalidades, secciones de producto, navegación completa), reorganizado en columna única. El usuario móvil accede a información equivalente sin versiones reducidas, garantizando paridad de experiencia entre dispositivos. |
| **Priorizar el contenido (P6)** | El título "Smart Nutrition" y el botón "Go to app" ocupan la parte superior visible de la pantalla sin necesidad de scroll, priorizando el mensaje principal y la acción de conversión. En la página de funcionalidades, cada tarjeta posiciona el título en negrita antes que la descripción, facilitando el escaneo rápido del contenido. |
| **Ser consistente (P3)** | El patrón de tarjeta en la página de funcionalidades mobile replica exactamente la misma estructura que la versión desktop (ícono a la izquierda, título a la derecha, descripción abajo), estableciendo un modelo de lectura familiar para usuarios que hayan interactuado previamente con la versión de escritorio. |

**Contact, About-us & Terms**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/mockup/landing/mobile/contact.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/landing/mobile/about-us.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/landing/mobile/terms.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Colour** | Los bordes rosados de los campos del formulario en Contacto y el botón "Submit" en el mismo tono salmón mantienen la paleta cromática de la plataforma incluso en los elementos interactivos más funcionales. En About Us, las manchas de acuarela rosada y verde azulado sobre el fondo blanco del hero replican el lenguaje visual decorativo de la versión desktop adaptado al ancho móvil. |
| **Texture** | En Contacto, la fotografía del hero muestra un grupo de personas diversas y sonrientes ocupando el ancho completo de la pantalla, introduciendo textura fotográfica humana que contextualiza la página antes del formulario. En About Us, las manchas de acuarela aportan textura orgánica al encabezado, diferenciando visualmente la página institucional de las demás. |
| **Shape** | Las tarjetas de Misión y Visión en About Us mobile conservan las esquinas redondeadas con fondo verde oscuro y el ícono circular superpuesto en la parte superior, manteniendo la forma orgánica de la versión desktop en columna única. El logo de NutriSmart en el footer combina una forma circular ilustrada con texto, funcionando como un objeto visual compacto adaptado al espacio reducido. |
| **Size** | En Términos y Condiciones, el título "Terms and conditions" ocupa las dos primeras líneas visibles con un tamaño notablemente mayor al cuerpo del texto, estableciendo jerarquía inmediata en una página de contenido denso. Los íconos de redes sociales en el footer tienen un tamaño táctil generoso que los hace accionables sin requerir precisión. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Consistencia y estándares (H4)** | El navbar con logo y hamburguesa, y el footer con estructura de dos columnas, íconos de redes sociales a color y selector de idioma se replican de forma idéntica en las tres páginas móviles, manteniendo el patrón establecido en la landing mobile y generando predictibilidad en la navegación. |
| **Prevención de errores (H5)** | Los campos del formulario de Contacto tienen bordes rosados claramente visibles sobre fondo blanco, delimitando el área de interacción y reduciendo el riesgo de que el usuario toque fuera del campo. El campo de mensaje tiene altura generosa para evitar que el usuario envíe mensajes incompletos por falta de espacio visual. |
| **Visibilidad del estado del sistema (H1)** | El número de teléfono real (+51 984231995) aparece superpuesto sobre la fotografía del hero en Contacto junto al ícono de llamada, comunicando de forma inmediata que existe un canal de contacto directo disponible antes de que el usuario llegue al formulario. |
| **Diseño estético y minimalista (H8)** | La página de Términos y Condiciones en mobile presenta el contenido legal en una sola tarjeta blanca sin imágenes, íconos ni elementos decorativos adicionales. Esta decisión respeta el principio de eliminar todo lo que no contribuya directamente a la comprensión del contenido legal en pantalla reducida. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Objects** | El logo de NutriSmart en navbar y footer de las tres páginas mobile es un objeto visual completo con ilustración, nombre de marca y tagline, comportándose de forma consistente como elemento de identidad en todas las vistas. Las tarjetas de Misión y Visión tratan cada concepto como un objeto independiente con ícono, título y descripción propios. |
| **Disclosure** | En About Us mobile, el párrafo introductorio aparece antes de las tarjetas de Misión y Visión, revelando el propósito general de la empresa antes de profundizar en sus valores institucionales. En Términos y Condiciones, los títulos de sección numerados permiten al usuario anticipar la estructura del documento sin leerlo completo. |
| **Front Doors** | La página de Contacto mobile ofrece dos puertas de entrada al mismo objetivo: el número telefónico visible en el hero y el formulario escrito debajo. Esto garantiza que usuarios que lleguen directamente a esta página desde cualquier canal encuentren siempre una vía de acción inmediata adecuada a su preferencia. |
| **Focused Navigation** | El footer en las tres páginas mobile presenta los mismos enlaces de navegación (Features, Contact, Terms and Conditions, About Us) definidos por su contenido, permitiendo al usuario reorientarse dentro de la plataforma desde cualquier página sin necesidad de volver al inicio. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Considera la situación del usuario (P2)** | Los campos del formulario de Contacto tienen altura suficiente para ser accionables con el dedo en condiciones de movilidad, y el botón "Submit" está posicionado debajo del último campo con espacio de separación que evita envíos accidentales al terminar de escribir el mensaje. |
| **Proporciona experiencias comparables (P1)** | Los íconos de redes sociales en el footer usan sus colores de marca oficiales (rojo Gmail, azul Facebook, gradiente Instagram, azul LinkedIn), permitiendo que usuarios con distintos niveles de alfabetización digital identifiquen los canales por color y forma sin depender únicamente del texto en pantalla reducida. |
| **Priorizar el contenido (P6)** | En About Us mobile, las tarjetas de Misión y Visión con fondo verde oscuro y texto blanco destacan visualmente sobre el fondo salmón de la página, priorizando el contenido institucional más relevante mediante contraste cromático deliberado incluso en formato de columna única. |
| **Ser consistente (P3)** | La estructura del footer se replica de forma idéntica en las tres páginas mobile con los mismos bloques (logo + enlaces + redes sociales + selector de idioma), estableciendo un patrón reconocible que permite al usuario ubicar recursos secundarios sin esfuerzo cognitivo adicional independientemente de la página en que se encuentre. |

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes

**Login, Dashboard, Analytics, Daily log & Balance progress**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/wireframe/webapp/login.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/webapp/dashboard.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/webapp/analytics.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
    <tr>
      <td><img src="../assets/img/wireframe/webapp/dailylog.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/webapp/balanceprogress.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Shape** | La barra lateral de navegación usa un layout rectangular fijo con ítems de texto e ícono alineados verticalmente. Las tarjetas de métricas (calorías, IMC, BMR, TDEE) son rectangulares con esquinas redondeadas y jerarquía numérica prominente. El ítem activo del menú lateral se resalta con un fondo diferenciado que indica la sección actual. En Login, los campos de entrada usan forma de píldora con bordes redondeados, diferenciándolos visualmente de los campos rectangulares del wireframe de la landing. |
| **Space** | El layout de la aplicación divide la pantalla en dos zonas fijas: sidebar izquierdo de navegación y área de contenido principal. Dentro del área de contenido, las tarjetas de métricas se distribuyen en una fila horizontal superior, seguidas de bloques de contenido secundario en grid de dos columnas. Este uso del espacio establece una jerarquía clara entre datos primarios y secundarios. |
| **Direction** | En Dashboard y Analytics, la lectura sigue un patrón en Z: de izquierda a derecha en la fila de métricas superiores, luego diagonal hacia el bloque principal de contenido y finalmente al panel lateral derecho. En Daily Log, la dirección es vertical descendente dentro de cada bloque de comidas, con el panel de búsqueda fijo a la derecha. |
| **Size** | Los valores numéricos clave (1340 kcal, 70.2 kg, 24.1 IMC) se muestran en un tamaño notablemente mayor al de sus etiquetas y unidades de medida, estableciendo una jerarquía tipográfica que permite al usuario escanear los datos más relevantes sin leer el contexto completo. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Visibilidad del estado del sistema (H1)** | El Dashboard saluda al usuario por nombre ("Good morning, Ana") con fecha actual, comunicando que el sistema está activo y contextualizado en tiempo real. Las barras de progreso en Daily Log muestran el porcentaje de cada macronutriente consumido respecto a la meta diaria. En Body Progress, la fecha de logro estimada ("~August 14, 2026") informa al usuario sobre su proyección actual. |
| **Reconocer antes que recordar (H6)** | El menú lateral muestra todos los ítems de navegación visibles de forma permanente, divididos en secciones PRINCIPAL y TOOLS. El ítem activo está resaltado, eliminando la necesidad de que el usuario recuerde en qué sección se encuentra. En Daily Log, cada comida muestra nombre, cantidad, calorías y macros en la misma fila, evitando que el usuario deba navegar para recordar qué registró. |
| **Flexibilidad y eficiencia en el uso (H7)** | En Body Progress, los filtros de tiempo "7 days", "30 days" y "90 days" permiten al usuario experto cambiar el rango del gráfico con un solo clic sin necesidad de configurar fechas manualmente. En Analytics, el botón "Export to PDF" y los mismos filtros de rango ofrecen atajos directos para usuarios avanzados. |
| **Prevención de errores (H5)** | En Body Progress, el campo "Log weight" muestra el peso actual como placeholder ("E.g.: 70.2") y lo confirma debajo del campo ("Current weight: 70.2 kg"), permitiendo al usuario verificar el valor antes de guardar. El campo "Update height" incluye la nota "BMI is automatically recalculated", informando las consecuencias de la acción antes de ejecutarla. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Objects** | Cada entrada del Daily Log trata la comida como un objeto con atributos propios: nombre, cantidad, calorías y macros (P, C, G). Cada registro del Log History en Body Progress tiene fecha, peso y variación como atributos independientes. Estos objetos se comportan como entidades vivas que acumulan historial y generan proyecciones. |
| **Multiple Classification** | La navegación lateral organiza el contenido en dos categorías diferenciadas: PRINCIPAL (Dashboard, Daily log, Smart Scan, Recommendations, Body progress) y TOOLS (Pantry, Wearable, Analytics, Subscription). Esta clasificación permite al usuario acceder al contenido tanto por flujo de uso habitual como por tipo de herramienta. |
| **Choices** | En Analytics, los filtros "7 days", "30 days" y "90 days" ofrecen tres perspectivas temporales significativas del progreso del usuario. En Login, el enlace "Forgot your password?" y "Create account" ofrecen rutas alternativas sin obligar al usuario a abandonar el flujo principal. |
| **Growth** | La estructura de Daily Log organiza las comidas por categoría (Breakfast, Lunch, Snack, Dinner) con entradas expandibles dentro de cada bloque. Esto permite que el número de alimentos registrados por comida crezca sin romper la jerarquía visual, añadiendo filas dentro del bloque correspondiente. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Priorizar el contenido (P6)** | En Dashboard, las tres tarjetas superiores (Calories Consumed, Calories Remaining, Net Balance) presentan los datos más relevantes para el seguimiento diario del usuario en la parte más visible de la pantalla, antes que cualquier otro contenido. Los valores numéricos en tamaño grande priorizan el dato sobre su contexto. |
| **Proporciona experiencias comparables (P1)** | El panel de búsqueda de alimentos en Daily Log incluye un campo de texto con placeholder descriptivo ("E.g.: rice, chicken breast, yogurt...") que orienta al usuario sobre el tipo de entrada esperada, ofreciendo una experiencia de búsqueda accesible tanto para usuarios que conocen los nombres exactos como para quienes buscan por categoría general. |
| **Deja al usuario mandar (P4)** | En Body Progress, el usuario puede editar su meta de peso y actualizar su altura en cualquier momento desde el panel lateral. En Analytics, el botón "Export to PDF" da al usuario control sobre sus propios datos, permitiéndole exportarlos cuando lo considere necesario. |
| **Agrega valor (P7)** | El bloque "Active Streak" en Dashboard muestra el número de días consecutivos con registro completo, agregando valor motivacional más allá del simple registro de datos. La integración con Google Fit que descuenta calorías activas del balance diario ("Active (Google Fit): -300 kcal") agrega valor contextual que una app de nutrición estándar no ofrece. |

**Recommendations, SmartScan, Suscription & Pantry**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/wireframe/webapp/recommendations.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/webapp/smartscan.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/wireframe/webapp/suscription.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
    <tr>
      <td><img src="../assets/img/wireframe/webapp/pantry.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Shape** | En Smart Scan, las zonas de carga de imagen usan bordes punteados para indicar áreas de arrastrar y soltar, diferenciándose visualmente de los bordes sólidos de las tarjetas de contenido. En Recommendations, las etiquetas de atributos (320 kcal, P 32g, Light) usan forma de píldora redondeada para distinguirse del texto corrido. En Subscription, los indicadores de características de cada plan usan círculos rellenos como bullets, estableciendo una lista visual reconocible. |
| **Space** | En Recommendations, el panel lateral derecho con "Active filters" y "Daily balance" ocupa aproximadamente un tercio del ancho de la pantalla, dejando dos tercios para las tarjetas de recomendaciones. Este balance espacial prioriza el contenido principal sin eliminar el contexto secundario relevante. En Pantry, el layout de dos columnas separa la gestión de ingredientes de las recetas sugeridas, organizando el flujo de causa-efecto de izquierda a derecha. |
| **Direction** | En Recommendations, la lectura sigue una dirección horizontal de izquierda a derecha dentro de cada tarjeta de plato: imagen → nombre → descripción → etiquetas → botón de acción. Esta dirección guía al usuario hacia el punto de conversión ("+Add to log") de forma natural. En Subscription, las tres tarjetas de plan se alinean horizontalmente permitiendo comparación visual simultánea. |
| **Size** | En Subscription, el precio de cada plan ($9.99, $14.99, $19.99) se muestra en un tamaño notablemente mayor al del nombre del plan y la descripción, facilitando la comparación económica inmediata sin necesidad de leer el contenido completo de cada tarjeta. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Visibilidad del estado del sistema (H1)** | En Recommendations, el banner superior indica el contexto actual de forma explícita: ciudad, temperatura, condición climática y hace cuánto se actualizó ("Updated 5 mins ago"). En Smart Scan, el botón en la esquina superior derecha indica el plan actual del usuario ("Plan Premium"), informando qué funcionalidades tiene disponibles antes de que intente usarlas. |
| **Prevención de errores (H5)** | En Recommendations, el panel "Active filters" muestra los filtros activos aplicados a todas las sugerencias (Lactose-free, Seafood-free) con botón de eliminación por filtro. Esto previene que el usuario reciba recomendaciones que no puede consumir sin necesidad de revisar su perfil. En Pantry, el resumen calórico al final de la lista de ingredientes indica explícitamente cuántas calorías quedan disponibles para las recetas sugeridas. |
| **Reconocer antes que recordar (H6)** | En Pantry, cada ingrediente de la lista incluye su categoría debajo del nombre (Grain, Animal protein, Fruit, Vegetable, Seasoning), permitiendo al usuario reconocer el tipo de ingrediente sin necesidad de recordarlo. En Smart Scan, las dos opciones (Scan food dish / Scan restaurant menu) están separadas en tarjetas distintas con título y descripción, evitando que el usuario deba recordar qué opción usar según su contexto. |
| **Libertad y control del usuario (H3)** | En Recommendations, los filtros activos tienen un botón "x" individual que permite al usuario eliminar cada restricción de forma independiente sin necesidad de ir a la configuración del perfil. En Smart Scan, cada opción ofrece dos métodos de entrada alternativos ("Take photo" y "Upload image"), dando al usuario control sobre cómo interactúa con la funcionalidad. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Objects** | En Recommendations, cada plato sugerido es un objeto con atributos propios: nombre, descripción contextual, calorías, proteínas, etiqueta de intensidad y acción de registro. En Pantry, cada ingrediente es un objeto con nombre y categoría, que al combinarse con otros objetos genera un nuevo objeto: la receta sugerida con sus propios atributos nutricionales. |
| **Choices** | En Smart Scan, la pantalla presenta exactamente dos opciones claramente diferenciadas: escanear un plato individual o escanear un menú de restaurante. Esta bifurcación binaria reduce la carga de decisión del usuario y encamina el flujo según su contexto de uso real. En Subscription, las tres tarjetas de plan ofrecen opciones con distintos niveles de funcionalidad y precio para diferentes perfiles de usuario. |
| **Exemplars** | En Pantry, la receta sugerida "Chicken and Cucumber Salad" muestra un ejemplo concreto del resultado que el usuario puede obtener a partir de sus ingredientes disponibles, ilustrando el valor de la funcionalidad antes de que el usuario agregue más ingredientes. |
| **Multiple Classification** | En Recommendations, cada plato puede clasificarse simultáneamente por múltiples atributos: calorías, contenido proteico y nivel de intensidad (Light). Esto permite al usuario evaluar cada opción desde distintos criterios de decisión sin navegar a una vista de detalle. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Considera la situación del usuario (P2)** | En Recommendations, el contexto climático y de ubicación detectado automáticamente ("It's hot in Lima — 31°C · Sunny") adapta las sugerencias al entorno físico real del usuario en ese momento, reconociendo que las necesidades nutricionales varían según la situación contextual y no solo según los objetivos declarados. |
| **Ofrecer opciones (P5)** | En Smart Scan, la zona de carga de imagen ofrece tres métodos alternativos de entrada: arrastrar y soltar, tomar foto y subir imagen. Esto contempla distintos contextos de uso: usuario en escritorio con archivo guardado, usuario con cámara web disponible, o usuario que prefiere cargar desde galería. |
| **Priorizar el contenido (P6)** | En Subscription, el contenido de cada plan se organiza jerárquicamente: precio como dato primario en tamaño grande, descripción resumida en una línea, y lista de características detalladas como contenido secundario. Esto permite al usuario tomar una decisión preliminar por precio antes de leer los detalles. |
| **Agrega valor (P7)** | En Pantry, el sistema cruza los ingredientes disponibles del usuario con su déficit calórico restante y sus restricciones activas para generar recetas personalizadas etiquetadas con el objetivo del usuario ("Weight-loss"). Este cruce de variables agrega un valor que ninguna app de recetas estándar ofrece, mejorando directamente la experiencia de usuarios con metas nutricionales específicas. |

### 4.4.2. Web Applications Wireflow Diagrams

### WireFlow 1 — Dashboard

| **User Goal N°1** | Como buscador saludable, quiero visualizar un resumen de mi progreso nutricional diario y recibir alertas cuando supere mis límites calóricos, para mantener el control de mi alimentación. |
|---|---|

| **Task Flow** |
|---|
| 1. El buscador saludable accede al Dashboard. |
| 2. El buscador saludable visualiza sus calorías consumidas, quemadas y el balance neto del día. |
| 3. El buscador saludable registra sus comidas a lo largo del día. |
| 4. El buscador saludable completa su registro diario. |
| 5. El buscador saludable visualiza su racha activa de 7 días consecutivos completada. |

| <center>**Wireflow** |
|---|
|![Dashboard Wireflow](../assets/img/wireflows/dashboard.png)|

### WireFlow 2 — Daily Log

| **User Goal N°2** | Como buscador saludable, quiero buscar y registrar los alimentos que consumo en mi registro diario, para llevar un control preciso de mis macronutrientes y calorías. |
|---|---|

| **Task Flow** |
|---|
| 1. El buscador saludable accede a la sección Daily Log. |
| 2. El buscador saludable escribe el nombre del alimento en el buscador. |
| 3. El buscador saludable selecciona el alimento deseado de los resultados. |
| 4. El buscador saludable selecciona la porción y la comida (Breakfast / Lunch / Dinner). |
| 5. El buscador saludable visualiza la confirmación del alimento añadido al log. |

| <center>**Wireflow** |
|---|
|![Daily Log Wireflow](../assets/img/wireflows/dailylog.png)|

### WireFlow 3 — Smart Scan

| **User Goal N°3** | Como buscador saludable, quiero escanear o fotografiar un plato o menú para identificar automáticamente sus ingredientes y registrar su información nutricional, ahorrando tiempo en el registro manual. |
|---|---|

| **Task Flow** |
|---|
| 1. El buscador saludable accede a la sección Smart Scan. |
| 2. El buscador saludable selecciona la opción *"Take photo"* o *"Upload image"*. |
| 3. El buscador saludable captura o sube una foto de un plato. |
| 4. El buscador saludable visualiza los ingredientes identificados que componen el plato. |
| 5. El buscador saludable confirma y guarda el registro nutricional. |

| <center>**Wireflow** |
|---|
|![Smart Scan Wireflow](../assets/img/wireflows/smartscan.png)|

### WireFlow 4 — Recommendations

| **User Goal N°4** | Como buscador saludable, quiero recibir recomendaciones de platos personalizadas según mi ubicación y clima actual, para elegir opciones que se adapten a mi contexto y perfil nutricional. |
|---|---|

| **Task Flow** |
|---|
| 1. El buscador saludable accede a la sección Recommendations. |
| 2. El sistema detecta automáticamente la ubicación y temperatura del usuario. |
| 3. El buscador saludable visualiza las recomendaciones de platos personalizadas según su ubicación y clima actual. |
| 4. El buscador saludable selecciona un plato recomendado. |

| <center>**Wireflow** |
|---|
|![Recommendations Wireflow](../assets/img/wireflows/recommendation.png)|

### WireFlow 5 — Body Progress

| **User Goal N°5** | Como buscador saludable, quiero registrar y actualizar mi peso corporal para monitorear mi evolución física y mantener datos precisos sobre mi progreso. |
|---|---|

| **Task Flow** |
|---|
| 1. El buscador saludable accede a la sección Body Progress. |
| 2. El buscador saludable ingresa un nuevo valor de peso. |
| 3. El buscador saludable visualiza la previsualización del BMI y TDEE actualizados. |
| 4. El buscador saludable presiona *"Save entry"* para confirmar el nuevo registro de peso. |

| <center>**Wireflow** |
|---|
|![Body Progress Wireflow](../assets/img/wireflows/bodyprogress.png)|

### WireFlow 6 — Wearable

| **User Goal N°6** | Como buscador saludable, quiero conectar mi dispositivo wearable o registrar manualmente mi actividad física, para que mis calorías quemadas se reflejen con precisión en mi balance nutricional diario. |
|---|---|

| **Task Flow** |
|---|
| 1. El buscador saludable accede a la sección Wearable. |
| 2. El buscador saludable selecciona la opción *"Connect to Google Fit"*. |
| 3. La conexión con Google Fit se completa exitosamente. |
| 4. El buscador saludable visualiza el dashboard completo con los datos sincronizados desde Google Fit. |

| <center>**Wireflow** |
|---|
|![Wearable Wireflow](../assets/img/wireflows/wearable.png)|

### WireFlow 7 — Subscription

| **User Goal N°7** | Como buscador saludable, quiero suscribirme a un plan de pago para acceder a las funcionalidades avanzadas de NutriSmart. |
|---|---|

| **Task Flow** |
|---|
| 1. El buscador saludable accede a la sección Subscription and Billing. |
| 2. El buscador saludable visualiza los tres planes disponibles: Basic ($9.99), Pro ($14.99) y Premium ($19.99). |
| 3. El buscador saludable selecciona el plan deseado. |
| 4. El buscador saludable ingresa sus datos bancarios en el formulario de pago. |
| 5. El buscador saludable presiona el botón *"Pay"*. |
| 6. El buscador saludable visualiza la confirmación de pago y el mensaje de bienvenida al plan seleccionado. |

| <center>**Wireflow** |
|---|
|![Subscription Wireflow](../assets/img/wireflows/suscription.png)|

### 4.4.2. Web Applications Mock-ups

**Login, Dashboard, Analytics, Daily log & Balance progress**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/mockup/webapp/login.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/webapp/dashboard.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/webapp/analytics.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
    <tr>
      <td><img src="../assets/img/mockup/webapp/dailylog.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/webapp/balanceprogress.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Colour** | La paleta de la aplicación usa el verde azulado como color primario de acción e identidad, aplicado consistentemente en el ítem activo del menú lateral, los botones de acción principales ("Save entry", "+ Log weight", filtros activos), las barras de progreso de macronutrientes y los gráficos de Analytics. El color rosado/salmón se reserva exclusivamente para estados de alerta o exceso (barras "Over goal" en Analytics, indicador de Fats en Daily Log), creando un sistema cromático semántico donde el verde representa progreso positivo y el rosado representa advertencia. |
| **Colour (íconos de navegación)** | Cada ítem del menú lateral tiene un ícono temático con color propio: un grid para Dashboard, un check para Daily log, un reloj para Recommendations, una línea de tendencia para Body progress, un corazón para Pantry, y un gráfico de barras para Analytics. Estos íconos reemplazan los placeholders del wireframe, permitiendo al usuario reconocer cada sección por forma y color sin leer la etiqueta. |
| **Shape** | El gráfico de barras en Analytics usa dos colores de barra diferenciados (verde azulado para "On target", rosado para "Over goal") con una línea punteada horizontal que marca la meta calórica. Esta representación visual permite al usuario evaluar su desempeño semanal de un vistazo sin necesidad de leer los valores numéricos de cada barra. El gráfico de línea en Body Progress muestra la evolución del peso con área sombreada bajo la curva, reforzando visualmente la tendencia descendente. |
| **Size** | En Dashboard, el número "1340" de calorías consumidas y el "460" de calorías restantes se muestran en un tamaño notablemente mayor a sus etiquetas y unidades, estableciendo jerarquía numérica que permite al usuario escanear el estado diario en menos de un segundo. En Login, el título "Welcome back" ocupa el ancho completo del panel derecho, priorizando la bienvenida sobre el formulario. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Visibilidad del estado del sistema (H1)** | En Dashboard, la tarjeta "Calories Consumed" muestra una barra de progreso verde que indica visualmente qué porcentaje de la meta diaria ha sido consumido. En Analytics, la etiqueta "✓ Within target" en verde y "⚠ Below target" en amarillo comunican el estado de cada métrica de forma inmediata sin requerir interpretación del usuario. En Body Progress, el gráfico de línea muestra la trayectoria real del peso versus la meta con una línea punteada de referencia. |
| **Relación entre el sistema y el mundo real (H2)** | En Daily Log, cada comida usa un ícono de reloj con color diferenciado por tiempo del día (naranja para Breakfast, verde para Lunch, rosado para Snack), conectando el registro nutricional con el contexto temporal real del usuario. En Login, el panel izquierdo usa el verde azulado oscuro con ilustración del logo y funcionalidades clave, comunicando el valor del producto en el lenguaje cotidiano del usuario antes de que inicie sesión. |
| **Prevención de errores (H5)** | En Body Progress, el campo "Log weight" muestra el peso actual como placeholder ("E.g.: 70.2") y lo confirma debajo del campo ("Current weight: 70.2 kg"), permitiendo al usuario verificar el valor de referencia antes de registrar uno nuevo. El botón "Update height" aparece visualmente desactivado (gris claro) cuando no hay cambios pendientes, previniendo guardados accidentales sin modificaciones. |
| **Reconocer antes que recordar (H6)** | En Analytics, la leyenda del gráfico de barras incluye tres categorías con color y etiqueta ("Over goal" en rosado, "On target" en verde, "No data" en gris), permitiendo al usuario interpretar el gráfico por reconocimiento visual sin necesidad de recordar el significado de cada color. El indicador de días "M T W T F S S" en el panel de macros usa el mismo color verde para los días con registro completo, reforzando el patrón de reconocimiento. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Objects** | En Dashboard, el gráfico donut de macros trata cada nutriente (Protein, Carbohydrates, Fat) como un objeto con color propio y valor numérico actual versus meta. Cada segmento del donut representa un objeto vivo que cambia a medida que el usuario registra alimentos durante el día. En Analytics, cada barra del gráfico es un objeto con atributos de fecha, valor calórico y estado respecto a la meta. |
| **Disclosure** | En Dashboard, la sección "Today's log" muestra únicamente el nombre, contenido resumido, hora y calorías totales de cada comida, sin detallar los alimentos individuales. El usuario que quiera ver el detalle completo puede navegar a Daily Log, donde accede a cada alimento con sus macros desglosados. |
| **Multiple Classification** | En Analytics, el progreso del usuario puede evaluarse simultáneamente desde cuatro perspectivas en las tarjetas superiores: ingesta calórica promedio, ingesta proteica promedio, racha de consistencia y variación de peso semanal. Cada métrica ofrece una clasificación diferente del mismo período de tiempo. |
| **Growth** | En Daily Log, cada bloque de comida (Breakfast, Lunch, Snack, Dinner) puede expandirse con nuevas entradas sin alterar la estructura de la página. El sistema escala verticalmente añadiendo filas dentro del bloque correspondiente, manteniendo la organización por tiempo del día independientemente del número de alimentos registrados. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Agrega valor (P7)** | El gráfico donut en Dashboard agrega valor visual respecto a la presentación de barras del wireframe, permitiendo al usuario ver la proporción relativa de cada macronutriente dentro del total consumido y no solo los valores absolutos. La etiqueta "-300 Google Fit" en el Dashboard comunica que la actividad física real del usuario ya está descontada del balance calórico, un nivel de personalización que agrega valor diferencial. |
| **Priorizar el contenido (P6)** | En Analytics, las cuatro tarjetas de métricas superiores (calorías, proteínas, racha, peso) presentan el dato más relevante en tamaño grande con una etiqueta de estado debajo, priorizando la información de desempeño antes de mostrar los gráficos detallados. El usuario puede entender su situación semanal leyendo solo la fila superior. |
| **Proporciona experiencias comparables (P1)** | El sistema de color semántico (verde para positivo, rosado para alerta) se aplica de forma consistente en Daily Log, Dashboard y Analytics, garantizando que un usuario que aprende el significado de los colores en una sección pueda interpretarlos correctamente en cualquier otra vista de la aplicación. |
| **Deja al usuario mandar (P4)** | En Body Progress, el enlace "Edit goal →" permite al usuario modificar su meta de peso en cualquier momento sin necesidad de contactar soporte ni navegar a configuración. En Analytics, el botón "Export to PDF" y los filtros de rango temporal dan al usuario control completo sobre cómo y cuándo accede a sus propios datos históricos. |

**Recommendations, SmartScan, Suscription & Pantry**

<center>
<div align="center">
  <table>
    <tr>
      <td><img src="../assets/img/mockup/webapp/recommendations.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/webapp/smartscan.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
      <td><img src="../assets/img/mockup/webapp/suscription.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
    <tr>
      <td><img src="../assets/img/mockup/webapp/pantry.png" style="max-width:100%; max-height:300px; object-fit:contain;" /></td>
    </tr>
  </table>
</div>
</center>

Elementos de Diseño

| Elemento | Justificación |
|---|---|
| **Colour** | En Recommendations, el banner de contexto climático usa un fondo amarillo/dorado suave con un ícono de sol animado, diferenciándolo cromáticamente del resto del contenido para comunicar que es información contextual en tiempo real y no contenido estático. En Smart Scan, las dos zonas de carga se diferencian por color: la izquierda usa verde azulado (consistente con la paleta primaria de la app) y la derecha usa lavanda/violeta, estableciendo una distinción visual inmediata entre escanear un plato y escanear un menú. |
| **Colour (etiquetas nutricionales)** | En Pantry, las etiquetas de macros en la receta sugerida usan colores diferenciados por nutriente: verde azulado para Proteína (P 18g) y rosado para Grasas (G 8g), replicando el sistema de color semántico establecido en las vistas de Dashboard y Daily Log. Esto crea consistencia cromática en toda la aplicación para representar los mismos nutrientes. |
| **Shape** | En Recommendations, cada tarjeta de plato incorpora un ícono de avión de papel en verde azulado a la izquierda, reemplazando los placeholders de imagen del wireframe con un ícono que comunica ligereza y rapidez, coherente con las etiquetas "Light" y "Refreshing" de los platos sugeridos. En Subscription, los bullets de características usan círculos rellenos en verde azulado, estableciendo visualmente que todas las características listadas están incluidas en el plan. |
| **Texture** | En Smart Scan, las zonas de carga de imagen mantienen el borde punteado del wireframe pero incorporan un fondo ligeramente diferenciado del blanco de la tarjeta, creando una textura de área interactiva que guía al usuario hacia la acción de arrastrar o subir archivos sin necesidad de texto adicional. |

Heurísticas de Nielsen

| Heurística | Justificación |
|---|---|
| **Visibilidad del estado del sistema (H1)** | En Recommendations, el ícono de sol con fondo amarillo y el timestamp "Updated 5 mins ago" comunican que el sistema está activo y que los datos climáticos son recientes. En la esquina superior derecha, el indicador "Lima · 31°C" con borde redondeado actúa como widget de estado permanente que informa el contexto geográfico y climático actual sin ocupar espacio en el contenido principal. |
| **Prevención de errores (H5)** | En Smart Scan, el botón "Plan Premium" en la esquina superior derecha con ícono de estrella informa al usuario su plan actual antes de que intente usar la funcionalidad, previniendo la frustración de descubrir limitaciones de plan después de intentar ejecutar una acción. En Pantry, la nota "Suggested recipes respect your remaining deficit" debajo de la barra calórica advierte al usuario sobre el criterio de filtrado antes de que evalúe las recetas. |
| **Consistencia y estándares (H4)** | El menú lateral mantiene la misma estructura de íconos temáticos y división PRINCIPAL/TOOLS en todas las vistas de la aplicación. En Subscription, los tres botones de compra ("Buy basic plan", "Buy pro plan", "Buy premium plan") usan el mismo estilo visual de botón primario con fondo verde oscuro, aplicando consistencia en los elementos de conversión más importantes de la página. |
| **Reconocer antes que recordar (H6)** | En Recommendations, las etiquetas de atributos de cada plato (320 kcal, P 32g, Light) usan forma de píldora con fondo diferenciado del texto corrido, permitiendo al usuario escanear los atributos clave de cada recomendación sin necesidad de leer la descripción completa. En Pantry, cada ingrediente muestra su categoría debajo del nombre (Grain, Animal protein, Fruit), evitando que el usuario deba recordar a qué grupo pertenece cada ítem. |

Arquitectura de la Información (AI)

| Principio AI | Justificación |
|---|---|
| **Objects** | En Pantry, cada ingrediente de la lista es un objeto con nombre, categoría e ícono de corazón propio, y al combinarse con otros ingredientes genera un nuevo objeto: la receta sugerida con sus atributos nutricionales, calóricos y de objetivo. Este comportamiento de objetos que generan nuevos objetos refleja el principio de contenido vivo con ciclo de vida. |
| **Choices** | En Smart Scan, la pantalla ofrece exactamente dos opciones visuales y semánticamente diferenciadas por color y por ícono: cámara en verde azulado para platos y documento en lavanda para menús. Esta bifurcación binaria con diferenciación cromática reduce la carga de decisión y hace que la elección sea reconocible antes que recordada. |
| **Disclosure** | En Recommendations, cada tarjeta de plato muestra nombre, descripción en una línea, calorías, proteínas y nivel de intensidad sin revelar la receta completa ni el desglose nutricional detallado. El usuario que quiera más información puede hacer clic en la tarjeta para profundizar, aplicando el principio de mostrar solo lo suficiente para tomar una decisión. |
| **Multiple Classification** | En Pantry, la receta sugerida "Chicken and Cucumber Salad" puede clasificarse simultáneamente por calorías totales (480 kcal), por macros individuales (P 18g, G 8g), por objetivo ("Weight-loss") y por ingredientes disponibles. Esto permite al usuario evaluar la receta desde múltiples criterios sin abandonar la vista. |

Diseño Inclusivo

| Principio | Justificación |
|---|---|
| **Considera la situación del usuario (P2)** | En Recommendations, el sistema detecta automáticamente la ubicación y temperatura actual del usuario y adapta las sugerencias a su contexto físico real. El banner "It's hot in Lima — 31°C · Sunny" reconoce que las necesidades nutricionales varían según el entorno, no solo según los objetivos declarados en el perfil. |
| **Agrega valor (P7)** | En Pantry, el ícono de corazón junto a cada ingrediente agrega valor visual que comunica que estos son ingredientes "guardados" o favoritos del usuario, diferenciándolos de una lista genérica de alimentos. En Recommendations, la etiqueta "Peruvian dish" junto a "Hake ceviche" agrega valor cultural que conecta las sugerencias con la identidad gastronómica local del usuario en Lima. |
| **Ofrecer opciones (P5)** | En Smart Scan, cada zona de carga ofrece dos métodos de entrada alternativos ("Take photo" y "Upload image"), contemplando usuarios que interactúan desde dispositivos con cámara disponible y usuarios que prefieren subir archivos desde su galería o sistema de archivos. |
| **Priorizar el contenido (P6)** | En Subscription, el precio de cada plan se muestra en el mayor tamaño tipográfico de la tarjeta, seguido de una descripción resumida en una línea y luego la lista de características. Esta jerarquía permite al usuario tomar una decisión preliminar basada en el precio antes de evaluar los detalles, priorizando el dato más determinante en la toma de decisión. |

### 4.4.3. Web Applications User Flow Diagrams

### User Flow 1 — Dashboard

| | |
|---|---|
| **User Goal N°1** | Como buscador saludable, quiero visualizar un resumen de mi progreso nutricional diario y recibir alertas cuando supere mis límites calóricos, para mantener el control de mi alimentación. |

| | |
|---|---|
| **Happy Path** | 1. El buscador saludable accede al Dashboard. |
| | 2. El buscador saludable visualiza sus calorías consumidas, quemadas y el balance neto del día. |
| | 3. El buscador saludable registra sus comidas a lo largo del día. |
| | 4. El buscador saludable completa su registro diario. |
| | 5. El buscador saludable visualiza su racha activa de 7 días consecutivos completada. |

| | |
|---|---|
| **Unhappy Path 1** | 1. El buscador saludable accede al Dashboard. |
| | 2. El buscador saludable registra alimentos superando su límite calórico. |
| | 3. El buscador saludable visualiza la alerta de exceso calórico con el mensaje: *"You've exceeded your calorie target by 240 kcal. Consider having a lighter dinner tonight."* |
| | 4. El buscador saludable revisa la sugerencia correctiva mostrada en el Dashboard. |


| <center>**User Flow** |
|---|
|![Dashboard Userflow](../assets/img/userflows/dashboard.png)|

---

### User Flow 2 — Daily Log

| | |
|---|---|
| **User Goal N°2** | Como buscador saludable, quiero buscar y registrar los alimentos que consumo en mi registro diario, para llevar un control preciso de mis macronutrientes y calorías. |

| | |
|---|---|
| **Happy Path** | 1. El buscador saludable accede a la sección Daily Log. |
| | 2. El buscador saludable escribe el nombre del alimento en el buscador. |
| | 3. El alimento existe en la base de datos y no tiene restricciones. |
| | 4. El buscador saludable visualiza la opción del alimento deseado en los resultados. |
| | 5. El buscador saludable selecciona el alimento deseado. |
| | 6. El buscador saludable selecciona la porción y la comida (Breakfast / Lunch / Dinner). |
| | 7. El buscador saludable visualiza la confirmación del alimento añadido al log. |

| | |
|---|---|
| **Unhappy Path 1** | 1. El buscador saludable accede a la sección Daily Log. |
| | 2. El buscador saludable escribe el nombre del alimento en el buscador. |
| | 3. El alimento no existe en la base de datos. |
| | 4. El buscador saludable visualiza el mensaje de que no hay resultados y la opción *"+ Add manually"*. |

| | |
|---|---|
| **Unhappy Path 2** | 1. El buscador saludable accede a la sección Daily Log. |
| | 2. El buscador saludable escribe el nombre del alimento en el buscador. |
| | 3. El alimento existe pero contiene restricciones (alérgenos detectados). |
| | 4. El buscador saludable visualiza los resultados con los alérgenos detectados resaltados en amarillo. |

| | |
|---|---|
| **Unhappy Path 3** | 1. El buscador saludable accede a la sección Daily Log. |
| | 2. El buscador saludable añade un alimento que supera el límite calórico diario. |
| | 3. El límite calórico ha sido excedido. |
| | 4. El buscador saludable visualiza la advertencia de límite calórico superado resaltada en rojo dentro del Daily Log. |

| <center>**User Flow** |
|---|
|![DailyLog Userflow](../assets/img/userflows/dailylog.png)|

---

### User Flow 3 — Smart Scan

| | |
|---|---|
| **User Goal N°3** | Como buscador saludable, quiero escanear o fotografiar un plato o menú para identificar automáticamente sus ingredientes y registrar su información nutricional, ahorrando tiempo en el registro manual. |

| | |
|---|---|
| **Happy Path** | 1. El buscador saludable accede a la sección Smart Scan. |
| | 2. El buscador saludable tiene Plan Pro o Premium. |
| | 3. El buscador saludable selecciona la opción *"Take photo"* o *"Upload image"*. |
| | 4. La foto es reconocible y no tiene restricciones. |
| | 5. El buscador saludable visualiza los ingredientes identificados que componen el plato fotografiado. |
| | 6. El buscador saludable confirma y guarda el registro nutricional. |

| | |
|---|---|
| **Unhappy Path 1** | 1. El buscador saludable accede a la sección Smart Scan. |
| | 2. El buscador saludable tiene Plan Basic. |
| | 3. El buscador saludable visualiza la interfaz del Plan Basic con el mensaje de que Smart Scan no está disponible en su plan actual. |

| | |
|---|---|
| **Unhappy Path 2** | 1. El buscador saludable accede a la sección Smart Scan. |
| | 2. El buscador saludable tiene Plan Pro. |
| | 3. El buscador saludable selecciona la opción *"Take photo"* o *"Upload image"*. |
| | 4. La foto no es reconocible. |
| | 5. El buscador saludable visualiza el mensaje de advertencia: *"The image does not contain recognizable food"*, con las opciones de tomar otra foto o cargar una imagen. |

| | |
|---|---|
| **Unhappy Path 3** | 1. El buscador saludable accede a la sección Smart Scan. |
| | 2. El buscador saludable tiene Plan Pro. |
| | 3. El buscador saludable selecciona la opción *"Take photo"* o *"Upload image"*. |
| | 4. La foto es reconocible pero contiene restricciones alimentarias. |
| | 5. El buscador saludable visualiza los ingredientes con restricciones marcados en rojo y excluidos del total nutricional. |

| <center>**User Flow** |
|---|
|![SmartScan Userflow](../assets/img/userflows/smartscan.png)|

---

### User Flow 4 — Recommendations

| | |
|---|---|
| **User Goal N°4** | Como buscador saludable, quiero recibir recomendaciones de platos personalizadas según mi ubicación y clima actual, para elegir opciones que se adapten a mi contexto y perfil nutricional. |

| | |
|---|---|
| **Happy Path** | 1. El buscador saludable accede a la sección Recommendations. |
| | 2. El buscador saludable tiene Plan Pro o Premium. |
| | 3. El acceso a la ubicación está disponible y el modo avión está desactivado. |
| | 4. La temperatura detectada es baja. |
| | 5. El buscador saludable visualiza recomendaciones de platos para clima frío, filtradas por su perfil y ubicación (Lima). |

| | |
|---|---|
| **Unhappy Path 1** | 1. El buscador saludable accede a la sección Recommendations. |
| | 2. El buscador saludable tiene Plan Basic. |
| | 3. El buscador saludable visualiza el mensaje *"Contextual recommendations — Pro or Premium plan"* con el botón *"Check subscription"*. |

| | |
|---|---|
| **Unhappy Path 2** | 1. El buscador saludable accede a la sección Recommendations. |
| | 2. El buscador saludable tiene Plan Pro o Premium. |
| | 3. El acceso a la ubicación no está disponible. |
| | 4. El buscador saludable visualiza el aviso de ubicación no disponible. |

| | |
|---|---|
| **Unhappy Path 3** | 1. El buscador saludable accede a la sección Recommendations. |
| | 2. El buscador saludable tiene Plan Pro o Premium. |
| | 3. El acceso a la ubicación está disponible pero el modo avión está activado, detectando una ciudad distinta (Cusco). |
| | 4. El buscador saludable visualiza el Travel Mode activo con la ciudad detectada y recomendaciones de platos tradicionales de Cusco. |

| <center>**User Flow** |
|---|
|![Recommendations Userflow](../assets/img/userflows/recommendation.png)|

---

### User Flow 5 — Body Progress

| | |
|---|---|
| **User Goal N°5** | Como buscador saludable, quiero registrar y actualizar mi peso corporal para monitorear mi evolución física y mantener datos precisos sobre mi progreso. |

| | |
|---|---|
| **Happy Path** | 1. El buscador saludable accede a la sección Body Progress. |
| | 2. El último registro de peso tiene menos de 7 días de antigüedad. |
| | 3. El buscador saludable ingresa un valor de peso válido (positivo). |
| | 4. El buscador saludable visualiza la previsualización del BMI, TDEE actualizados. |
| | 5. El buscador saludable presiona *"Save entry"* para confirmar el nuevo registro de peso. |

| | |
|---|---|
| **Unhappy Path 1** | 1. El buscador saludable accede a la sección Body Progress. |
| | 2. El último registro de peso tiene más de 7 días de antigüedad. |
| | 3. El buscador saludable visualiza el aviso de datos desactualizados con el botón *"Log now"* para registrar su peso actual. |

| | |
|---|---|
| **Unhappy Path 2** | 1. El buscador saludable accede a la sección Body Progress. |
| | 2. El buscador saludable ingresa un valor inválido (negativo o no numérico). |
| | 3. El buscador saludable visualiza el mensaje de error en rojo: *"Weight must be a positive value greater than 0"* o *"Goal weight must be lower than your current weight"*. |

| <center>**User Flow** |
|---|
|![BodyProgress Userflow](../assets/img/userflows/bodyprogress.png)|

---

### User Flow 6 — Wearable

| | |
|---|---|
| **User Goal N°6** | Como buscador saludable, quiero conectar mi dispositivo wearable o registrar manualmente mi actividad física, para que mis calorías quemadas se reflejen con precisión en mi balance nutricional diario. |

| | |
|---|---|
| **Happy Path** | 1. El buscador saludable accede a la sección Wearable. |
| | 2. El buscador saludable tiene Plan Premium. |
| | 3. El buscador saludable visualiza las opciones: *"Connect to Google Fit"* y *"Manual log activity"*. |
| | 4. La conexión con Google Fit es exitosa. |
| | 5. El buscador saludable visualiza el dashboard completo con los datos sincronizados desde Google Fit. |

| | |
|---|---|
| **Unhappy Path 1** | 1. El buscador saludable accede a la sección Wearable. |
| | 2. El buscador saludable no tiene Plan Premium. |
| | 3. El buscador saludable visualiza el mensaje de que la función requiere un plan superior, con el botón *"View plans"*. |

| | |
|---|---|
| **Unhappy Path 2** | 1. El buscador saludable accede a la sección Wearable. |
| | 2. El buscador saludable tiene Plan Premium. |
| | 3. La conexión con Google Fit no se completa correctamente. |
| | 4. El buscador saludable visualiza el error de sincronización *"Google Fit sync error"* con los datos del último sync disponible. |
| | 5. El buscador saludable selecciona la opción *"Manual log activity"*. |
| | 6. El buscador saludable ingresa un valor inválido al registrar la actividad. |
| | 7. El buscador saludable visualiza el mensaje de advertencia de valor incorrecto. |

| <center>**User Flow** |
|---|
|![Wreable Userflow](../assets/img/userflows/wereable.png)|

---

### User Flow 7 — Subscription

| | |
|---|---|
| **User Goal N°7** | Como buscador saludable, quiero suscribirme a un plan de pago para acceder a las funcionalidades avanzadas de NutriSmart. |

| | |
|---|---|
| **Happy Path** | 1. El buscador saludable accede a la sección Subscription and Billing. |
| | 2. El buscador saludable visualiza los tres planes disponibles: Basic ($9.99), Pro ($14.99) y Premium ($19.99). |
| | 3. El buscador saludable selecciona el plan deseado (Basic, Pro o Premium). |
| | 4. El buscador saludable ingresa sus datos bancarios en el formulario de pago. |
| | 5. El buscador saludable presiona el botón *"Pay"*. |
| | 6. El pago es procesado exitosamente. |
| | 7. El buscador saludable visualiza la pantalla de confirmación de pago con el mensaje de bienvenida al plan seleccionado. |

| | |
|---|---|
| **Unhappy Path 1** | 1. El buscador saludable accede a la sección Subscription and Billing. |
| | 2. El buscador saludable selecciona un plan y completa el formulario de pago. |
| | 3. El buscador saludable presiona el botón *"Pay"*. |
| | 4. El pago no es procesado. |
| | 5. El buscador saludable visualiza la pantalla de error de pago con el mensaje *"Payment not processed. Your subscription has not been activated. Please check your details or try a different payment method."* |

| | |
|---|---|
| **Unhappy Path 2** | 1. El buscador saludable accede a la sección Subscription and Billing. |
| | 2. El buscador saludable selecciona un plan y revisa el resumen del pedido. |
| | 3. El buscador saludable presiona el botón *"Back"* para regresar a la selección de planes. |
| | 4. El buscador saludable visualiza nuevamente la pantalla de selección de planes. |

| <center>**User Flow** |
|---|
|![Subscription Userflow](../assets/img/userflows/suscription.png)|

## 4.5. Web Applications Prototyping

|   |
|---|
|<center> Desktop Web Browser|
|![Desktop Web Browser](../assets/img/prototyping/desktop.png)|

https://upcedupe-my.sharepoint.com/:v:/g/personal/u202411669_upc_edu_pe/IQARIaNnElxCSJ2CHvTwWK1NAZvtl3lP4tIWEVJMpTv8qkY?e=3WhL8q&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D


|   |
|---|
|<center> Mobile Web Browser|
|![Mobile Web Browser](../assets/img/prototyping/mobile.png)|

https://upcedupe-my.sharepoint.com/:v:/g/personal/u202411669_upc_edu_pe/IQARIaNnElxCSJ2CHvTwWK1NAZvtl3lP4tIWEVJMpTv8qkY?e=3WhL8q&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D


## 4.6. Domain-Driven Software Architecture

### 4.6.1. Design-Level EventStorming

### 4.6.2. Software Architecture Context Diagram

### 4.6.3. Software Architecture Container Diagrams

### 4.6.4. Software Architecture Components Diagrams

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams

## 4.8. Database Design

### 4.8.1. Database Diagrams