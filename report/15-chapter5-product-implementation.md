# CAPÍTULO V: Product Implementation, Validation & Deployment

El proceso de construcción, verificación y puesta en marcha de NutriSmart representa la fase donde los conceptos arquitectónicos se materializan en una solución funcional. Esta etapa es determinante para transformar los modelos de diseño en una plataforma operativa, permitiendo validar la viabilidad de nuestra propuesta tecnológica y asegurar que el producto final cumpla con los estándares de calidad esperados por los usuarios en el ecosistema de salud digital.

## 5.1. Software Configuration Management

La gestión de configuración de software (SCM) en NutriSmart garantiza la integridad y trazabilidad de todos los artefactos del proyecto durante su ciclo de vida. Este apartado detalla los procesos para administrar los cambios en el código fuente y la documentación, asegurando versiones reproducibles y una colaboración estructurada que minimice conflictos y optimice la calidad de las entregas finales.

### 5.1.1. Software Development Environment Configuration

En este apartado, el equipo detalla el ecosistema de herramientas digitales seleccionadas para la construcción de NutriSmart. Cada solución ha sido elegida para optimizar una fase específica del ciclo de vida, garantizando la interoperabilidad y el flujo de trabajo constante entre los miembros del proyecto.

**Project Management**

Con el fin de centralizar la administración de tareas y asegurar la sincronía del grupo, se adoptaron plataformas que permiten una planificación ágil y un seguimiento detallado del backlog.

- **Trello:** Herramienta de tipo SaaS. Se utilizó como el tablero Kanban principal para la organización de las User Stories y la asignación de responsabilidades individuales. Su interfaz permitió visualizar el progreso de cada funcionalidad desde su etapa de "To Do" hasta su validación final.

    [Link de registro o inicio de sesion](https://trello.com)

    **Evidencia de uso:**

    ![Trello Evidence](../assets/img/evidence/trello.png)

- **Microsoft Teams:** Herramienta de tipo SaaS. Se empleó como el centro neurálgico para la comunicación formal y síncrona del equipo. Esta plataforma permitió integrar las sesiones de videoconferencia con el almacenamiento compartido de archivos y el chat grupal, facilitando la toma de decisiones estratégicas y la organización de reuniones de sprint review y daily stand-ups.

    [Link de registro, inicio de sesion y descarga](https://www.microsoft.com/teams)

    **Evidencia de uso:**

    ![Teams Evidence](../assets/img/evidence/teams.png)

**Requirement Management**

Para la fase de análisis y especificación de los requerimientos de NutriSmart, se implementaron herramientas de modelado visual que permiten transformar las necesidades del usuario en estructuras técnicas comprensibles para todo el equipo.

- **Miro:** Herramienta de tipo SaaS. Se estableció como el entorno colaborativo principal para la captura de requisitos dinámicos. A través de sesiones de EventStorming, el equipo pudo identificar los eventos de dominio, las reglas de negocio y los flujos de trabajo de los 7 Bounded Contexts. Esta herramienta facilitó la transición de las necesidades del cliente hacia una lógica de sistema reactiva.

    [Link de registro o inicio de sesion](https://miro.com)

    **Evidencia de uso:**

    ![Miro Evidence](../assets/img/evidence/miro.png)

- **Structurizr:** Herramienta de tipo SaaS. Se utilizó para la especificación técnica de los requisitos arquitectónicos mediante el modelo C4. Esta suite permitió documentar el contexto del sistema, los contenedores y los componentes de manera jerárquica, asegurando que el diseño de software esté alineado estrictamente con las capacidades funcionales exigidas por la plataforma.

    [Link de registro o inicio de sesion](https://structurizr.com)

    **Evidencia de uso:**

    ![Structurizr Evidence](../assets/img/evidence/structurizr.png)

**Product UX/UI Design**

En el diseño de la interfaz y la experiencia del usuario para la salud digital, se utilizaron soluciones enfocadas en la fidelidad visual y el entendimiento de las necesidades del cliente.

- **Figma:** Herramienta de tipo SaaS. Se utilizó para la arquitectura visual de NutriSmart, permitiendo la creación de prototipos interactivos de alta fidelidad. Mediante esta plataforma, se definieron los estilos, la tipografía y los componentes de UI que aseguran una experiencia coherente y atractiva.

    [Link de registro, inicio de sesion y descarga](https://www.figma.com)

    **Evidencia de uso:**

    ![Figma Evidence](../assets/img/evidence/figma.jpeg)

- **UXPressia:** Herramienta de tipo SaaS. Se aplicó para la construcción de los Customer Journey Maps y el análisis de los perfiles de usuario (User Personas). Permitió identificar los puntos de dolor de los usuarios al gestionar su nutrición, orientando el diseño hacia soluciones personalizadas.

    [Link de registro o inicio de sesion](https://uxpressia.com)

    **Evidencia de uso:**

    ![UXPressia Evidence](../assets/img/evidence/uxpressia.png)

**Software Development**

Para la fase de construcción de la plataforma, se seleccionaron entornos de desarrollo integrados (IDE) que maximizan la productividad del equipo y aseguran la calidad del código fuente mediante herramientas avanzadas de depuración y autocompletado.

- **Visual Studio Code:** Herramienta de tipo Desktop (IDE). Se utilizó como el entorno de trabajo versátil para la edición de scripts, archivos de configuración y la integración de herramientas de control de versiones. Gracias a su ecosistema de extensiones, permitió una edición ágil y personalizada de los diferentes módulos del proyecto, facilitando una codificación ligera y eficiente.

    [Link de descarga](https://code.visualstudio.com/)

    **Evidencia de uso:**

    ![VSCode Evidence](../assets/img/evidence/vscode.png)

- **IntelliJ IDEA:** Herramienta de tipo Desktop (IDE). Se empleó como el entorno de desarrollo integrado especializado para la arquitectura del backend en Spring Boot con Java. Su potente motor de análisis de código permitió gestionar de forma robusta los componentes del dominio y asegurar que la lógica del servidor cumpliera con los estándares de rendimiento exigidos por la plataforma.

    [Link de descarga](https://www.jetbrains.com/idea/)

- **WebStorm:** Herramienta de tipo Desktop (IDE). Se empleó como el entorno de desarrollo integrado especializado para la arquitectura del frontend en Angular. Su potente motor de análisis de código permitió gestionar de forma robusta los componentes reactivos de la interfaz y asegurar que la lógica de cliente cumpliera con los estándares de rendimiento exigidos por la plataforma.

    [Link de descarga](https://www.jetbrains.com/webstorm/)

**Software Testing**

Con el objetivo de garantizar la calidad y el cumplimiento de los criterios de aceptación, se utilizó un estándar de especificación basado en el comportamiento.

- **Gherkin:** Lenguaje de especificación técnica. Se implementó para definir los escenarios de prueba bajo el formato "Given, When, Then". Su uso permitió que las validaciones del sistema fueran legibles tanto para el equipo de desarrollo como para el área de negocio, asegurando que cada funcionalidad opere según lo previsto.

    [Link de la documentacion y uso](https://cucumber.io/docs/gherkin/)

    **Evidencia de uso:**

    ![Gherkin Evidence](../assets/img/evidence/gherkin.jpeg)

**Software Documentation**

La gestión de los activos digitales y la preservación del historial de cambios se realizó mediante una plataforma líder en el control de versiones.

- **GitHub:** Herramienta de tipo SaaS. Se utilizó como el repositorio maestro de NutriSmart, donde se resguardó el código fuente, la documentación técnica y las definiciones de pruebas. Su infraestructura permitió la colaboración asíncrona entre desarrolladores y garantizó la trazabilidad total del proyecto.

    [Link de registro o inicio de sesion](https://github.com)

    **Evidencia de uso:**

    ![GitHub Evidence](../assets/img/evidence/github.png)

**Software Deployment**

Con el propósito de garantizar la accesibilidad de la propuesta de valor inicial y automatizar su publicación, se utilizó un servicio de alojamiento en la nube que permite el despliegue efectivo del sitio de presentación (Landing Page). Este enfoque asegura que los interesados puedan visualizar la solución preliminar de forma rápida y confiable.

- **GitHub Pages:** Herramienta de tipo SaaS. Actúa como la plataforma de publicación estática para la difusión inicial del proyecto. Su implementación permitió automatizar el ciclo de actualización a partir del código fuente resguardado en la rama principal, facilitando una sincronización inmediata entre los ajustes realizados por el equipo y la versión web disponible para los usuarios.

    [Link de la documentacion y uso](https://pages.github.com/)

### 5.1.2. Source Code Management

Para garantizar la integridad y el control total sobre las modificaciones del software, el equipo ha seleccionado GitHub como plataforma centralizada de gestión de versiones. Este sistema permite una colaboración distribuida y asíncrona, facilitando la auditoría de cambios y la integración de las diferentes capas de la aplicación NutriSmart.

**Repositorios del Proyecto**

La solución se ha segmentado en repositorios independientes para mantener una arquitectura limpia y una separación de responsabilidades clara:

- **nutrismart-website:** Repositorio dedicado al sitio de presentación estática (Landing Page).

    [Link del repositorio nutrismart-website](https://github.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-website)

- **nutrismart-platform:** Contiene el núcleo de la solución (Backend), desarrollado como una API RESTful en Java con Spring Boot. Este repositorio aloja la lógica de negocio, los servicios de dominio y las suites de pruebas automatizadas.

    [Link del repositorio nutrismart-platform](https://github.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-platform)

- **nutrismart-webapp:** Espacio reservado para el código del cliente web (Frontend) construido en Angular.

    [Link del repositorio nutrismart-webapp](https://github.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp)

- **nutrismart-report:** Repositorio de soporte utilizado para la gestión de la documentación técnica y los informes del proyecto.

    [Link del repositorio nutrismart-report](https://github.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-report)

**Implementación de GitFlow**

Para la organización y administración de la base de código, el equipo ha adoptado el esquema de ramificación GitFlow. Este flujo de trabajo se fundamenta en el modelo estratégico propuesto por Vincent Driessen en su publicación "A successful Git branching model", el cual proporciona una estructura robusta para gestionar el ciclo de vida del software mediante roles específicos para cada rama:

- **Main Branch:** Resguarda el código fuente definitivo que se encuentra en el entorno de producción. Es la versión oficial y estable de NutriSmart; cualquier cambio aquí representa una versión liberada al usuario.
    - **Notación:** `main o master`.
- **Develop Branch:** Actúa como la rama matriz para la integración de todas las capacidades técnicas en desarrollo. Es el espacio donde se consolidan las funcionalidades antes de ser enviadas a la fase de publicación.
    - **Notación:** `develop`.
- **Feature Branches:** Segmentos temporales creados para trabajar en requerimientos específicos o historias de usuario del backlog. Se originan a partir de develop y deben reintegrarse a esta misma rama una vez finalizada y validada la tarea.
    - **Notación:** `feature/US-nombre`.
- **Release Branches:** Utilizadas para preparar un lanzamiento oficial de la plataforma. Permiten realizar auditorías finales, ajustes de configuración y correcciones menores sin interrumpir el desarrollo de nuevas funciones en la rama matriz.
    - **Notación:** `release/vX.Y.Z`.
- **Hotfix Branches:** Ramas de corrección urgente creadas directamente desde main para resolver errores críticos detectados en producción. Una vez corregido el problema, se fusionan tanto en main como en develop para mantener la consistencia del código en todas las ramas activas.
    - **Notación:** `hotfix/nombre-del-error`.

**Conventional Commits**

Se adopta esta convención para estandarizar el historial de cambios y facilitar la generación automática de bitácoras (changelogs). Este estándar permite identificar rápidamente la intención de cada modificación mediante una estructura semántica clara.

El formato mandatorio es: `<tipo>[alcance]: <descripción>`, el cual incluye un encabezado obligatorio y, de ser necesario, un cuerpo técnico y pie de página para referencias.

Los tipos de confirmación permitidos para este proyecto son:

- **feat:** Incorporación de una nueva funcionalidad o capacidad al sistema.
- **fix:** Resolución de un error técnico, bug o comportamiento no deseado.
- **docs:** Modificaciones exclusivas en la documentación, manuales o archivos README.
- **style:** Ajustes relacionados con el formato, indentación o estética del código sin alterar su lógica funcional.
- **chore:** Labores de mantenimiento, actualizaciones de dependencias o ajustes en la configuración del entorno de compilación.
- **refactor:** Cambios en la estructura del código destinados a mejorar su legibilidad o eficiencia interna.
- **test:** Inclusión, corrección o actualización de escenarios de pruebas unitarias o de integración.

**Semantic Versioning**

Se emplea la versión 2.0.0 de Semantic Versioning bajo el esquema vX.Y.Z:

- **X (MAYOR):** Cambios grandes o incompatibles con versiones anteriores.
- **Y (MINOR):** Nuevas funcionalidades compatibles con versiones anteriores.
- **Z (PATCH):** Correcciones menores o parches que no afectan la funcionalidad.

### 5.1.3. Source Code Style Guide & Conventions

Para asegurar que el código de NutriSmart sea mantenible, escalable y profesional, el equipo ha adoptado una serie de normas y guías de estilo internacionales. Como política fundamental, toda la nomenclatura técnica (variables, clases, métodos y comentarios) será redactada íntegramente en inglés, garantizando un estándar global en el desarrollo.

**Convenciones aplicadas por lenguaje:**

**HTML**

Siguiendo la "HTML Style Guide and Coding Conventions" de W3Schools y la "Google HTML/CSS Style Guide", se mantiene una arquitectura semántica y accesible. El código se escribe íntegramente en minúsculas, con una indentación de dos espacios y comentarios descriptivos para separar bloques funcionales.

**Estructura y etiquetas principales empleadas:**

- **Base:** `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>` para la jerarquía global.
- **Metadatos:** `<meta>`, `<title>`, `<link>` para la configuración y vinculación de estilos.
- **Semántica:** `<nav>`, `<section>`, `<header>`, `<footer>`, `<main>` para la organización del contenido principal.
- **Contenido:** `<h1>`, `<h2>`, `<p>`, `<img>`, `<a>` para la visualización de métricas y enlaces.
- **Interacción:** `<form>`, `<input>`, `<label>`, `<button>` para el registro de datos en formularios interactivos.

**CSS**

El archivo styles.css se estructuró bajo la "Google HTML/CSS Style Guide", aplicando una organización modular mediante comentarios (ej. /* NAVIGATION */, /* HERO CAROUSEL */). Se emplea kebab-case para clases y una indentación uniforme.

**Propiedades y convenciones aplicadas:**

- **Diseño y Layout:** `display: flex`, `grid-template-columns`, `position`, `z-index` para una interfaz responsiva.
- **Dimensiones:** `width`, `height`, `max-width`, `min-height`.
- **Espaciado:** `padding`, `margin`, `gap`.
- **Tipografía:** `font-family`, `font-size`, `font-weight`, `line-height`, `color`.
- **Decoración:** `background-color`, `border-radius`, `box-shadow`, `border`.
- **Interactividad:** `transition`, `transform`, `:hover` para mejorar la experiencia de usuario.

**JavaScript**

La lógica de cliente se fundamenta en las "MDN JavaScript guidelines" y la "W3C JavaScript Style Guide", priorizando un código modular, seguro y de alto rendimiento. Se emplean comentarios descriptivos en inglés para documentar la finalidad de cada bloque funcional y se aplica la convención camelCase para la nomenclatura de variables y funciones.

**Estructura y elementos técnicos aplicados:**

- **Selección del DOM:** Uso de métodos estandarizados como `document.getElementById()` y `document.querySelector()` para la captura de elementos de la interfaz.
- **Gestión de Eventos:** Implementación de `addEventListener()` para controlar acciones como click (botones de registro), submit (formularios de métricas) y el evento `DOMContentLoaded` para asegurar la carga del script.
- **Validaciones de Datos:** Aplicación de expresiones regulares para verificar la integridad de correos electrónicos, teléfonos y formatos de entrada.
- **Interacción Dinámica:** Manipulación de clases mediante `classList` para menús interactivos, modales de confirmación y feedback visual en formularios.
- **Control Lógico:** Empleo de condicionales `(if/else)`, bucles de iteración `(forEach)` y temporizadores `(setInterval())` para la actualización de datos en tiempo real.

**TypeScript**

El desarrollo del frontend en Angular se rige por la "Angular Style Guide" oficial y las "Google TypeScript Style Guide". Estas normas garantizan que los componentes, servicios e interfaces de NutriSmart sean robustos, escalables y fáciles de mantener por cualquier miembro del equipo.

**Convenciones de tipografía y estructura:**

- **PascalCase:** Para nombres de clases, componentes e interfaces `(ej. NutritionService)`.
- **camelCase:** Para variables locales, propiedades y métodos `(ej. dailyGoal, getUserData())`.
- **kebab-case:** Para nombres de archivos y selectores de componentes `(ej. user-profile.component.ts, app-nutrition-log)`.
- **Principios SOLID:** Implementación del Principio de Responsabilidad Única (SRP). Cada componente o servicio gestiona una operación atómica del dominio, evitando el acoplamiento innecesario y facilitando las pruebas unitarias.
- **Tipado estricto:** Se utiliza el modo estricto de TypeScript para garantizar la integridad de los datos en tiempo de compilación.

**Java**

El desarrollo del backend se rige por la "Google Java Style Guide" y las convenciones oficiales de Oracle. Estas normas aseguran que la lógica de los 7 Bounded Contexts de NutriSmart sea robusta, escalable y fácil de auditar por cualquier miembro del equipo técnico.

**Convenciones de tipografía y estructura:**

- **PascalCase:** Para nombres de clases e interfaces `(ej. public class UserProfile, NutritionService)`.
- **camelCase:** Para métodos, parámetros y variables locales `(ej. int currentCalories, calculateDailyGoal())`.
- **Principios SOLID:** Implementación rigurosa del Principio de Responsabilidad Única (SRP). Cada servicio o controlador de Spring Boot gestiona una operación atómica del dominio, evitando el acoplamiento innecesario y facilitando las pruebas unitarias.
- **Formateo y Claridad:** Se utilizan comentarios concisos en inglés para documentar la finalidad de métodos complejos y se aplican las anotaciones de Spring Boot de forma explícita para mejorar la legibilidad del código.

**Gherkin (.feature)**

Las pruebas de aceptación del sistema fueron redactadas empleando la sintaxis Gherkin, siguiendo las "Gherkin Conventions for Readable Specifications". Estos archivos se encuentran organizados por historias de usuario dentro del repositorio de GitHub, asegurando una trazabilidad total entre el requerimiento funcional y su validación técnica.

**Convenciones aplicadas:**

- **Estructura canónica Given – When – Then:** Se emplea este formato de forma estricta para mapear la secuencia lógica y las precondiciones, acciones y resultados esperados de cada caso de prueba.
- **Uso de Scenario Outline y Examples:** Se implementan plantillas de escenarios junto con tablas de datos para validar de manera eficiente diversos flujos de entrada y salida.
- **Equilibrio de lenguaje:** Se utiliza un léxico que balancea la terminología técnica con el lenguaje de negocio, facilitando que tanto analistas como desarrolladores mantengan una visión compartida del sistema.

### 5.1.4. Software Deployment Configuration

Durante este sprint se configuraron la organización y los repositorios del proyecto NutriSmart en GitHub, estableciendo la estructura base para el despliegue de todos los productos digitales de la solución. A continuación se describen los pasos realizados.

##### Creación de la organización en GitHub

Se creó la organización `upc-pre-202610-1asi0729-17952-devteam` en GitHub, la cual centraliza todos los repositorios del proyecto. Para crearla:

- Iniciar sesión en [github.com](https://github.com)
- Hacer click en el ícono de perfil → **Your organizations**
- Click en **New organization**
- Seleccionar el plan **Free**
- Ingresar el nombre `upc-pre-202610-1asi0729-17952-devteam`
- Completar la configuración e invitar a los miembros del equipo

##### Creación de los repositorios

Dentro de la organización se crearon 4 repositorios, uno por cada producto digital de la solución:

| Repositorio | Descripción |
|---|---|
| `nutrismart-report` | Documentación e informe del proyecto |
| `nutrismart-website` | Landing page estática |
| `nutrismart-webapp` | Frontend Web Application |
| `nutrismart-platform` | Web Services / Backend |

Para crear cada repositorio:

- Ir a la organización → **Repositories** → **New**
- Asignar el nombre correspondiente
- Seleccionar visibilidad **Public**
- Inicializar con un `README.md`
- Click en **Create repository**

##### Configuración de ramas base (Gitflow)

En cada repositorio se configuraron las ramas base del flujo de trabajo:

- Por defecto GitHub crea la rama `main`
- Desde `main` se crea la rama `develop`
- Se establece `develop` como rama base para los Pull Requests en **Settings** → **Branches** → **Default branch**

## 5.2. Landing Page, Services & Applications Implementation

La implementación del Landing Page, los servicios web y las aplicaciones representa la etapa crítica donde el equipo consolida el desarrollo de NutriSmart. Este proceso permite materializar el diseño y las funcionalidades planificadas, transformando los requisitos en un producto tangible y operativo. En esta fase se traduce cada especificación técnica en código fuente, construyendo la infraestructura necesaria para satisfacer las necesidades identificadas de los segmentos objetivo.

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1

<table>
  <tr>
    <th colspan="2">Sprint #</th>
    <th colspan="2">Sprint 1</th>
  </tr>
  <tr>
    <th colspan="4">Sprint Planning Background</th>
  </tr>
  <tr>
    <td colspan="2">Date</td>
    <td colspan="2">2026-04-03</td>
  </tr>
  <tr>
    <td colspan="2">Time</td>
    <td colspan="2">06:00 PM (GMT-5)</td>
  </tr>
  <tr>
    <td colspan="2">Location</td>
    <td colspan="2">Reunión presencial</td>
  </tr>
  <tr>
    <td colspan="2">Prepared By</td>
    <td colspan="2">Villarreal Bazan, Angel Martin</td>
  </tr>
  <tr>
    <td colspan="2">Attendees (to planning meeting)</td>
    <td colspan="2">Del Aguila Del Aguila, Olenka Priscilla / Espinoza Cruz, Angela Milagros / Mora Rivera, Joel Fernando / Soto Palacios, Brandon Wilder / Villarreal Bazan, Angel Martin</td>
  </tr>
  <tr>
    <th colspan="4">Sprint n – 1 Review Summary</th>
  </tr>
  <tr>
    <td colspan="4">No aplica. El Sprint 1 es el primero de la cadencia del proyecto NutriSmart. No existe sprint anterior que revisar.</td>
  </tr>
  <tr>
    <th colspan="4">Sprint n – 1 Retrospective Summary</th>
  </tr>
  <tr>
    <td colspan="4">No aplica. Al ser la primera iteración, no hay retrospectiva previa documentada. El equipo acordó en esta reunión establecer como normas de trabajo el uso de GitFlow con ramas <code>feature/</code>, <code>develop</code> y <code>main</code>, Conventional Commits para todos los mensajes, y revisión de Pull Requests con mínimo un aprobador antes de hacer merge a <code>develop</code>.</td>
  </tr>
  <tr>
    <th colspan="4">Sprint Goal &amp; User Stories</th>
  </tr>
  <tr>
    <td colspan="2">Sprint 1 Goal</td>
    <td colspan="2">Our focus is on delivering a fully functional and publicly accessible NutriSmart Landing Page in both English and Spanish. We believe it delivers a clear understanding of the platform's value proposition, subscription plans, and team identity to potential users from both target segments,adults seeking weight loss and young adults seeking muscle gain. This will be confirmed when any visitor can navigate all landing page sections (Hero, Features, Plans, About Us, FAQ, Contact), switch the interface language between English (en_US) and Spanish (es_419), and access the web application entry point from the landing page without any broken links or accessibility violations.</td>
  </tr>
  <tr>
    <td colspan="2">Sprint 1 Velocity</td>
    <td colspan="2">15 Story Points</td>
  </tr>
  <tr>
    <td colspan="2">Sum of Story Points</td>
    <td colspan="2">15 Story Points</td>
  </tr>
</table>

#### 5.2.1.2. Aspect Leaders and Collaborators

El Sprint 1 abarca exclusivamente la construcción del sitio web estático (Landing Page) de NutriSmart. Los aspectos identificados para organizar el liderazgo y la colaboración en este sprint son los siguientes:

**Hero & Navigation:** Comprende el carrusel de la sección hero con sus tres diapositivas (call-to-action, video del producto, video del equipo), la barra de navegación y el enrutamiento entre páginas del sitio estático.

**Features, Plans & FAQ:** Comprende la sección de tres funciones principales destacadas, la subpágina de lista completa de funciones, la tabla comparativa de planes Basic / Pro / Premium y la sección de preguntas frecuentes con acordeón interactivo.

**About Us & Contact:** Comprende la subpágina About Us con la descripción de la startup, misión y visión, el formulario de contacto con validación del lado cliente y el despliegue de los enlaces a redes sociales.

**i18n & a11y:** Comprende la implementación del módulo de internacionalización (en_US / es_419) con persistencia de preferencia de idioma durante la sesión, y el cumplimiento de accesibilidad con atributos ARIA en todos los componentes interactivos (carrusel, acordeón FAQ, formulario, navegación).

**Terms of Service & Footer:** Comprende la subpágina de Términos y Condiciones, el footer global con enlaces legales, redes sociales, selector de idioma y copyright, y el vínculo del botón de login con el punto de entrada de la aplicación web.

| Team Member (Last Name, First Name) | GitHub Username | Hero & Navigation | Features, Plans & FAQ | About Us & Contact | i18n & a11y | Terms of Service & Footer |
|-------------------------------------|-----------------|:-----------------:|:---------------------:|:------------------:|:-----------:|:-------------------------:|
| Del Aguila Del Aguila, Olenka Priscilla | olenkisha_14 | C | L | C | C | C |
| Espinoza Cruz, Angela Milagros | Emy127 | C | C | L | C | C |
| Mora Rivera, Joel Fernando | xJoelFMRx | L | C | C | C | C |
| Soto Palacios, Brandon Wilder | Brandon1677 | C | C | C | C | L |
| Villarreal Bazan, Angel Martin | nevatrix | C | C | C | L | C |

#### 5.2.1.3. Sprint Backlog 1

El Sprint 1 tiene como objetivo principal entregar el sitio web estático (Landing Page) de NutriSmart completamente funcional, accesible y desplegado públicamente. Todos los User Stories de este sprint pertenecen al Epic EP_LS Landing Page y cubren las secciones del sitio: Hero con carrusel, Funciones principales, Comparativa de planes, Cambio de idioma, Términos y condiciones, About Us, FAQ, formulario de contacto y enlaces a redes sociales. El entregable del sprint es la Landing Page publicada en GitHub Pages y accesible desde cualquier navegador de escritorio o móviL.
A continuación se presenta el board del sprint en Trello y la tabla de work-items correspondiente.

![Board Sprint 1](../assets/img/sprint1/sprintbacklog.png)
URL del Board (Trello): [Enlace Trello](https://trello.com/invite/b/69e7e914df07d176838add9d/ATTIdd4dfe357744be4dc97cce9e1ff43aeeC1917E49/sprint-1)

| US ID | US Title | Task ID | Task Title | Description | Est. (h) | Assigned To | Status |
|-------|----------|---------|------------|-------------|----------|-------------|--------|
| US-LP01 | View Hero Section with Carousel | T01 | Set up repository and project structure | Create the GitHub repository, configure GitFlow with `main` / `develop` / `feature/*` branches, add `.gitignore`, `README.md`, and establish the base folder structure (`/assets`, `/css`, `/js`, `/pages`). | 2 | Villarreal Bazan, Angel Martin | Done |
| US-LP01 | View Hero Section with Carousel | T02 | Implement global CSS design tokens and base styles | Define CSS custom properties (color palette, typography scale, spacing, border-radius, transition) aligned with Material Design guidelines and the NutriSmart style guide. | 3 | Villarreal Bazan, Angel Martin | Done |
| US-LP01 | View Hero Section with Carousel | T03 | Build navbar component with responsive hamburger menu | Implement the fixed top navigation bar including logo, navigation links, language selector, login button, and hamburger menu for mobile breakpoints with ARIA `role="navigation"` and `aria-label`. | 3 | Villarreal Bazan, Angel Martin | Done |
| US-LP01 | View Hero Section with Carousel | T04 | Build hero carousel CTA slide | Implement the first carousel slide with headline, subtitle, and CTA button that redirects to the web application authentication entry point. Apply `aria-live="polite"` and `role="region"` to the carousel container. | 3 | Villarreal Bazan, Angel Martin | Done |
| US-LP01 | View Hero Section with Carousel | T05 | Build hero carousel abt-product video slide | Implement the second carousel slide embedding the About-the-Product video, ensuring the video is playable and the slide is reachable via carousel navigation controls. | 2 | Villarreal Bazan, Angel Martin | Done |
| US-LP01 | View Hero Section with Carousel | T06 | Build hero carousel abt-team video slide | Implement the third carousel slide embedding the About-the-Team video. Add previous/next navigation buttons with `aria-label="Previous slide"` and `aria-label="Next slide"`. | 2 | Villarreal Bazan, Angel Martin | Done |
| US-LP02 | View Main Features Section | T07 | Build feature highlights section (3 featured capabilities) | Implement the features section on `index.html` displaying exactly three capability cards, each with an icon, title, and brief description. Add a "See all features" link pointing to `features.html`. | 3 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| US-LP02 | View Main Features Section | T08 | Build `features.html` full features subpage | Create the complete features subpage listing all platform capabilities organised by category, each with title and functional description. Apply page hero, teal grid layout and consistent footer. | 3 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| US-LP03 | View Subscription Plans Comparison Table | T09 | Build subscription plans comparison section | Implement the three-column plans comparison table (Basic, Pro, Premium) with feature availability indicators and a CTA button per plan that redirects to the registration flow. | 3 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| US-LP04 | Switch Interface Language (Landing) | T10 | Implement i18n module with `en_US` and `es_419` string dictionaries | Create `i18n.js` with `en` and `es` translation maps covering all text content across all pages. Implement the `applyTranslation(lang)` function that updates all elements with `data-i18n` attributes. | 4 | Mora Rivera, Joel Fernando | Done |
| US-LP04 | Switch Interface Language (Landing) | T11 | Implement language toggle and session persistence | Wire the language selector in the navbar and footer to `applyTranslation()`. Persist the selected language in `sessionStorage` so the choice is maintained as the visitor navigates between pages. | 2 | Mora Rivera, Joel Fernando | Done |
| US-LP04 | Switch Interface Language (Landing) | T12 | Add `data-i18n` attributes to all HTML elements across all pages | Audit all pages (`index.html`, `features.html`, `about-us.html`, `contact.html`, `terms.html`) and add `data-i18n` attributes to every text node that must be translated. | 3 | Mora Rivera, Joel Fernando | Done |
| US-LP05 | View Terms of Service | T13 | Build `terms.html` Terms and Conditions subpage | Create the Terms of Service page with full legal content (privacy policy, data use, subscription terms). Ensure the page is linked from the footer on all pages and content renders in the active language. | 2 | Soto Palacios, Brandon Wilder | Done |
| US-LP05 | View Terms of Service | T14 | Build global footer component | Implement the site-wide footer with the NutriSmart tagline, navigation links, social media links, language selector, Terms and Conditions link, and copyright notice. Apply consistent styles across all pages. | 3 | Soto Palacios, Brandon Wilder | Done |
| US-LP06 | View About Us Section | T15 | Build `about-us.html` — startup description, mission and vision | Implement the About Us page hero section and the startup description block with mission and vision cards. Content must be i18n-ready with `data-i18n` attributes. | 3 | Espinoza Cruz, Angela Milagros | Done |
| US-LP06 | View About Us Section | T16 | Add team member cards section to `about-us.html` | Implement the team member cards section displaying each member's name, role, and avatar image. | 2 | Espinoza Cruz, Angela Milagros | Done |
| US-LP07 | View Frequently Asked Questions Section | T17 | Build FAQ accordion component on `about-us.html` and `features.html` | Implement the FAQ section with at least five question-and-answer pairs using a keyboard-accessible accordion pattern with `aria-expanded`, `aria-controls`, and `role="region"` on each answer panel. | 3 | Espinoza Cruz, Angela Milagros | Done |
| US-LP08 | Access Login from Landing Page | T18 | Add persistent login access option to all page headers | Ensure the login button is present in the navbar on every page and correctly redirects to the web application authentication entry point URL. | 1 | Mora Rivera, Joel Fernando | Done |
| US-LP09 | Submit Contact Form | T19 | Build `contact.html` contact form with client-side validation | Create the contact page with name, email, phone, and message fields. Implement client-side validation: required fields, email format, phone format, minimum message length. Display inline error messages with `role="alert"` for each invalid field. | 4 | Espinoza Cruz, Angela Milagros | Done |
| US-LP09 | Submit Contact Form | T20 | Implement contact form submission confirmation feedback | On valid submission, display a success confirmation message and reset the form. Ensure the confirmation is announced by screen readers using `aria-live="assertive"`. | 2 | Espinoza Cruz, Angela Milagros | Done |
| US-LP10 | View Social Media Links | T21 | Implement social media links section in footer | Add at least three social media profile links to the footer. Each link must open in a new tab with `target="_blank" rel="noopener noreferrer"` and include an `aria-label` describing the destination. | 1 | Soto Palacios, Brandon Wilder | Done |

#### 5.2.1.4. Development Evidence for Sprint Review

Durante este sprint, el equipo completó la implementación completa de la landing page de NutriSmart. El desarrollo abarcó la creación de todas las páginas (index, features, about us, contact y terms), la hoja de estilos compartida con su sistema de diseño, las interacciones en JavaScript, la internacionalización (i18n) y los assets estáticos del proyecto. Todo el trabajo fue gestionado mediante Gitflow, con ramas feature individuales por página fusionadas en `develop` y finalmente liberadas en `main` como versión 1.0.0.

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Committed on |
|---|---|---|---|---|---|
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/set-up | 4c65aba | feat: initial project setup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/set-up | f3715be | style: add style guidelines section | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | 1c1142c | style: add navbar styles | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | d05346a | feat: add navbar markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | 7e4bd8a | feat: add hero section markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | ab2e26d | feat: add main features hero markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | 2b23574 | feat: add segments markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | 391b735 | feat: add plans markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | be2b0e8 | feat: add features grid markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | e44e445 | feat: add faq markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | b8cf917 | feat: add footer markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | 552ebfa | style: add hamburger and mobile drawer styles | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | 1beb4e7 | refactor: reorganize styles by page section | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/index | 54ee410 | style: add index page styles | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/features | 748bcb0 | feat: add features page markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/features | 88705fc | style: add features page styles | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/about-us | 1318a66 | feat: add about us page markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/about-us | 3ed9a72 | style: add about us page styles | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/contact | 160a277 | style: add contact page styles | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/contact | 8a25e71 | feat: add contact page markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/terms | ef7e448 | feat: add terms page markup | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/terms | 1df54f1 | style: add terms page styles | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/footer | 15592db | style: add footer style | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/footer | edacad3 | style: add responsive styles | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/footer | 57f8f8a | style: add scroll snap style | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/footer | 2e708ec | feat: add i18n translations | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/footer | 9f012bb | feat: add core scripts and interactions | — | 24/04/2026 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-website | feature/footer | 240e369 | chore: add project assets | — | 24/04/2026 |

#### 5.2.1.5. Execution Evidence for Sprint Review

Durante el Sprint 1, el equipo completó la implementación y despliegue público del sitio web estático (Landing Page) de NutriSmart. Se entregaron las diez User Stories comprometidas (US-LP01–US-LP10), cubriendo la totalidad de las secciones del sitio: Hero con carrusel de tres diapositivas, sección de funciones principales con subpágina completa, tabla comparativa de planes de suscripción, módulo de internacionalización en_US / es_419 con persistencia de sesión, subpágina About Us con misión, visión y tarjetas del equipo, acordeón de preguntas frecuentes, formulario de contacto con validación del lado cliente, acceso persistente al login desde todas las páginas, sección de redes sociales y subpágina de Términos y Condiciones. El sitio fue desplegado en GitHub Pages.

A continuación se presentan screenshots de las principales vistas implementadas durante el sprint.

**Hero Section (Call to Action)**
![Hero](../assets/img/sprint1/hero.png)

**Main Features Section y enlace a subpágina completa**
![Main features](../assets/img/sprint1/main.png)

**Subscription Plans Comparison Table**
![Suscriptions](../assets/img/sprint1/suscriptions.png)

**About Us**
![About-us](../assets/img/sprint1/about-us.png)

**FAQ accordion**
![FAQ](../assets/img/sprint1/faq.png)

**Contact page con formulario y validación**
![Contact](../assets/img/sprint1/contact.png)

**Terms and Conditions subpage**
![Terms](../assets/img/sprint1/terms.png)

**Footer con redes sociales, selector de idioma y enlace legal**
![Footer](../assets/img/sprint1/footer.png)

**Cambio de idioma activo**
![Language](../assets/img/sprint1/language.png)

El video de demostración del Sprint 1 ilustra la navegación completa por todas las secciones de la Landing Page, el cambio de idioma entre inglés y español, la validación del formulario de contacto y el acceso al punto de entrada de la aplicación web desde la página de inicio.

**URL del video de demostración del Sprint 1:** [Video review sprint](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202417857_upc_edu_pe/IQAsVc-ygqmaQqOPRh7NVn1jAYeQxZXoJBe2kHvxwLfq17c?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=8FcM6m)


#### 5.2.1.6. Services Documentation Evidence for Sprint Review

El Sprint 1 tuvo como único alcance la implementación del sitio web estático (Landing Page) de NutriSmart. En esta iteración no se desarrollaron ni desplegaron Web Services, endpoints RESTful ni ningún componente de backend. Por ello, no existe documentación de servicios con OpenAPI que reportar en este sprint.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

Durante este sprint se realizó el despliegue de la landing page de NutriSmart en GitHub Pages. El proceso abarcó la configuración del repositorio remoto, la integración del flujo Gitflow con la rama `main` como fuente de despliegue, y la habilitación del servicio de hosting estático de GitHub. A continuación se describen los pasos realizados.

##### Creación del repositorio en GitHub

Se creó el repositorio público `nutrismart-website` bajo la organización `upc-pre-202610-1asi0729-17952-devteam` en GitHub. Este repositorio centraliza todo el código fuente de la landing page y sirve como base para el despliegue continuo.

##### Configuración de ramas bajo Gitflow

Se estableció la estructura de ramas siguiendo Gitflow:

- `main` > rama de producción (fuente de despliegue)
- `develop` > rama de integración
- `feature/*` > ramas de desarrollo por funcionalidad

Todo el trabajo fue integrado mediante Pull Requests desde las ramas `feature/*` hacia `develop`, y finalmente desde `develop` hacia `main` como parte del release `v1.0.0`.

##### Merge a main y creación del tag de release

Una vez completadas todas las features del sprint, se realizó el merge de `develop` a `main` mediante un Pull Request en GitHub, etiquetando el commit resultante como `v1.0.0`.

##### Configuración de GitHub Pages

Para habilitar el despliegue se siguieron los pasos:

1. Ingresar al repositorio en GitHub
2. Ir a **Settings** > **Pages**
3. En la sección **Build and deployment**, seleccionar:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Hacer click en **Save**

GitHub Pages procesó el contenido de la rama `main` y generó automáticamente la URL de despliegue.

##### URL de despliegue

La landing page quedó disponible públicamente en: [Landing Page](https://upc-pre-202610-1asi0729-17952-devteam.github.io/nutrismart-website/)

#### 5.2.1.8. Team Collaboration Insights during Sprint

Durante el Sprint, todos los miembros del equipo participaron activamente en las actividades de implementación, tal como se refleja en los analíticos de colaboración de GitHub. Como se puede observar en la gráfica de contribuciones, los integrantes Nevatrix, xJoelFMRx, olenkisha14, Emy127 y Brandon1677 realizaron commits de manera constante. Cada miembro aportó al desarrollo del Sprint.

![Insight](../assets/img/sprint1/insight.png)

### 5.2.2. Sprint 2

#### 5.2.2.1. Sprint Planning 2


<table>
  <tr>
    <th colspan="2">Sprint #</th>
    <th colspan="2">Sprint 2</th>
  </tr>
  <tr>
    <th colspan="4">Sprint Planning Background</th>
  </tr>
  <tr>
    <td colspan="2">Date</td>
    <td colspan="2">2026-04-24</td>
  </tr>
  <tr>
    <td colspan="2">Time</td>
    <td colspan="2">07:00 PM (GMT-5)</td>
  </tr>
  <tr>
    <td colspan="2">Location</td>
    <td colspan="2">Reunión virtual vía Microsoft Teams</td>
  </tr>
  <tr>
    <td colspan="2">Prepared By</td>
    <td colspan="2">Villarreal Bazan, Angel Martin</td>
  </tr>
  <tr>
    <td colspan="2">Attendees (to planning meeting)</td>
    <td colspan="2">Del Aguila Del Aguila, Olenka Priscilla / Espinoza Cruz, Angela Milagros / Mora Rivera, Joel Fernando / Soto Palacios, Brandon Wilder / Villarreal Bazan, Angel Martin</td>
  </tr>
  <tr>
    <th colspan="4">Sprint 1 Review Summary</th>
  </tr>
  <tr>
    <td colspan="4">En el Sprint 1 se entregó la Landing Page de NutriSmart en su totalidad: Hero con carrusel de tres diapositivas, sección de funciones principales con subpágina completa, tabla comparativa de planes, módulo de internacionalización en_US / es_419 con persistencia de sesión, subpágina About Us, acordeón de preguntas frecuentes, formulario de contacto con validación del lado cliente, acceso persistente al login desde todas las páginas, sección de redes sociales y subpágina de Términos y Condiciones. El sitio fue desplegado exitosamente en GitHub Pages. Las 10 User Stories comprometidas (US-LP01–US-LP10) fueron completadas al 100%, con un total de 15 Story Points entregados.</td>
  </tr>
  <tr>
    <th colspan="4">Sprint 1 Retrospective Summary</th>
  </tr>
  <tr>
    <td colspan="4">El equipo identificó como fortaleza la distribución clara de responsabilidades mediante la tabla LACX y la disciplina en el uso de Conventional Commits y GitFlow. Como área de mejora se identificó la necesidad de establecer un mock compartido desde el inicio del sprint para que todos los miembros trabajen sobre los mismos datos de prueba desde el primer día. Para el Sprint 2 se acordó: (1) crear el archivo <code>auth.mock.ts</code> con un usuario autenticado completamente poblado antes de iniciar cualquier tarea de implementación, (2) mantener reuniones de sincronización dos veces por semana para detectar bloqueos en la integración entre bounded contexts, y (3) establecer la rama <code>develop</code> como única fuente de integración antes de hacer merge a <code>main</code>.</td>
  </tr>
  <tr>
    <th colspan="4">Sprint Goal &amp; User Stories</th>
  </tr>
  <tr>
    <td colspan="2">Sprint 2 Goal</td>
    <td colspan="2">Our focus is on delivering the complete authenticated frontend of the NutriSmart web application, covering the IAM, Behavioral Consistency, Nutrition Tracking, Metabolic Adaptation, Restaurant Intelligence, Smart Recommendation, Subscriptions, and Analytics bounded contexts. We believe it delivers a functional and navigable experience that allows users to register, complete onboarding, log their daily nutrition, monitor their behavioral adherence status through the four states (ON_TRACK, AT_RISK, DROPPED, RECOVERED), receive contextual recommendations, scan food plates and restaurant menus, manage their pantry, track their body metrics with activity-based caloric adjustments via manual activity logging, and manage their subscription plan. This will be confirmed when a user can complete the full registration and onboarding flow, interact with all primary views of each bounded context using json-server mock data, observe all behavioral adherence states transitioning correctly in the dashboard, and navigate between all authenticated views without broken routes or accessibility violations.</td>
  </tr>
  <tr>
    <td colspan="2">Sprint 2 Velocity</td>
    <td colspan="2">116 Story Points</td>
  </tr>
  <tr>
    <td colspan="2">Sum of Story Points</td>
    <td colspan="2">116 Story Points</td>
  </tr>
</table>

#### 5.2.2.2. Aspect Leaders and Collaborators

El Sprint 2 abarca la construcción del frontend completo de la aplicación web autenticada de NutriSmart, siguiendo la arquitectura DDD por bounded context (`domain / application / infrastructure / presentation`). Los aspectos identificados para organizar el liderazgo y la colaboración son los siguientes:
 
**IAM:** Comprende el flujo completo de autenticación (registro con emisión de `AccountCreated`, login con `SessionStarted`, recuperación de contraseña), el onboarding de 5 pasos con Angular CDK Stepper que emite `OnboardingCompleted` y `MetabolicTargetSet`, el cierre de sesión con `SessionTerminated`, los route guards, y la vista de Perfil & Configuración con sub-paneles de datos personales, restricciones dietéticas, nivel de actividad y configuración de notificaciones por tipo de evento conductual.
 
**Behavioral Consistency & Analytics:** Comprende el dashboard principal con los cuatro estados de adherencia conductual (`ON_TRACK`, `AT_RISK`, `DROPPED`, `RECOVERED`) y sus respectivos banners reactivos vinculados a `BehavioralDropDetected`, `NutritionalAbandonmentRisk` y `ConsistencyRecovered`, el widget de racha con milestones en 7/14/21/30 días, la vista de Analytics con gráficos de historial calórico y línea de tiempo de adherencia, y la exportación de reporte PDF para usuarios Premium.
 
**Nutrition Tracking:** Comprende la búsqueda de alimentos con debounce y badges `NutritionalRiskLevel`, el Daily Log con balance diario en tiempo real y emisión de `MealRecorded` / `DailyGoalExceeded` / `DailyGoalMet`, los modales `AddFood` y `RestrictedItemBlocked`, el estado `MealSkipped` visible en cada sección de comida, los widgets de monitoreo de déficit (WEIGHT_LOSS) y proteína/superávit (MUSCLE_GAIN), el historial y análisis semanal de macros por segmento, el panel de detalle de comida por ítem.
 
**Restaurant Intelligence & Smart Scan:** Comprende la vista de selección de modo de escaneo con verificación de plan, el flujo de análisis de plato con `MealPhotoAnalyzed` y edición de ítems antes de confirmar como `MealRecord`, el escaneo de menú con `RestaurantMealAnalyzed`, la sección de platos restringidos con `RestrictedDishFlagged`, el ranking compatible con `CompatibleDishesRanked` y acción de registro directo desde la lista, y la vista de Despensa con gestión de ingredientes y sugerencias de recetas ordenadas por el macro más deficitario del día.
 
**Smart Recommendation & Metabolic Adaptation:** Comprende la vista de Recomendaciones con banner climático, tarjeta preventiva (`PreventiveRecommendationGenerated`) para AT_RISK, tarjeta de intervención (`InterventionRecommendationGenerated`) para DROPPED, tarjeta de ajuste de estrategia (`StrategyAdjustmentSuggested`), tarjeta `BestDishRecommended` con justificación de macros, y panel de Modo Viaje. También comprende la vista Body Progress con métricas BMI/BMR/TDEE, gráfico de evolución de peso, configuración de peso objetivo, sección de composición corporal para MUSCLE_GAIN, banners de `StagnationDetected` y `StrategyMismatchDetected`, y el registro manual de actividad física con estimación MET y emisión de `CaloricTargetAdjusted`.
 
| Team Member (Last Name, First Name) | GitHub Username | IAM | Behavioral Consistency & Analytics | Nutrition Tracking | Restaurant Intelligence & Smart Scan | Smart Recommendation & Metabolic Adaptation |
|-------------------------------------|-----------------|:----------------:|:-----------------------------------:|:-----------------------------------:|:-------------------------------------:|:--------------------------------------------:|
| Del Aguila Del Aguila, Olenka Priscilla | olenkisha_14 | C | C | C | L | C |
| Espinoza Cruz, Angela Milagros | Emy127 | C | C | C | C | L |
| Mora Rivera, Joel Fernando | xJoelFMRx | C | C | L | C | C |
| Soto Palacios, Brandon Wilder | Brandon1677 | C | L | C | C | C |
| Villarreal Bazan, Angel Martin | nevatrix | L | C | C | C | C |
 
#### 5.2.2.3. Sprint Backlog 2


El Sprint 2 tiene como objetivo entregar el frontend completo de la aplicación web autenticada de NutriSmart. El desarrollo cubre los bounded contexts de IAM (EP06), Behavioral Consistency (EP01), Nutrition Tracking (EP02), Metabolic Adaptation (EP03), Restaurant Intelligence (EP04), Smart Recommendation (EP05), Subscriptions (EP07), y Analytics & Reporting (EP08), siguiendo la arquitectura DDD por bounded context. Los servicios de backend se simulan mediante `json-server`. La actividad física se implementa como registro manual: el usuario especifica tipo y duración, el sistema estima calorías quemadas por tabla MET y las deduce del balance calórico diario emitiendo `CaloricTargetAdjusted`, sin depender de un dispositivo wearable externo.
 
![Board Sprint 2](../assets/img/sprint2/sprintbacklog.png)
 
URL del Board (Trello): [Enlace Trello](https://trello.com/invite/b/6a03a5352711a147e1dcddde/ATTId2ac96f1c9b394e8f4c8f3ad82fcdacb692DB4EB/sprint-backlog-2)
 
| US ID | US Title | Task ID | Task Title | Description | Est. (h) | Assigned To | Status |
|-------|----------|---------|------------|-------------|----------|-------------|--------|
| US38 | Create an Account to Gain Access to a Nutritional Plan Calibrated to My Body | T01 | Scaffold Angular project with DDD folder structure, router, and shared auth mock | Initialize the Angular project following the bounded-context folder structure (`iam/`, `behavioral-consistency/`, `nutrition-tracking/`, `metabolic-adaptation/`, `restaurant-intelligence/`, `smart-recommendation/`, `analytics/`, `subscriptions/`, `shared/`). Configure Angular Router with public and protected route groups. Integrate Angular Material with NutriSmart custom theme (#508B89). Configure `HttpClient` with `BaseApi` and `BaseApiEndpoint`. Configure `json-server` with `db.json` fixtures covering all Sprint 2 domain entities. Create `auth.mock.ts` with a fully populated authenticated user (goalType, restrictions, weight, height, plan, adherenceStatus) for use by all team members from day 1. | 5 | Villarreal Bazan, Angel Martin | Done |
| US38 | Create an Account to Gain Access to a Nutritional Plan Calibrated to My Body | T02 | Define DDD layer files for IAM bounded context | Create the `UserCredentials` and `UserProfile` domain entities. Create the `IamApi` infrastructure class extending `BaseApi` with `register()`, `login()`, `logout()`, `forgotPassword()`, and `resetPassword()` methods. Create the `IamAssembler` and the `IamStore` Angular service using Signals. | 3 | Villarreal Bazan, Angel Martin | Done |
| US38 | Create an Account to Gain Access to a Nutritional Plan Calibrated to My Body | T03 | Build registration view with AccountCreated emission | Implement the `/auth/register` view with Angular Reactive Forms for first name, last name, email, password (min 8 characters), and terms acceptance checkbox. On valid submit, call `IamStore.register()` mock, emit `AccountCreated`, and redirect to onboarding. Display Angular Material form field errors for duplicate email (409) and weak password. Apply `aria-required` and `aria-invalid` to all fields. | 4 | Villarreal Bazan, Angel Martin | Done |
| US39 | Resume My Nutritional Plan and Adherence Progress From Any Session | T04 | Build login view with SessionStarted emission and session persistence | Implement the `/auth/login` view with Angular Reactive Forms for email and password. On valid submit, call `IamStore.login()` mock, store the JWT in `localStorage`, emit `SessionStarted`, and redirect to `/dashboard` showing the current `AdherenceStatus`. Display a generic invalid credentials Angular Material error after 1 failed attempt. After 5 consecutive failures, display a lockout Angular Material Banner. | 4 | Villarreal Bazan, Angel Martin | Done |
| US40 | Recover Access to My Account and Nutritional History After Forgetting the Password | T05 | Build forgot password and reset password views | Implement the `/auth/forgot-password` view with a neutral confirmation message regardless of whether the email is registered. Implement the `/auth/reset-password` view with new password and confirm password inputs with cross-field validation. On success, redirect to `/auth/login` with a Snackbar confirmation. | 3 | Villarreal Bazan, Angel Martin | Done |
| US19 | Complete Onboarding to Generate a Nutritional Plan Calibrated to My Actual Metabolism | T06 | Build 5-step onboarding flow emitting OnboardingCompleted and MetabolicTargetSet | Implement the `/onboarding` multi-step flow using Angular CDK Stepper with 5 steps: (1) Goal — WEIGHT_LOSS or MUSCLE_GAIN cards; (2) Physical data — weight, height, birthdate, biological sex, activity level; (3) Dietary restrictions and medical conditions — tag-based multi-select; (4) Targets preview — BMI, BMR, TDEE, daily caloric target, macro distribution bars; (5) Plan selection — Basic, Pro, Premium cards. Block submission if weight, height, or biological sex are missing. On confirm, emit `OnboardingCompleted` and `MetabolicTargetSet`, then redirect to `/dashboard`. | 8 | Villarreal Bazan, Angel Martin | Done |
| US42 | Terminate the Session to Prevent Unauthorized Access to Personal Health Data | T07 | Implement logout with SessionTerminated emission and route guards | Implement the logout action that clears the JWT from `localStorage`, emits `SessionTerminated`, and redirects to `/auth/login`. Implement an Angular `AuthGuard` that redirects unauthenticated users to `/auth/login` for all protected routes. | 2 | Villarreal Bazan, Angel Martin | Done |
| US41 | Keep Nutritional Recommendations Accurate by Updating Physical Conditions and Restrictions | T08 | Build Profile & Settings view with 5 sub-panels and MetabolicTargetsRecalculated on activity update | Create the `ProfileSettings` domain entity. Extend `IamApi` with `getProfile()`, `updateProfile()`, `updateRestrictions()`, `updateGoal()`, and `updateNotificationSettings()`. Implement the `/profile` view with 5 panels: Personal information, Physical details and goals (goal toggle emits `MetabolicTargetsRecalculated` on save), Dietary restrictions with 6 notification toggles (meal skip, behavioral drop, abandonment risk, recovery, streak milestones, strategy adjustment), Language, and Security and privacy. | 7 | Villarreal Bazan, Angel Martin | Done |
| US01 | Maintain Daily Nutritional Adherence | T09 | Define DDD layer files for Behavioral Consistency bounded context | Create the `BehavioralProgress`, `AdherenceState`, and `StreakRecord` domain entities. Create the `BehavioralApi` extending `BaseApi` with `getAdherenceStatus()`, `getStreakStatus()`, and `getAdherenceHistory()`. Create `BehavioralAssembler` and `BehavioralStore` using Signals. | 3 | Soto Palacios, Brandon Wilder | Done |
| US01 | Maintain Daily Nutritional Adherence | T10 | Build Dashboard ON_TRACK state with all metric widgets | Implement the `/dashboard` view with greeting, 3 metric cards (calories consumed vs target, calories remaining, net balance), Today's log panel with 4 meal rows (Breakfast/Lunch/Snack/Dinner), Daily macros SVG donut chart with 3 macro progress bars, and Active Streak card with 7 weekly dots. Apply `aria-live="polite"` to all metric cards. | 6 | Soto Palacios, Brandon Wilder | Done |
| US02 | Receive Early Warning Before Abandoning the Plan | T11 | Build Dashboard AT_RISK state triggered by BehavioralDropDetected | Extend the `/dashboard` to display AT_RISK when `AdherenceStatus` is `AT_RISK` (3 consecutive misses). Show an orange warning banner with a See suggestion → link to `/recommendations`, missed window badges on affected meal rows, orange progress bars, orange streak card, and an ⚠ AT_RISK header badge. Toggled via demo bar button. | 3 | Soto Palacios, Brandon Wilder | Done |
| US03 | Prevent Nutritional Abandonment Through Intervention | T12 | Build Dashboard DROPPED state triggered by NutritionalAbandonmentRisk | Extend the `/dashboard` to display DROPPED when `AdherenceStatus` is `DROPPED` (7 days inactive after AT_RISK). Show a red intervention banner with a See reactivation plan → button, replace meal rows with a centered empty state block, set all metric cards to zero, and show a red streak card. Toggled via demo bar button. | 3 | Soto Palacios, Brandon Wilder | Done |
| US04 | Recover Nutritional Consistency After a Drop | T13 | Build Dashboard RECOVERED state triggered by ConsistencyRecovered | Extend the `/dashboard` to display RECOVERED when `AdherenceStatus` is `RECOVERED`. Show a green recovery banner, green streak card with count 1 and `ConsistencyRecovered` ✓ label, and a green ↩ RECOVERED · Day 1 header badge. Toggled via demo bar button. | 2 | Soto Palacios, Brandon Wilder | Done |
| US05 | Celebrate Consistency Milestones to Reinforce Habits | T14 | Build streak milestone widget with StreakMilestoneReached notification | Extend the Active Streak card to display a milestone badge at 7, 14, 21, and 30 days. Show an Angular Material Snackbar congratulating the user on each milestone. | 2 | Soto Palacios, Brandon Wilder | Done |
| US48 | Get a Complete Picture of My Nutritional and Behavioral State at a Glance | T15 | Define DDD layer files for Analytics bounded context and build Analytics view | Create `DailySummary`, `WeeklyHistory`, and `AdherenceHistory` domain entities. Create `AnalyticsApi` with `getDailySummary()`, `getWeeklyHistory()`, `getMonthlyHistory()`, `getAdherenceHistory()`, and `exportPdfReport()`. Create `AnalyticsStore` using Signals. Implement the `/analytics` view with 3-period toggle (7/30/90 days), 4 metric cards, daily calories bar chart (over-goal bars in red, on-target in teal), Avg Macros panel, weight evolution line chart, and for the 30-day period an Adherence History timeline showing ON_TRACK/AT_RISK/DROPPED/RECOVERED days in distinct colors. | 6 | Soto Palacios, Brandon Wilder | Done |
| US49 | Export Objective Evidence of Nutritional Compliance | T16 | Build PDF export button with Premium entitlement check | Implement the Export to PDF button in `/analytics`. For Premium users call `AnalyticsStore.exportPdfReport()` and trigger file download. For Basic/Pro users disable the button and show a tooltip indicating PDF Reports require a Premium plan. | 2 | Soto Palacios, Brandon Wilder | Done |
| US07 | Block Incompatible Foods Automatically to Eliminate Nutritional Risk | T17 | Define DDD layer files for Nutrition Tracking bounded context | Create `FoodItem`, `MealRecord`, and `DailyIntake` domain entities with invariants: `DailyIntake` cannot exceed the caloric limit without emitting `DailyGoalExceeded`; a `MealRecord` with a restricted ingredient must emit `RestrictedItemBlocked`. Create `NutritionApi` with `searchFoods()`, `createMealEntry()`, `getDailyLog()`, `updateMealEntry()`, `deleteMealEntry()`, and `getDailyBalance()`. Create `NutritionAssembler` and `NutritionStore` using Signals. | 3 | Mora Rivera, Joel Fernando | Done |
| US08 | Find Accurate Nutritional Data to Make Informed Food Decisions | T18 | Build food search with debounce, restriction flags, and NutritionalRiskLevel badges | Implement the food search panel within the Daily Log view with an Angular Material Input applying 400ms `debounceTime`. Display results with food name, serving size, and kcal. Flag restricted items with a ⚠ Restriction chip and the corresponding `NutritionalRiskLevel` (LOW / MEDIUM / HIGH) badge. Show empty state with a manual entry option. | 4 | Mora Rivera, Joel Fernando | Done |
| US09 | Log a Meal to Maintain an Accurate Daily Intake Record and Validate Macro Progress | T19 | Build Daily Log view with meal expansion panels, summary bar, and MealRecorded / DailyGoalExceeded states | Implement the `/nutrition/log` view with a date navigator, 5-column summary bar, and 4 Angular Material Expansion Panel meal sections. Each section shows logged items with name, quantity, macros, kcal, and remove button. Display a daily balance right panel with goal, consumed, active calories, and remaining. When a new entry causes total calories to exceed target by more than 10%, show a red Angular Material Alert identifying `DailyGoalExceeded` and the exact kcal exceeded. When all windows are logged within ±10%, show a green Angular Material Alert identifying `DailyGoalMet`. | 5 | Mora Rivera, Joel Fernando | Done |
| US07 | Block Incompatible Foods Automatically to Eliminate Nutritional Risk | T20 | Build Add Food modal with macro preview and RestrictedItemBlocked modal | Implement the Add Food Angular Material Dialog with quantity input that scales macros in real time, meal type selector, 4-cell macro preview grid, and Confirm/Cancel buttons. Implement the `RestrictedItemBlocked` Angular Material Dialog with a red top border, food name in red, conflicting restriction and `NutritionalRiskLevel`, and an Understood button. The blocked modal opens instead of the add modal when the food contains a restricted ingredient. | 4 | Mora Rivera, Joel Fernando | Done |
| US10 | Detect Meal Skips Automatically to Prevent Silent Adherence Losses | T21 | Build MealSkipped state in Daily Log meal sections | Extend each meal section to display a Missed window · `MealSkipped` orange Angular Material Chip badge in the section header when the meal window closes without any logged entry. Replace the items list with a gray italic empty state text. Activate via the MealSkipped demo state button. | 2 | Mora Rivera, Joel Fernando | Done |
| US15 | Prevent Exceeding the Caloric Deficit Limit Before It Counts as a Behavioral Miss | T22 | Build real-time caloric deficit monitoring widget for WEIGHT_LOSS users | Implement the caloric deficit widget within `/nutrition/log` for WEIGHT_LOSS users, showing remaining calories before the deficit limit with a color-coded status chip (on track / approaching limit / exceeded). Update reactively via `NutritionStore` Signals on every `MealRecorded`. | 2 | Mora Rivera, Joel Fernando | Done |
| US16 | Ensure Muscle Growth Conditions Are Met Through Daily Protein and Surplus Tracking | T23 | Build protein and caloric surplus tracker widget for MUSCLE_GAIN users | Implement the protein tracker widget within `/nutrition/log` for MUSCLE_GAIN users, showing consumed protein vs target as an Angular Material Progress Bar and an Angular Material Banner warning when protein falls below 2.0g/kg. Update reactively via Signals. | 2 | Mora Rivera, Joel Fernando | Done |
| US14 | Identify Weekly Eating Patterns That Are Sabotaging Fat Loss Consistency | T24 | Build weekly and monthly nutritional history view with deficit pattern detection | Implement the `/nutrition/history` view with a weekly summary (daily calorie total vs deficit target, days where limit was exceeded flagged in red, weekly macro averages) and monthly summary (caloric average, days within target, weekdays with highest rate of `DailyGoalExceeded`). Provide a period selector. | 3 | Mora Rivera, Joel Fernando | Done |
| US17 | Detect Recurring Macro Imbalances That Are Eroding Fat Loss Progress Over the Week | T25 | Build weekly macro analysis view for WEIGHT_LOSS users | Implement the `/nutrition/macro-analysis` view for WEIGHT_LOSS users displaying each day's caloric total against the deficit target, average daily deviation in kcal, and macro distribution breakdown flagging any day where fat or carbohydrate intake deviates more than 15% from the recommended distribution correlated with `DailyGoalExceeded` events. | 3 | Mora Rivera, Joel Fernando | Done |
| US18 | Identify Protein and Surplus Gaps That Are Blocking Weekly Muscle Synthesis | T26 | Build weekly protein and surplus analysis view for MUSCLE_GAIN users | Implement the `/nutrition/macro-analysis` view for MUSCLE_GAIN users showing protein consumed per day, days below the minimum target, overall weekly protein compliance as a percentage, and a surplus stability report identifying days where the surplus dropped below zero. | 3 | Mora Rivera, Joel Fernando | Done |
| US13 | Identify Which Specific Foods Are Breaking My Macro Balance | T27 | Build meal nutritional detail panel with per-item macro contribution | Implement the meal detail panel for a selected meal category displaying each food item with name, quantity, calories, protein, carbohydrates, and fat. Display a consolidated summary showing whether the meal alone exceeded its recommended time-slot allocation. | 2 | Mora Rivera, Joel Fernando | Done |
| US43 | Subscribe to a Plan to Unlock the Domain Features Required to Achieve My Nutritional Goals | T28 | Define DDD layer files for Subscriptions and build subscription view | Create `Subscription` and `BillingRecord` domain entities. Create `SubscriptionsApi` with `getActivePlan()`, `upgradePlan()`, `downgradePlan()`, `cancelPlan()`, and `getBillingHistory()`. Create `SubscriptionsStore` using Signals. Implement the `/subscription` view with an active plan banner, a 3-card plan comparison section (Basic, Pro, Premium), and a Payment history Angular Material Table with date, plan, amount, status badge, and PDF receipt button. | 6 | Mora Rivera, Joel Fernando | Done |
| US44 | Upgrade the Plan to Unlock Features That Remove the Barriers Preventing Full Adherence | T29 | Build upgrade confirmation dialog with BenefitsEnabled emission | Implement the Upgrade Angular Material Dialog showing newly unlocked features with green badges (e.g. Smart Scan for Pro, Restaurant Menu Analysis and Wearable Sync for Premium), prorated charge detail, Stripe card input placeholder, and a Confirm upgrade · `SubscriptionActivated → BenefitsEnabled` button. | 2 | Mora Rivera, Joel Fernando | Done |
| US45 | Downgrade the Plan Without Losing Paid Access Until the Current Billing Period Ends | T30 | Build downgrade confirmation dialog with BenefitsDisabled scheduling | Implement the Downgrade Angular Material Dialog showing features that will be lost in red, the effective date at the end of the billing cycle (access preserved until then), and a Confirm downgrade button that schedules `BenefitsDisabled`. | 2 | Mora Rivera, Joel Fernando | Done |
| US28 | Analyze a Restaurant Menu to Eliminate Nutritional Uncertainty When Eating Out | T31 | Define DDD layer files for Restaurant Intelligence bounded context | Create `MenuAnalysis`, `DishEstimate`, and `RankedDish` domain entities. Create `RestaurantApi` with `scanMenu()`, `getRankedDishes()`, and `logSelectedDish()`. Create `RestaurantAssembler` and `RestaurantStore` using Signals. | 3 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| US12 | Reduce Logging Friction by Photographing a Meal Instead of Searching Item by Item | T32 | Define DDD layer files for Smart Scan and build scan mode selection view | Create `ScanResult` and `ScannedFoodItem` domain entities. Create `SmartScanApi` with `scanFoodPlate()` and `confirmPlateScan()`. Create `SmartScanStore` using Signals. Implement the `/smart-scan` landing view with two Angular Material Cards: Scan food dish (teal, Pro/Premium) and Scan restaurant menu (Premium only, with upgrade badge). Apply plan entitlement check from `IamStore`. | 4 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| US12 | Reduce Logging Friction by Photographing a Meal Instead of Searching Item by Item | T33 | Build plate scan analyzing state and MealPhotoAnalyzed result view with MealRecord confirmation | Implement the plate scan processing state with animated spinner and Analyzing your meal... text. Implement the scan result view with an editable food items list (name, quantity input in grams, kcal, macros), total estimated kcal, a meal type selector, and a Confirm and log · `MealRecorded` → teal button that stores each item and triggers daily macro validation. Implement the invalid image state with Log manually → link. | 5 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| US28 | Analyze a Restaurant Menu to Eliminate Nutritional Uncertainty When Eating Out | T34 | Build restaurant menu scan view with RestaurantMealAnalyzed result | Implement the `/smart-scan/menu` view with photo upload, call `RestaurantStore.scanMenu()` mock on upload, emit `RestaurantMealAnalyzed`, and display identified dishes with name, estimated calories, protein, carbohydrates, and fat. Block access for Basic and Pro users with a plan upgrade prompt. Implement unreadable image state. | 4 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| US29 | Automatically Remove Unsafe Dishes From Consideration to Protect Nutritional Safety at Restaurants | T35 | Build RestrictedDishFlagged section in menu scan results | Extend the menu scan result view to display a collapsible. Restricted dishes section (red border) listing each dish that emitted `RestrictedDishFlagged`, the specific restriction triggered, and a visual indicator excluding it from the compatibility ranking. | 3 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| US30 | Get an Instant Best-Dish Recommendation to Make the Optimal Choice at a Restaurant Without Calculation | T36 | Build CompatibleDishesRanked view with best dish card and log-from-ranking action | Implement the ranked dishes view with a Best match card (teal border, Best match badge, dish name, macro-based justification identifying which daily macro deficit the dish addresses and by how many grams, Log this dish → button that creates a `MealRecord` and emits `MealRecorded`) and a ranked alternatives list. Sort by lowest caloric density for WEIGHT_LOSS and by highest protein for MUSCLE_GAIN. | 4 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| US37 | Convert Available Pantry Ingredients Into a Meal That Covers My Most Critical Macro Deficit | T37 | Define DDD layer files for Pantry and build pantry view with recipe suggestions sorted by macro deficit | Create `PantryItem` and `RecipeSuggestion` domain entities. Create `PantryApi` with `getPantryItems()`, `addPantryItem()`, `deletePantryItem()`, and `getRecipeSuggestions()`. Create `PantryStore` using Signals. Implement the `/pantry` view with ingredient list (name, category, remove button) and an Add ingredient search input. Right panel shows recipe suggestion cards with recipe name, kcal, ingredients list, macro badges, and goal-type badge, sorted by the most deficient macro (protein for MUSCLE_GAIN, lowest caloric density for WEIGHT_LOSS). Unconditionally exclude recipes containing restricted ingredients. Display empty pantry state with prompt. | 6 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| US35 | Receive Meal Suggestions That Match the Weather So My Body Gets What It Needs in Each Climate | T38 | Define DDD layer files for Smart Recommendation and build recommendations view with weather banner | Create `RecommendationSession`, `WeatherContext`, and `TravelContext` domain entities. Create `RecommendationsApi` with `getWeatherRecommendations()`, `activateTravelMode()`, `deactivateTravelMode()`, `getPreventiveRecommendation()`, `getInterventionRecommendation()`, and `getStrategyAdjustment()`. Create `RecommendationsStore` using Signals. Implement the `/recommendations` view with a weather context banner and 3 recommendation Angular Material Cards with food name, description tags, kcal, protein badge, weather badge, and + Add to log button. Implement cold weather state (blue banner) and hot weather state (orange banner) toggled via demo bar. | 5 | Espinoza Cruz, Angela Milagros | Done |
| US31 | Receive a Simple Meal Suggestion That Makes Returning to Consistency Easy After a Drop | T39 | Build AT_RISK preventive card with PreventiveRecommendationGenerated | Extend `/recommendations` to prepend an orange-bordered Angular Material Card when `AdherenceStatus` is `AT_RISK`, showing ⚠ Adherence alert badge, a meal suggestion fitting the remaining daily macros with minimal preparation effort, `PreventiveRecommendationGenerated` event label, and an orange Log this now → button. | 3 | Espinoza Cruz, Angela Milagros | Done |
| US32 | Get a Graduated Return Plan After Abandonment That Does Not Overwhelm Me With the Full Routine Immediately | T40 | Build DROPPED intervention card with InterventionRecommendationGenerated | Extend `/recommendations` to prepend a red-bordered Angular Material Card when `AdherenceStatus` is `DROPPED`, showing. Reactivation plan badge, simplified targets with reduced kcal for days 1–3 and progressive increase from day 4, `InterventionRecommendationGenerated` event label, and a red Accept simplified plan → button. | 2 | Espinoza Cruz, Angela Milagros | Done |
| US33 | Automatically Adjust My Nutritional Strategy When My Body Has Adapted and Progress Has Stalled | T41 | Build strategy adjustment card with StrategyAdjustmentSuggested and MetabolicTargetsRecalculated | Extend `/recommendations` to display a teal-bordered Angular Material Card when `StagnationDetected` is emitted, showing the proposed new caloric target and macro distribution, `StrategyAdjustmentSuggested` event label, and an Apply new strategy button that calls `RecommendationsStore.getStrategyAdjustment()` mock and emits `MetabolicTargetsRecalculated`. | 2 | Espinoza Cruz, Angela Milagros | Done |
| US36 | Stay on Track Nutritionally When Traveling Without Knowing the Local Cuisine | T42 | Build Travel Mode panel with auto-detection and local dish recommendations | Extend `/recommendations` with a Travel Mode Angular Material Slide Toggle, a detected city badge from geolocation mock, and a manual city input with confirm button. When active, replace weather recommendations with local dish cards (dish name, local cuisine tags, kcal, protein badge, Local badge, + Add to log button). Implement unrecognized city fallback. | 4 | Espinoza Cruz, Angela Milagros | Done |
| US34 | Receive a Justified Best-Dish Recommendation That Confirms My Order Is the Right Nutritional Choice | T43 | Build BestDishRecommended card with macro-based justification | Extend `/recommendations` to display a `BestDishRecommended` card sourced from `RestaurantStore` when a prior menu scan exists, showing the top-ranked dish with a justification that identifies which daily macro deficit the dish addresses most effectively and by how many grams. The card links to the full ranked dishes view. | 2 | Espinoza Cruz, Angela Milagros | Done |
| US19 | Complete Onboarding to Generate a Nutritional Plan Calibrated to My Actual Metabolism | T44 | Define DDD layer files for Metabolic Adaptation bounded context | Create `NutritionPlan`, `BodyMetric`, and `BodyComposition` domain entities with invariants: `NutritionPlan` cannot have a caloric target without defined physiological restrictions. Create `MetabolicApi` with `logWeight()`, `updateHeight()`, `getMetricsHistory()`, `setTargetWeight()`, `getMetabolicTargets()`, `updateBodyComposition()`, `logActivity()`, and `getActivityHistory()`. Create `MetabolicAssembler` and `MetabolicStore` using Signals. | 3 | Espinoza Cruz, Angela Milagros | Done |
| US22 | Understand the Metabolic Basis of My Nutritional Targets So I Can Make Informed Adjustments | T45 | Build Body Progress view with BMI/BMR/TDEE metric cards and MetabolicTargetsRecalculated on weight update | Implement the `/body-progress` view with Update height and + Log weight buttons. Display 4 metric cards (current weight with timestamp, BMI with WHO category badge, BMR in kcal/day, TDEE in kcal/day). On weight save, call `MetabolicStore.logWeight()` mock and emit `MetabolicTargetsRecalculated`. Display a 14-day staleness Angular Material Banner warning. | 5 | Espinoza Cruz, Angela Milagros | Done |
| US20 | Update Body Metrics So the Nutritional Plan Does Not Become Outdated as My Body Changes | T46 | Build weight evolution chart with period toggle, goal reference line, and log history table | Implement the weight evolution line chart within `/body-progress` with a 3-period Angular Material Button Toggle (7/30/90 days). Include a dashed pink goal weight reference line. Display a Log History Angular Material Table with the last 3 entries (date, weight, change from previous) and a View all → link. | 3 | Espinoza Cruz, Angela Milagros | Done |
| US26 | Set a Target Weight to Make Progress Measurable and Give the System a Reference for Projection | T47 | Build target weight configuration dialog with projected achievement date | Implement the target weight Angular Material Dialog with a kg input (rejects values ≥ current weight for WEIGHT_LOSS), a projected achievement date calculated from the current deficit rate in `NutritionPlan`, and Save/Cancel buttons. | 2 | Espinoza Cruz, Angela Milagros | Done |
| US27 | Verify That Weight Gain Is Muscle and Not Fat to Protect the Quality of the Bulk | T48 | Build body composition section for MUSCLE_GAIN users with StrategyAdjustmentSuggested on fat excess | Extend `/body-progress` to show a Body Composition section for MUSCLE_GAIN users displaying estimated body fat percentage, lean mass, and fat mass in kg using the U.S. Navy formula from waist and neck inputs. Display a red Angular Material Banner and emit `StrategyAdjustmentSuggested` when body fat increase exceeds 1.5% over the last two weeks. | 4 | Espinoza Cruz, Angela Milagros | Done |
| US23 | Keep My Caloric Capacity Accurate on Training Days Without Manual Recalculation | T49 | Build activity log view with MET-based calorie estimation and CaloricTargetAdjusted emission | Implement the `/activity` view with an Angular Reactive Forms entry form containing an Angular Material Select for activity type (Running, Cycling, Swimming, Weight Training, Walking, HIIT, Yoga, Other) and a duration input in minutes with positive non-zero validation. On submit, call `MetabolicStore.logActivity()` mock, estimate calories burned using a MET lookup table and user body weight, emit `CaloricTargetAdjusted` with the new net daily target, and display the deduction in a Snackbar. Update the Active calories row in the `/nutrition/log` daily balance panel reactively via Signals. Display a log history Angular Material Table with the last 5 entries (date, activity type, duration, kcal burned) and a remove button per row. Apply `aria-live="polite"` to the balance update region. | 5 | Espinoza Cruz, Angela Milagros | Done |
| US06 | Detect Strategy Mismatch to Protect Adherence | T50 | Build StrategyMismatchDetected and GradualAdjustmentSuggested banners in Body Progress | Extend `/body-progress` to display a purple Angular Material Banner when `StrategyMismatchDetected` is emitted (adherence rate below 60% after `MetabolicTargetsRecalculated`), showing the proposed softer intermediate target from `GradualAdjustmentSuggested` and an Apply gradual plan button. When adherence rate is ≥ 60%, display a green `StrategyConsistencyConfirmed` badge confirming the new targets apply directly. | 2 | Espinoza Cruz, Angela Milagros | Done |
| US25 | Force a Strategy Recalibration When My Body Has Stopped Responding to the Current Plan | T51 | Build StagnationDetected indicator in Body Progress view | Extend `/body-progress` to display a teal Angular Material Banner when `StagnationDetected` is emitted (14 days without measurable physical progress), showing the days without progress and a Go to strategy adjustment → link to the strategy card in `/recommendations`. | 2 | Espinoza Cruz, Angela Milagros | Done |
| — | Cross-cutting | T52 | Integrate ngx-translate into all Sprint 2 views and apply ARIA attributes globally | Add `en.json` and `es.json` entries for all static text in all Sprint 2 views. Wire the language selector via `LanguageSwitcher`. Apply `translate` pipe to all template text. Audit all views and apply ARIA attributes: `aria-label` on icon-only buttons, `aria-required` and `aria-invalid` on form fields, `aria-live="polite"` on dynamic metric cards and nutrition totals, `role="alert"` on error messages, `aria-expanded` on Angular Material Expansion Panels. Verify full keyboard navigation. | 4 | Villarreal Bazan, Angel Martin | Done |

#### 5.2.2.4. Development Evidence for Sprint Review


Durante este sprint, el equipo completó la implementación del frontend completo de la aplicación web autenticada de NutriSmart. El desarrollo cubrió los bounded contexts de IAM, Behavioral Consistency, Nutrition Tracking, Subscriptions, Restaurant Intelligence, Smart Scan, Pantry, Smart Recommendation y Metabolic Adaptation, incluyendo el módulo de registro manual de actividad física con emisión de `CaloricTargetAdjusted`. Todo el trabajo fue gestionado mediante GitFlow, con ramas `feature/` individuales por bounded context fusionadas en `develop` y liberadas en `main` como versión `2.0.0`.

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Committed on |
|---|---|---|---|---|---|
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/set-up | `a3f8c12` | feat: scaffold angular project with ddd folder structure | — | 2026-05-07 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/set-up | `b7d1e45` | chore: configure json-server with db.json fixtures | — | 2026-05-07 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/set-up | `c2a9f78` | chore: add shared auth mock with fully populated user | — | 2026-05-07 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/iam | `d5e3b21` | feat(iam): add user-credentials and user-profile domain entities | — | 2026-05-07 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/iam | `e8c6d54` | feat(iam): add iam-api and iam-store with signals | — | 2026-05-07 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/iam | `f1a4e87` | feat(iam): add registration view with account-created emission | — | 2026-05-07 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/iam | `g9b2c30` | feat(iam): add login view with session-started emission | — | 2026-05-07 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/iam | `h4d7f63` | feat(iam): add forgot and reset password views | — | 2026-05-08 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/iam | `i6e1a96` | feat(iam): add 5-step onboarding with onboarding-completed and metabolic-target-set | — | 2026-05-08 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/iam | `j3f8b29` | feat(iam): add auth guard and session-terminated on logout | — | 2026-05-08 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/iam | `k7c5d62` | feat(iam): add profile settings view with 5 sub-panels | — | 2026-05-08 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/behavioral-consistency | `l2a9e95` | feat(behavioral): add behavioral-progress and adherence-state domain entities | — | 2026-05-08 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/behavioral-consistency | `m8b3f28` | feat(behavioral): add behavioral-api and behavioral-store | — | 2026-05-08 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/behavioral-consistency | `n5c7a61` | feat(behavioral): add dashboard on-track state | — | 2026-05-08 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/behavioral-consistency | `o1d4e94` | feat(behavioral): add dashboard at-risk state with behavioral-drop-detected banner | — | 2026-05-08 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/behavioral-consistency | `p9e2b27` | feat(behavioral): add dashboard dropped state with nutritional-abandonment-risk banner | — | 2026-05-09 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/behavioral-consistency | `q4f6c60` | feat(behavioral): add dashboard recovered state with consistency-recovered banner | — | 2026-05-09 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/behavioral-consistency | `r6a1d93` | feat(behavioral): add streak milestone widget with streak-milestone-reached notification | — | 2026-05-09 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/analytics | `s2b8e26` | feat(analytics): add analytics-api and analytics-store | — | 2026-05-09 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/analytics | `t7c5f59` | feat(analytics): add analytics view with period selector and charts | — | 2026-05-09 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/analytics | `u3d9a92` | feat(analytics): add adherence history timeline for 30-day period | — | 2026-05-09 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/analytics | `v8e4b25` | feat(analytics): add pdf export with premium entitlement check | — | 2026-05-09 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/nutrition-tracking | `w1f2c58` | feat(nutrition-tracking): add food-item meal-record and daily-intake domain entities | — | 2026-05-09 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/nutrition-tracking | `x5a7d91` | feat(nutrition-tracking): add nutrition-api and nutrition-store | — | 2026-05-09 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/nutrition-tracking | `y9b3e24` | feat(nutrition-tracking): add food search with nutritional-risk-level flags | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/nutrition-tracking | `z4c8f57` | feat(nutrition-tracking): add daily log view with meal expansion panels | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/nutrition-tracking | `a7d5a90` | feat(nutrition-tracking): add add-food modal and restricted-item-blocked modal | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/nutrition-tracking | `b2e1b23` | feat(nutrition-tracking): add meal-skipped daily-goal-exceeded and daily-goal-met states | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/nutrition-tracking | `c6f9c56` | feat(nutrition-tracking): add caloric deficit widget for weight-loss users | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/nutrition-tracking | `d1a4d89` | feat(nutrition-tracking): add protein and surplus tracker for muscle-gain users | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/nutrition-tracking | `e8b2e22` | feat(nutrition-tracking): add weekly history and macro analysis views | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/nutrition-tracking | `f3c7f55` | feat(nutrition-tracking): add meal detail panel with per-item macro contribution | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/subscriptions | `g9d5a88` | feat(subscriptions): add subscription and billing-record domain entities | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/subscriptions | `h4e3b21` | feat(subscriptions): add subscriptions-api and subscriptions-store | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/subscriptions | `i7f1c54` | feat(subscriptions): add subscription view with plan comparison cards | — | 2026-05-10 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/subscriptions | `j2a8d87` | feat(subscriptions): add upgrade dialog with benefits-enabled emission | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/subscriptions | `k6b6e20` | feat(subscriptions): add downgrade dialog with benefits-disabled scheduling | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/restaurant-intelligence | `l1c4f53` | feat(restaurant): add menu-analysis and ranked-dish domain entities | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/restaurant-intelligence | `m5d2a86` | feat(restaurant): add restaurant-api and restaurant-store | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/restaurant-intelligence | `n9e9b19` | feat(restaurant): add menu scan view with restaurant-meal-analyzed result | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/restaurant-intelligence | `o3f7c52` | feat(restaurant): add restricted-dish-flagged section | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/restaurant-intelligence | `p8a5d85` | feat(restaurant): add compatible-dishes-ranked view with log-from-ranking action | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-scan | `q2b3e18` | feat(smart-scan): add scan-result domain entities and smart-scan-api | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-scan | `r7c1f51` | feat(smart-scan): add scan mode selection view with plan entitlement check | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-scan | `s4d8a84` | feat(smart-scan): add plate scan result view with meal-recorded confirmation | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-recommendation | `t6e6b17` | feat(recommendations): add recommendation-session and travel-context domain entities | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-recommendation | `u1f4c50` | feat(recommendations): add recommendations-api and recommendations-store | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-recommendation | `v5a2d83` | feat(recommendations): add recommendations view with weather context banner | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-recommendation | `w9b9e16` | feat(recommendations): add at-risk preventive card with preventive-recommendation-generated | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-recommendation | `x3c7f49` | feat(recommendations): add dropped intervention card with intervention-recommendation-generated | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-recommendation | `y8d5a82` | feat(recommendations): add strategy-adjustment-suggested card | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-recommendation | `z2e3b15` | feat(recommendations): add travel mode panel with local dish suggestions | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-recommendation | `a7f1c48` | feat(recommendations): add best-dish-recommended card with macro justification | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-recommendation | `b4a8d81` | feat(pantry): add pantry domain entities and pantry-api | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/smart-recommendation | `c9b6e14` | feat(pantry): add pantry view with ingredient list and recipe suggestions | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/metabolic-adaptation | `d1c4f47` | feat(metabolic): add nutrition-plan body-metric and body-composition domain entities | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/metabolic-adaptation | `e6d2a80` | feat(metabolic): add metabolic-api and metabolic-store | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/metabolic-adaptation | `f3e9b13` | feat(metabolic): add body progress view with bmi bmr tdee metric cards | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/metabolic-adaptation | `g8f7c46` | feat(metabolic): add weight evolution chart with goal reference line | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/metabolic-adaptation | `h2a5d79` | feat(metabolic): add target weight dialog with projected achievement date | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/metabolic-adaptation | `i7b3e12` | feat(metabolic): add body composition section with strategy-adjustment-suggested on fat excess | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/metabolic-adaptation | `j4c1f45` | feat(metabolic): add activity log view with met-based calorie estimation | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/metabolic-adaptation | `k9d8a78` | feat(metabolic): emit caloric-target-adjusted and wire to daily log balance | — | 2026-05-11 |
| upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp | feature/metabolic-adaptation | `l5e6b11` | feat(metabolic): add stagnation-detected and strategy-mismatch-detected banners | — | 2026-05-11 |

#### 5.2.2.5. Execution Evidence for Sprint Review


Durante el Sprint 2, el equipo completó la implementación del frontend completo de la aplicación web autenticada de NutriSmart, cubriendo los bounded contexts de IAM, Behavioral Consistency, Nutrition Tracking, Subscriptions, Restaurant Intelligence, Smart Scan, Pantry, Smart Recommendation y Metabolic Adaptation. La aplicación consume una capa de servicios mock mediante `json-server`, presenta navegación completa entre todas las vistas autenticadas, formularios validados con Angular Reactive Forms, internacionalización activa mediante `ngx-translate`, estado reactivo gestionado con Angular Signals, y atributos ARIA en todos los componentes interactivos. El módulo de actividad física registra manualmente tipo y duración, estima calorías quemadas por tabla MET, emite `CaloricTargetAdjusted`, y actualiza el balance calórico del Daily Log en tiempo real.
 
A continuación se presentan screenshots de las principales vistas implementadas durante el sprint.
 **Registro, login y onboarding**

![Registration view](../assets/img/sprint2/register.png)
![Onboarding step 2 — physical data](../assets/img/sprint2/onboarding-physical-data.png)
![Onboarding step 4 — targets preview with BMI, BMR, TDEE and macro distribution](../assets/img/sprint2/onboarding-targets-preview.png)

**Dashboard**

![Dashboard ON_TRACK state](../assets/img/sprint2/dashboard-on-track.png)

**Nutrition Tracking — Daily Log, análisis semanal y bloqueo de restricciones**

![Daily log view with meal expansion panels and 5-column summary bar](../assets/img/sprint2/daily-log.png)
![RestrictedItemBlocked modal with NutritionalRiskLevel indicator](../assets/img/sprint2/restricted-item-blocked.png)
![DailyGoalMet alert banner](../assets/img/sprint2/daily-goal-met.png)
![Meal detail panel with per-item macro contribution](../assets/img/sprint2/meal-detail-panel.png)

**Restaurant Intelligence y Smart Scan**

![Plate scan result — editable food items list with MealRecorded confirmation](../assets/img/sprint2/plate-scan-result.png)
![RestrictedDishFlagged section in menu scan results](../assets/img/sprint2/restricted-dish-flagged.png)

**Smart Recommendation y Pantry**

![Recommendations view](../assets/img/sprint2/recommendations-hot-weather.png)
![Pantry view](../assets/img/sprint2/pantry.png)

**Metabolic Adaptation y actividad física**

![Body Progress view with BMI BMR TDEE metric cards](../assets/img/sprint2/body-progress.png)

**Analytics y Suscripciones**

![Analytics view](../assets/img/sprint2/analytics.png)
![Suscription](../assets/img/sprint2/upgrade-dialog.png)
 
El video de demostración del Sprint 2 ilustra la navegación completa por todos los bounded contexts, la transición entre los cuatro estados de adherencia conductual del dashboard, el flujo de escaneo de plato y menú de restaurante con selección y log del plato compatible, el registro manual de actividad física con deducción en tiempo real en el balance calórico, y la gestión de suscripciones con upgrade de plan.
 
**URL del video de demostración del Sprint 2:** [Video sprint 2](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202417857_upc_edu_pe/IQDLiegjIZsTQq6qG8EwJNFBATiDuurOIn-XejaMJAToBnc?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=vafcFN)

#### 5.2.2.6. Services Documentation Evidence for Sprint Review

El Sprint 2 tuvo como alcance exclusivo la construcción del frontend de la aplicación web autenticada. Todos los datos son servidos mediante una capa mock con `json-server` a partir del archivo `db.json`, sin conexión a endpoints reales de backend. Por esta razón, no se generó documentación OpenAPI ni se desplegaron Web Services durante esta iteración.
 
La especificación completa de los endpoints RESTful que el frontend consumirá en producción se encuentra documentada en las Technical Stories TS01–TS10 del Product Backlog del Capítulo III. Su implementación está planificada para el Sprint 3 dentro del repositorio `nutrismart-platform`, cubriendo: IAM y sesiones (TS01, TS02), Behavioral Consistency (TS04), Nutrition Tracking con validación de restricciones (TS03), Metabolic Adaptation con wearable sync (TS05), Restaurant Intelligence (TS06), Smart Recommendation con pantry (TS07), Analytics & Reporting con exportación PDF (TS08), Subscriptions (TS09), y Smart Scan con health check (TS10).

#### 5.2.2.7. Software Deployment Evidence for Sprint Review

Durante este sprint se realizó el despliegue de la aplicación web autenticada de NutriSmart en Coolify, utilizando el repositorio `nutrismart-webapp` como fuente de despliegue continuo y el dominio propio `app-smart.nutriproject.xyz` como punto de acceso público. A continuación se describen los pasos realizados.

##### Creación del repositorio en GitHub

Se creó el repositorio público `nutrismart-webapp` bajo la organización `upc-pre-202610-1asi0729-17952-devteam` en GitHub. Este repositorio centraliza el código fuente del frontend Angular y sirve como base para el despliegue continuo desde Coolify.

[Link del repositorio nutrismart-webapp](https://github.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-webapp)

##### Configuración de ramas bajo Gitflow

Se estableció la estructura de ramas siguiendo Gitflow:

- `main` → rama de producción (fuente de despliegue)
- `develop` → rama de integración
- `feature/*` → ramas de desarrollo por bounded context

Todo el trabajo fue integrado mediante Pull Requests desde las ramas `feature/*` hacia `develop`, y finalmente desde `develop` hacia `main` como parte del release `v2.0.0`.

##### Merge a main y creación del tag de release

Una vez completadas todas las features del sprint, se realizó el merge de `develop` a `main` mediante un Pull Request en GitHub, etiquetando el commit resultante como `v2.0.0`.

##### Configuración del despliegue en Coolify

Para habilitar el despliegue continuo desde el repositorio se siguieron los pasos:

1. Ingresar al panel de administración de Coolify
2. Crear una nueva aplicación seleccionando **GitHub** como fuente
3. Conectar el repositorio `nutrismart-webapp` de la organización `upc-pre-202610-1asi0729-17952-devteam`
4. Configurar los parámetros de build:
   - **Build command:** `npm run build`
   - **Output directory:** `dist/nutrismart-webapp`
   - **Branch:** `main`
5. Asignar el dominio personalizado `app-smart.nutriproject.xyz` en la sección **Domains**
6. Guardar la configuración y ejecutar el primer despliegue manual

Coolify procesó el contenido de la rama `main`, ejecutó el build de Angular, y sirvió los artefactos estáticos generados bajo el dominio configurado.

##### URL de despliegue

La aplicación web quedó disponible públicamente en: [NutriSmart Web App](https://app-smart.nutriproject.xyz/)

#### 5.2.2.8. Team Collaboration Insights during Sprint

Durante el Sprint 2, todos los miembros del equipo participaron activamente en las actividades de implementación, tal como se refleja en los analíticos de colaboración de GitHub. Como se puede observar en la gráfica de contribuciones, los integrantes Nevatrix, xJoelFMRx, olenkisha14, Emy127 y Brandon1677 realizaron commits de manera constante a lo largo del sprint, cada uno liderando su bounded context asignado y colaborando en los aspectos transversales de i18n y accesibilidad.

![Insight](../assets/img/sprint2/insight.png)

### 5.2.3. Sprint 3

#### 5.2.3.1. Sprint Planning 3

<table>
  <tr>
    <th colspan="2">Sprint #</th>
    <th colspan="2">Sprint 3</th>
  </tr>
  <tr>
    <th colspan="4">Sprint Planning Background</th>
  </tr>
  <tr>
    <td colspan="2">Date</td>
    <td colspan="2">2026-06-09</td>
  </tr>
  <tr>
    <td colspan="2">Time</td>
    <td colspan="2">07:00 PM (GMT-5)</td>
  </tr>
  <tr>
    <td colspan="2">Location</td>
    <td colspan="2">Reunión virtual vía Microsoft Teams</td>
  </tr>
  <tr>
    <td colspan="2">Prepared By</td>
    <td colspan="2">Villarreal Bazan, Angel Martin</td>
  </tr>
  <tr>
    <td colspan="2">Attendees (to planning meeting)</td>
    <td colspan="2">Del Aguila Del Aguila, Olenka Priscilla / Espinoza Cruz, Angela Milagros / Mora Rivera, Joel Fernando / Soto Palacios, Brandon Wilder / Villarreal Bazan, Angel Martin</td>
  </tr>
  <tr>
    <th colspan="4">Sprint 2 Review Summary</th>
  </tr>
  <tr>
    <td colspan="4">En el Sprint 2 se entregó el frontend completo de la aplicación web autenticada de NutriSmart, cubriendo los bounded contexts de IAM, Behavioral Consistency, Nutrition Tracking, Subscriptions, Restaurant Intelligence, Smart Scan, Pantry, Smart Recommendation y Metabolic Adaptation. Todas las vistas fueron implementadas con Angular Material, ngx-translate, Angular Signals y datos mock servidos mediante json-server. La aplicación fue desplegada exitosamente en Coolify bajo el dominio app-smart.nutriproject.xyz. Las 52 tasks comprometidas fueron completadas al 100%, con un total de 116 Story Points entregados.</td>
  </tr>
  <tr>
    <th colspan="4">Sprint 2 Retrospective Summary</th>
  </tr>
  <tr>
    <td colspan="4">El equipo identificó como fortaleza la organización por bounded context con liderazgo claro mediante la matriz LACX, así como el uso disciplinado de GitFlow y Conventional Commits. Como área de mejora se identificó la necesidad de establecer los contratos de API (endpoints, request/response shapes) antes de iniciar la implementación, de modo que frontend y backend puedan avanzar en paralelo sin bloqueos. Para el Sprint 3 se acordó: (1) definir los endpoints RESTful de cada bounded context en la primera semana usando springdoc-openapi como contrato vivo, (2) mantener reuniones de sincronización tres veces por semana dado el mayor nivel de integración entre capas, (3) establecer datos de seeder deterministas para que todos los miembros trabajen sobre el mismo estado de base de datos desde el primer día, y (4) no implementar integración con Stripe ni con wearables/Health API en este sprint, postergando dichas integraciones para el Sprint 4.</td>
  </tr>
  <tr>
    <th colspan="4">Sprint Goal &amp; User Stories</th>
  </tr>
  <tr>
    <td colspan="2">Sprint 3 Goal</td>
    <td colspan="2">Our focus is on delivering the complete backend platform of NutriSmart, covering the IAM, Behavioral Consistency, Nutrition Tracking, Metabolic Adaptation, Restaurant Intelligence, Smart Recommendation, Subscriptions, and Analytics bounded contexts, documented with OpenAPI and deployed to production. We believe it delivers a fully functional RESTful API that allows the frontend and future mobile clients to authenticate users, persist nutritional logs, manage subscription plans, analyze behavioral adherence, generate restaurant menu rankings, and provide contextual recommendations, all without requiring Stripe payment processing or wearable device integration. This will be confirmed when all documented endpoints return the correct HTTP status codes and response bodies when exercised through Swagger UI deployed at smart-api.nutriproject.xyz, and the frontend running at app-smart.nutriproject.xyz successfully consumes real backend data instead of json-server mocks.</td>
  </tr>
  <tr>
    <td colspan="2">Sprint 3 Velocity</td>
    <td colspan="2">130 Story Points</td>
  </tr>
  <tr>
    <td colspan="2">Sum of Story Points</td>
    <td colspan="2">130 Story Points</td>
  </tr>
</table>

#### 5.2.3.2. Aspect Leaders and Collaborators

El Sprint 3 abarca la construcción del backend completo de la plataforma NutriSmart, siguiendo la arquitectura DDD por bounded context (`domain / application / infrastructure / interfaces`). Los aspectos identificados para organizar el liderazgo y la colaboración son los siguientes:

**IAM & Subscriptions:** Comprende el bounded context de Identity and Access Management con los agregados `User` y `PasswordResetToken`, los servicios `AuthCommandService`, `UserCommandService` y `UserQueryService`, la capa de persistencia JPA, el adaptador Gmail para envío de correos de recuperación de contraseña, los controladores `AuthController` y `UsersController` documentados con `@Tag` y `@Operation`, y el seeder de usuarios. También comprende el bounded context de Subscriptions con los agregados `Subscription` y `BillingRecord`, sus servicios de comando y consulta, la capa de persistencia JPA y los controladores `SubscriptionsController` y `BillingHistoryController`. No incluye integración con Stripe ni procesamiento real de pagos.

**Behavioral Consistency:** Comprende el bounded context con los agregados `BehavioralProgress`, `EatingBehaviorPattern` y `RecoveryPlan`, sus respectivos servicios de comando y consulta, la capa de persistencia JPA con mappers y adapters, y los controladores `BehavioralProgressController`, `EatingBehaviorPatternsController` y `RecoveryPlansController` documentados con OpenAPI. Incluye el seeder de datos conductuales para los cuatro estados de adherencia.

**Nutrition Tracking:** Comprende el bounded context con los agregados de registro nutricional diario, sus servicios de comando y consulta, la capa de persistencia JPA y los controladores RESTful documentados con OpenAPI para búsqueda de alimentos, registro de comidas y consulta de balance diario.

**Restaurant Intelligence & Smart Recommendation:** Comprende el bounded context de Restaurant Intelligence con el análisis de menús mediante IA (DeepSeek), el ranking de platos compatibles, la detección de platos restringidos y los controladores correspondientes. También comprende el bounded context de Smart Recommendation con el servicio de recomendaciones contextuales (clima via OpenWeatherMap, estados AT_RISK/DROPPED) y su capa de persistencia y controladores REST.

**Metabolic Adaptation & Analytics:** Comprende el bounded context de Metabolic Adaptation con las métricas corporales (BMI, BMR, TDEE), el historial de peso, el registro manual de actividad física con estimación MET y los controladores RESTful. También comprende el bounded context de Analytics con el resumen diario, historial semanal y mensual, la línea de tiempo de adherencia y la exportación de reportes PDF para usuarios Premium.

| Team Member (Last Name, First Name) | GitHub Username | IAM & Subscriptions & SmartRecommendation | Behavioral Consistency | Nutrition Tracking | Restaurant Intelligence & Analytics | Metabolic Adaptation |
|-------------------------------------|-----------------|:-------------------:|:----------------------:|:------------------:|:----------------------------------------------:|:--------------------------------:|
| Del Aguila Del Aguila, Olenka Priscilla | olenkisha_14 | C | C | C | C | L |
| Espinoza Cruz, Angela Milagros | Emy127 | C | C | C | L | C |
| Mora Rivera, Joel Fernando | xJoelFMRx | C | L | C | C | C |
| Soto Palacios, Brandon Wilder | Brandon1677 | C | C | L | C | C |
| Villarreal Bazan, Angel Martin | nevatrix | L | C | C | C | C |

#### 5.2.3.3. Sprint Backlog 3

El Sprint 3 tiene como objetivo entregar el backend completo de la plataforma NutriSmart. El desarrollo cubre los bounded contexts de IAM (TS01), Nutrition Tracking — Food Catalog (TS02), Nutrition Tracking — Meal Log y Balance Diario (TS03), Nutrition Tracking — Smart Scan (TS04), Restaurant Intelligence (TS05), Metabolic Adaptation (TS06), Behavioral Consistency (TS07), Smart Recommendation (TS08), Subscriptions (TS09) y Analytics (TS10), siguiendo la arquitectura DDD por bounded context con capas `domain`, `application`, `infrastructure` e `interfaces`. La integración con Stripe, wearables y Google Health API queda fuera del alcance de este sprint. Todos los endpoints son documentados con springdoc-openapi 3.0.2 y Swagger UI.

![Board Sprint 3](../assets/img/sprint3/sprintbacklog.png)

URL del Board (Trello): [Enlace Trello Sprint 3](https://trello.com/invite/b/6a324d0a407108191564f8e5/ATTIe781d1b527b8ef53d1540aacdf84146d5982BED7/sprint-backlog-3)

| US ID | US Title | Task ID | Task Title | Description | Est. (h) | Assigned To | Status |
|-------|----------|---------|------------|-------------|----------|-------------|--------|
| TS01 | API: IAM — Authentication and User Management Endpoints | T01 | Scaffold Spring Boot project con DDD folder structure, OpenAPI config y JWT Security | Inicializar el proyecto Spring Boot 3 con Java 21, configurar la estructura de paquetes por bounded context, integrar springdoc-openapi 3.0.2 con SecurityScheme JWT, configurar `OpenApiConfiguration` con servidores local y producción, configurar CORS para el dominio del frontend, y configurar el filtro JWT para validación de tokens en cada request. | 4 | Villarreal Bazan, Angel Martin | Done |
| TS01 | API: IAM — Authentication and User Management Endpoints | T02 | Implementar dominio IAM: agregados, value objects, repositorios y excepciones | Crear los value objects `EmailAddress`, `ActivityLevel`, `UserGoal`, `UserPlan` y `DietaryRestriction`. Crear los agregados `User` y `PasswordResetToken` con sus invariantes de negocio. Crear las excepciones de dominio y los puertos de repositorio `UserRepository` y `PasswordResetTokenRepository`. | 5 | Villarreal Bazan, Angel Martin | Done |
| TS01 | API: IAM — Authentication and User Management Endpoints | T03 | Implementar servicios de aplicación y capa de persistencia IAM | Implementar `AuthCommandService` (registro, login, logout), `UserCommandService` (actualizar perfil, eliminar cuenta, submit onboarding), `UserQueryService` (buscar por ID, por email, listar todos) y `PasswordResetCommandService`. Crear las entidades JPA `UserJpaEntity` y `PasswordResetTokenJpaEntity`, los repositorios Spring Data, los adaptadores de persistencia y el adaptador de email Gmail. | 7 | Villarreal Bazan, Angel Martin | Done |
| TS01 | API: IAM — Authentication and User Management Endpoints | T04 | Implementar REST controllers IAM, seeder y documentación OpenAPI | Implementar `AuthController` con endpoints `POST /api/v1/auth/login`, `POST /api/v1/auth/register`, `POST /api/v1/auth/forgot-password`, `POST /api/v1/auth/reset-password` y `GET /api/v1/auth/check-email`. Implementar `UsersController` con endpoints CRUD de usuario. Documentar con `@Tag`, `@Operation` y `@ApiResponse`. Implementar seeder de usuarios determinista (un usuario WEIGHT_LOSS Basic, uno MUSCLE_GAIN Pro, uno Premium). | 5 | Villarreal Bazan, Angel Martin | Done |
| TS02 | API: Nutrition Tracking — Food Catalog Endpoints | T05 | Implementar dominio Food Catalog: agregados, value objects y repositorios | Crear el agregado `FoodItem` con sus atributos nutricionales (caloriesPer100g, proteinPer100g, carbsPer100g, fatPer100g), value objects `ItemType`, `WeatherType` y `DietaryRestriction`, el puerto `FoodItemRepository` y las excepciones de dominio correspondientes. | 3 | Soto Palacios, Brandon Wilder | Done |
| TS02 | API: Nutrition Tracking — Food Catalog Endpoints | T06 | Implementar servicios de aplicación Food Catalog: command y query services | Implementar `FoodItemCommandService` (crear, actualizar, eliminar food item) y `FoodItemQueryService` (listar todos, filtrar por itemType, buscar por ID). Garantizar que los filtros por `itemType` y `weatherType` sean aplicados en la capa de consulta. | 4 | Soto Palacios, Brandon Wilder | Done |
| TS02 | API: Nutrition Tracking — Food Catalog Endpoints | T07 | Implementar capa de persistencia y REST controller Food Catalog con documentación OpenAPI | Crear la entidad JPA `FoodItemJpaEntity`, el mapper de persistencia, el repositorio Spring Data y el adaptador de persistencia. Implementar el controlador REST con los endpoints `GET /api/v1/foods`, `POST /api/v1/foods`, `PUT /api/v1/foods/{id}` y `DELETE /api/v1/foods/{id}`. Documentar con `@Tag`, `@Operation` y `@ApiResponse`. | 4 | Soto Palacios, Brandon Wilder | Done |
| TS03 | API: Nutrition Tracking — Meal Log, Daily Balance, and Daily Intake Endpoints | T08 | Implementar dominio Meal Log y Daily Balance: agregados, value objects y puertos | Crear los agregados `MealRecord` y `DailyBalance` con sus invariantes de negocio, value objects `MealType` y `NutrientUnit`, los puertos de repositorio `MealRecordRepository` y `DailyBalanceRepository`, y las excepciones de dominio incluyendo la de registro duplicado para `DailyIntake`. | 4 | Soto Palacios, Brandon Wilder | Done |
| TS03 | API: Nutrition Tracking — Meal Log, Daily Balance, and Daily Intake Endpoints | T09 | Implementar servicios de aplicación Meal Log y Daily Balance: command y query services | Implementar `MealRecordCommandService` (registrar, actualizar y eliminar comida) y `MealRecordQueryService` (listar por userId y fecha). Implementar `DailyBalanceQueryService` (consultar balance diario por usuario). Implementar `DailyIntakeCommandService` con validación de unicidad por userId y fecha (responde 409 ante duplicado). | 5 | Soto Palacios, Brandon Wilder | Done |
| TS03 | API: Nutrition Tracking — Meal Log, Daily Balance, and Daily Intake Endpoints | T10 | Implementar capa de persistencia y REST controllers Meal Log, Daily Balance e Daily Intake con documentación OpenAPI | Crear entidades JPA, mappers y adaptadores de persistencia para `MealRecord`, `DailyBalance` y `DailyIntake`. Implementar los controladores REST con los endpoints `GET /api/v1/nutrition-log`, `POST /api/v1/nutrition-log`, `PUT /api/v1/nutrition-log/{id}`, `DELETE /api/v1/nutrition-log/{id}`, `GET /api/v1/daily-balance`, `GET /api/v1/daily-intake`, `GET /api/v1/daily-intake/{id}`, `POST /api/v1/daily-intake` y `PUT /api/v1/daily-intake/{id}`, documentados con `@Tag`, `@Operation` y `@ApiResponse`. | 5 | Soto Palacios, Brandon Wilder | Done |
| TS04 | API: Nutrition Tracking — Smart Scan Plate Analysis Endpoints | T11 | Implementar dominio Smart Scan: agregados, value objects, puertos y restricción de plan | Crear el agregado `PlateAnalysis` con su colección de `DetectedFoodItem` (incluyendo los campos `foodItemId` nullable, `isEstimate` y macronutrientes estimados). Crear el puerto `PlateAnalysisRepository` y el port de servicio externo `PlateAnalysisAIPort`. Modelar la excepción de dominio para acceso restringido a planes Basic. | 3 | Soto Palacios, Brandon Wilder | Done |
| TS04 | API: Nutrition Tracking — Smart Scan Plate Analysis Endpoints | T12 | Implementar servicio de aplicación Smart Scan con adaptador DeepSeek/Gemini | Implementar `PlateAnalysisCommandService` que recibe una imagen en Base64, la envía al adaptador externo (DeepSeek/Gemini) para análisis y retorna los ítems detectados con sus estimaciones de macronutrientes. Implementar `PlateAnalysisConfirmCommandService` que persiste los ítems confirmados como `MealRecord` y retorna el conteo de registros creados. | 5 | Soto Palacios, Brandon Wilder | Done |
| TS04 | API: Nutrition Tracking — Smart Scan Plate Analysis Endpoints | T13 | Implementar capa de persistencia y REST controllers Smart Scan con validación de plan y documentación OpenAPI | Crear entidades JPA, mappers y adaptadores de persistencia para `PlateAnalysis`. Implementar el controlador REST con los endpoints `POST /api/v1/nutrition-log/smart-scan/plate` (retorna ítems detectados, requiere plan Pro o Premium) y `POST /api/v1/nutrition-log/smart-scan/plate/confirm` (persiste ítems y retorna count). Documentar con `@Tag`, `@Operation` y `@ApiResponse`. | 4 | Soto Palacios, Brandon Wilder | Done |
| TS05 | API: Restaurant Intelligence — Menu Scan Endpoint | T14 | Implementar dominio Restaurant Intelligence: agregados, value objects y puertos | Crear los agregados `MenuAnalysis`, `DishEstimate` y `RankedDish` con sus invariantes. Modelar los value objects `CompatibilityScore`, `ConflictingRestriction` y `MatchedFoodItemId` (nullable). Crear el puerto `MenuAnalysisRepository` y el port de servicio externo `MenuAnalysisAIPort`. | 3 | Espinoza Cruz, Angela Milagros | Done |
| TS05 | API: Restaurant Intelligence — Menu Scan Endpoint | T15 | Implementar servicios de aplicación Restaurant Intelligence con adaptador DeepSeek | Implementar `MenuAnalysisCommandService` que recibe una imagen en Base64, la reenvía al adaptador DeepSeek para identificación de platos y generación de ranking por compatibilidad nutricional con restricciones y metas del usuario autenticado. Implementar la lógica de reducción de `compatibilityScore` para platos con `conflictingRestrictions`. | 6 | Espinoza Cruz, Angela Milagros | Done |
| TS05 | API: Restaurant Intelligence — Menu Scan Endpoint | T16 | Implementar capa de persistencia y REST controller Restaurant Intelligence con validación de plan y documentación OpenAPI | Crear entidades JPA, mappers y adaptadores de persistencia para `MenuAnalysis` y `RankedDish`. Implementar el controlador REST con el endpoint `POST /api/v1/restaurant-intelligence/menu-scan` restringido a planes Pro y Premium, retornando los platos rankeados con `rank`, `dishName`, `compatibilityScore`, `conflictingRestrictions` y `scannedAt`. Documentar con `@Tag`, `@Operation` y `@ApiResponse`. | 5 | Espinoza Cruz, Angela Milagros | Done |
| TS06 | API: Metabolic Adaptation — Body Metrics, Body Composition, Activity Logs, and Metabolic Adaptation Log Endpoints | T17 | Implementar dominio Metabolic Adaptation: agregados, value objects y puertos | Crear los agregados `BodyMetric` (con `weightKg`, `heightCm`, `targetWeightKg` y `projectedAchievementDate`), `BodyComposition` (con fórmula Navy para `calculatedBodyFatPercent` y campo `overrideBodyFatPercent`), `ActivityLog` y `WearableConnection` con sus invariantes. Crear los puertos de repositorio y las excepciones de dominio. | 4 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| TS06 | API: Metabolic Adaptation — Body Metrics, Body Composition, Activity Logs, and Metabolic Adaptation Log Endpoints | T18 | Implementar servicios de aplicación Metabolic Adaptation: command y query services | Implementar `BodyMetricCommandService` (registrar peso, actualizar altura, configurar peso objetivo con proyección de logro) y `BodyMetricQueryService` (historial de peso por userId). Implementar `BodyCompositionCommandService` (calcular body fat con fórmula Navy). Implementar `ActivityLogCommandService` (registro manual con estimación MET y calorías quemadas) y `ActivityLogQueryService`. | 5 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| TS06 | API: Metabolic Adaptation — Body Metrics, Body Composition, Activity Logs, and Metabolic Adaptation Log Endpoints | T19 | Implementar capa de persistencia Metabolic Adaptation con JPA | Crear entidades JPA, mappers y adaptadores de persistencia para `BodyMetric`, `BodyComposition`, `ActivityLog`, `WearableConnection` y `MetabolicAdaptationLog`. Verificar que la columna `projectedAchievementDate` se calcule y persista correctamente en el adaptador. | 4 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| TS06 | API: Metabolic Adaptation — Body Metrics, Body Composition, Activity Logs, and Metabolic Adaptation Log Endpoints | T20 | Implementar REST controllers Metabolic Adaptation con documentación OpenAPI | Implementar los controladores REST con los endpoints `GET /api/v1/body-metrics`, `POST /api/v1/body-metrics`, `PUT /api/v1/body-metrics/{id}`, `GET /api/v1/body-compositions`, `POST /api/v1/body-compositions`, `PUT /api/v1/body-compositions/{id}`, `GET /api/v1/activity-logs`, `POST /api/v1/activity-logs`, `GET /api/v1/activity-logs/{id}`, `DELETE /api/v1/activity-logs/{id}`, `GET /api/v1/metabolic-adaptation-logs` y `POST /api/v1/metabolic-adaptation-logs`, todos documentados con `@Tag`, `@Operation` y `@ApiResponse`. | 5 | Del Aguila Del Aguila, Olenka Priscilla | Done |
| TS07 | API: Behavioral Consistency — Behavioral Progress, Eating Behavior Patterns, and Recovery Plans Endpoints | T21 | Implementar dominio Behavioral Consistency: agregados, value objects y puertos | Crear los value objects y enumeraciones `AdherenceStatus` (ON_TRACK/AT_RISK/DROPPED/RECOVERED). Crear los agregados `BehavioralProgress` (con `streak`, `consecutiveMisses`, `weeklyCompletionRate` y `goalMetDates`), `EatingBehaviorPattern` y `RecoveryPlan` (con `isActive`, `targetBehavior`, `simplifiedCalorieTarget`, `checkInDays`) con sus invariantes. Crear los puertos de repositorio y las excepciones de dominio. | 4 | Mora Rivera, Joel Fernando | Done |
| TS07 | API: Behavioral Consistency — Behavioral Progress, Eating Behavior Patterns, and Recovery Plans Endpoints | T22 | Implementar servicios de aplicación Behavioral Consistency: command y query services | Implementar los servicios de comando y consulta para `BehavioralProgress` (inicialización, actualización de streak y weeklyCompletionRate), `EatingBehaviorPattern` (crear y actualizar) y `RecoveryPlan` (crear, actualizar y eliminar). Garantizar que la transición de estados de adherencia siga las reglas de negocio del dominio. | 5 | Mora Rivera, Joel Fernando | Done |
| TS07 | API: Behavioral Consistency — Behavioral Progress, Eating Behavior Patterns, and Recovery Plans Endpoints | T23 | Implementar capa de persistencia Behavioral Consistency con JPA | Crear entidades JPA para los tres agregados del bounded context. Implementar mappers de persistencia, repositorios Spring Data y adaptadores de persistencia. Verificar que los conversores de `AdherenceStatus` sean aplicados correctamente en las entidades JPA. | 4 | Mora Rivera, Joel Fernando | Done |
| TS07 | API: Behavioral Consistency — Behavioral Progress, Eating Behavior Patterns, and Recovery Plans Endpoints | T24 | Implementar REST controllers Behavioral Consistency con documentación OpenAPI | Implementar `BehavioralProgressController`, `EatingBehaviorPatternsController` y `RecoveryPlansController` con sus recursos (DTOs), assemblers y documentación `@Tag`, `@Operation`, `@ApiResponse`. Cubrir los endpoints `GET /behavioral-progress`, `GET /behavioral-progress/{id}`, `POST /behavioral-progress`, `PUT /behavioral-progress/{id}`, los endpoints análogos para eating-behavior-patterns, y `GET /recovery-plans`, `GET /recovery-plans/{id}`, `POST /recovery-plans`, `PUT /recovery-plans/{id}` y `DELETE /recovery-plans/{id}`. | 5 | Mora Rivera, Joel Fernando | Done |
| TS08 | API: Smart Recommendation — Pantry, Recipes, Weather Snapshots, Recommendation Cards, Recommendation Sessions, and Travel Contexts Endpoints | T25 | Implementar dominio Smart Recommendation: agregados, value objects y puertos | Crear los agregados `PantryItem`, `Recipe`, `WeatherSnapshot`, `UserLocationSnapshot`, `RecommendationCard`, `RecommendationSession` y `TravelContext` con sus invariantes. Crear los value objects `WeatherType`, `CardType` y `AdherenceStatus`. Crear los puertos de repositorio y los ports de servicios externos `WeatherServicePort` y `RecommendationAIPort`. | 4 | Angel Martin Villarreal Bazan | Done |
| TS08 | API: Smart Recommendation — Pantry, Recipes, Weather Snapshots, Recommendation Cards, Recommendation Sessions, and Travel Contexts Endpoints | T26 | Implementar servicios de aplicación Smart Recommendation con adaptadores externos | Implementar los servicios de comando y consulta para pantry, recipes, weather snapshots (incluyendo la lógica de sync con OpenWeatherMap en `POST /weather-snapshots/sync`), recommendation cards (con auto-fill cuando hay menos de 5 tarjetas para un `weatherType`), recommendation sessions y travel contexts. Implementar el adaptador para OpenWeatherMap y el adaptador para DeepSeek (generación de recomendaciones preventivas AT_RISK e intervención DROPPED). | 7 | Angel Martin Villarreal Bazan | Done |
| TS08 | API: Smart Recommendation — Pantry, Recipes, Weather Snapshots, Recommendation Cards, Recommendation Sessions, and Travel Contexts Endpoints | T27 | Implementar capa de persistencia Smart Recommendation con JPA | Crear entidades JPA, mappers y adaptadores de persistencia para todos los agregados del bounded context: `PantryItem`, `Recipe`, `WeatherSnapshot`, `UserLocationSnapshot`, `RecommendationCard`, `RecommendationSession` y `TravelContext`. | 5 | Angel Martin Villarreal Bazan | Done |
| TS08 | API: Smart Recommendation — Pantry, Recipes, Weather Snapshots, Recommendation Cards, Recommendation Sessions, and Travel Contexts Endpoints | T28 | Implementar REST controllers Smart Recommendation con documentación OpenAPI | Implementar los controladores REST cubriendo `GET /pantry`, `GET /pantry/{id}`, `POST /pantry`, `DELETE /pantry/{id}`, `GET /recipes`, `GET /recipes/{id}`, `POST /recipes`, `GET /weather-snapshots`, `POST /weather-snapshots`, `PUT /weather-snapshots/{id}`, `POST /weather-snapshots/sync`, `GET /user-location-snapshots`, `POST /user-location-snapshots`, `GET /recommendation-cards`, `POST /recommendation-cards`, `GET /recommendation-sessions`, `POST /recommendation-sessions`, `PUT /recommendation-sessions/{id}`, `GET /travel-contexts`, `POST /travel-contexts` y `PUT /travel-contexts/{id}`. Documentar con `@Tag`, `@Operation` y `@ApiResponse`. | 5 | Angel Martin Villarreal Bazan | Done |
| TS09 | API: Subscriptions — Subscription Lifecycle and Billing History Endpoints | T29 | Implementar dominio Subscriptions: agregados, value objects y puertos | Crear los value objects `SubscriptionPlan` y `SubscriptionStatus`. Crear los agregados `Subscription` (con `billingCycleStart`, `billingCycleEnd` y `pricePerMonth`) y `BillingRecord` con sus invariantes. Crear las excepciones de dominio y los puertos de repositorio `SubscriptionRepository` y `BillingRecordRepository`. | 3 | Villarreal Bazan, Angel Martin | Done |
| TS09 | API: Subscriptions — Subscription Lifecycle and Billing History Endpoints | T30 | Implementar servicios de aplicación Subscriptions: command y query services | Implementar `SubscriptionCommandService` (crear, actualizar plan — upgrade/downgrade sin procesamiento Stripe) y `SubscriptionQueryService` (obtener por ID, listar por userId). Implementar `BillingRecordCommandService` (crear registro de facturación con status PAID) y `BillingRecordQueryService` (obtener por ID, listar todos). | 4 | Villarreal Bazan, Angel Martin | Done |
| TS09 | API: Subscriptions — Subscription Lifecycle and Billing History Endpoints | T31 | Implementar capa de persistencia y REST controllers Subscriptions con documentación OpenAPI | Crear entidades JPA `SubscriptionJpaEntity` y `BillingRecordJpaEntity`, sus mappers, repositorios Spring Data y adaptadores de persistencia. Implementar `SubscriptionsController` con endpoints `GET /api/v1/subscriptions`, `POST /api/v1/subscriptions`, `GET /api/v1/subscriptions/{id}` y `PUT /api/v1/subscriptions/{id}`, e `BillingHistoryController` con `GET /api/v1/billing-history`, `GET /api/v1/billing-history/{id}` y `POST /api/v1/billing-history`. Documentar con `@Tag`, `@Operation` y `@ApiResponse`. | 4 | Villarreal Bazan, Angel Martin | Done |
| TS10 | API: Analytics — Dashboard Query and Recalculation Endpoints | T32 | Implementar dominio Analytics: agregados, value objects y puertos de integración | Crear los agregados `Analytics`, `DailySummary` y `AdherenceHistory` con sus value objects (`BmiCategory`, `AdherenceStatus`). Crear los puertos de repositorio y los puertos de adaptadores de contextos cruzados `BehavioralSummaryPort`, `NutritionSummaryPort`, `BodyMetricsSummaryPort` y `UserDataPort`. | 4 | Angela Milagros Espinoza Cruz | Done |
| TS10 | API: Analytics — Dashboard Query and Recalculation Endpoints | T33 | Implementar servicios de aplicación Analytics: command y query services | Implementar `AnalyticsCommandService` (recalcular dashboard diario con agregación de nutrition-log, body-metrics y behavioral-progress; validar formato yyyy-MM-dd retornando 400 ante entrada malformada) y `AnalyticsQueryService` (obtener analytics consolidado por userId; retornar 404 cuando el usuario no existe). | 5 | Angela Milagros Espinoza Cruz | Done |
| TS10 | API: Analytics — Dashboard Query and Recalculation Endpoints | T34 | Implementar capa de persistencia Analytics con JPA y adaptadores de contextos cruzados | Crear entidades JPA y adaptadores de persistencia para `Analytics`, `DailySummary` y `AdherenceHistory`. Implementar los adaptadores de integración con otros bounded contexts: `BehavioralSummaryAdapter`, `NutritionSummaryAdapter`, `BodyMetricsSummaryAdapter` y `UserDataAdapter`. | 5 | Del Angela Milagros Espinoza Cruz | Done |
| TS10 | API: Analytics — Dashboard Query and Recalculation Endpoints | T35 | Implementar REST controller Analytics con documentación OpenAPI y despliegue en producción | Implementar `AnalyticsController` con recursos `AnalyticsResource` y `UpdateDashboardResource` y sus assemblers. Exponer los endpoints `GET /api/v1/analytics/{userId}` y `POST /api/v1/analytics/dashboard/update`, restringiendo la exportación PDF a usuarios Premium. Documentar con `@Tag`, `@Operation` y `@ApiResponse`. Agregar Dockerfile multi-stage, configurar CORS para `app-smart.nutriproject.xyz`, actualizar `pom.xml` con la versión de release y configurar el despliegue en Coolify bajo el dominio `smart-api.nutriproject.xyz`. | 6 | Angela Milagros Espinoza Cruz | Done |

#### 5.2.3.4. Development Evidence for Sprint Review

Durante este sprint, el equipo completó la implementación del backend completo de la plataforma NutriSmart, cubriendo los bounded contexts de IAM, Subscriptions, Behavioral Consistency, Nutrition Tracking, Metabolic Adaptation, Restaurant Intelligence, Smart Recommendation y Analytics. El desarrollo fue gestionado mediante GitFlow, con ramas `feature/` individuales por bounded context fusionadas en `develop` y liberadas en `main` como versión `1.1.3`. Todos los endpoints fueron documentados con springdoc-openapi 3.0.2 y desplegados en producción bajo el dominio `smart-api.nutriproject.xyz`.

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Committed on |
|---|---|---|---|---|---|
| nutrismart-platform | feature/setup | `bd94e79` | chore: add project scaffolding, Maven wrapper, and build config | — | 2026-06-15 |
| nutrismart-platform | feature/setup | `9e8e22a` | feat(shared): add application entry point and shared bounded context | — | 2026-06-15 |
| nutrismart-platform | feature/setup | `7a5a918` | chore: add application resources, i18n messages, and smoke test | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `2160218` | feat: add LogActivityCommand | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `5e3e325` | feat: add LogBodyMetricsCommand | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `00600f8` | feat: add LogBodyCompositionCommand | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `a62719b` | feat: add ConnectWearableCommand | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `e2bb105` | feat: add DeleteWearableConnectionCommand | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `d4cc952` | feat: add DeleteActivityLogCommand | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `1f712bf` | feat: add RecordMetabolicAdaptationCommand | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `ffd7038` | feat: add UpdateBodyCompositionCommand | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `b23f6de` | feat: add UpdateBodyMetricCommand | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `e256647` | feat: add UpdateWearableConnectionCommand | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `d6e7b5e` | feat: add ActivityLogCommandFailure | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `abd626e` | feat: add ActivityLogCommandService | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `bdaae52` | feat: add BodyCompositionCommandFailure | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `889ff6d` | feat: add BodyCompositionCommandService | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `ec8f23b` | feat: add BodyMetricCommandFailure | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `d5abbb9` | feat: add BodyMetricCommandService | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `f139d3f` | feat: add MetabolicAdaptationLogCommandFailure | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `343fcfa` | feat: add MetabolicAdaptationLogCommandService | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `ebd5bda` | feat: add WearableConnectionCommandFailure | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `2451f35` | feat: add WearableConnectionCommandService | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `4fcfa27` | feat: add ActivityLogCommandServiceImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `7f54757` | feat: add BodyCompositionCommandServiceImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `cc4ecbc` | feat: add BodyMetricCommandServiceImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `cf57f13` | feat: add MetabolicAdaptationLogCommandServiceImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `6507b39` | feat: add WearableConnectionCommandServiceImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `6cb36fc` | feat: add GetAllActivityLogsQuery | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `db5cec3` | feat: add GetActivityLogByIdQuery | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `ce04217` | feat: add GetAllBodyCompositionsQuery | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `f0b7c71` | feat: add GetAllBodyMetricsQuery | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `c89fe95` | feat: add GetAllMetabolicAdaptationLogsQuery | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `26d5f89` | feat: add GetAllWearableConnectionsQuery | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `de58276` | feat: add GetWearableConnectionByIdQuery | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `ac2fd12` | feat: add ActivityLogQueryService | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `c3d3df1` | feat: add BodyCompositionQueryService | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `bcc70ce` | feat: add BodyMetricQueryService | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `be412a0` | feat: add MetabolicAdaptationLogQueryService | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `63abb4f` | feat: add WearableConnectionQueryService | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `53bbf3d` | feat: add MetabolicAdaptationContextFacade interface | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `8054a51` | feat: add ACL facade implementation MetabolicAdaptationContextFacadeImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `5c72d09` | feat: add ActivityLog aggregate | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `47c04c3` | feat: add BodyComposition aggregate | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `9db652c` | feat: add BodyMetric aggregate | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `48b92db` | feat: add WearableConnection aggregate | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `aa34515` | feat: add MetabolicAdaptationLog aggregate | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `3f7bd75` | feat: add BodyMetricRepository | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `91efabd` | feat: add BodyCompositionRepository | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `3a2007f` | feat: add ActivityLogRepository | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `c2bbc0f` | feat: add WearableConnectionRepository | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `3e63bdf` | feat: add MetabolicAdaptationLogRepository | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `f4d44ae` | feat: add WearableStatus value object | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `251dcfe` | feat: add MetabolicChangeTrigger value object | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `699d735` | feat: add BmiCategory value object | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `4d7fcdf` | feat: add DomainInvalidExceptions | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `9abbed0` | feat: add BodyMetricQueryServiceImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `4aa44b5` | feat: add BodyCompositionQueryServiceImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `e8da2db` | feat: add ActivityLogQueryServiceImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `1e90f8b` | feat: add WearableConnectionQueryServiceImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `4cc1173` | feat: add MetabolicAdaptationLogQueryServiceImpl | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `19bc996` | feat: add BodyMetricJpaEntity | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `bf82a71` | feat: add BodyCompositionJpaEntity | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `b1c6b07` | feat: add ActivityLogJpaEntity | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `1ac3674` | feat: add WearableConnectionJpaEntity | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `4c69be7` | feat: add MetabolicAdaptationLogJpaEntity | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `00cb7ba` | feat: add WearableStatusAttributeConverter | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `bf68584` | feat: add MetabolicChangeTriggerAttributeConverter | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `c27ecc0` | feat: add BodyMetricPersistenceMapper | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `c815ee7` | feat: add BodyCompositionPersistenceMapper | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `0316198` | feat: add ActivityLogPersistenceMapper | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `2016c4a` | feat: add WearableConnectionPersistenceMapper | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `bb537d4` | feat: add MetabolicAdaptationLogPersistenceMapper | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `040f6f1` | feat: add BodyMetricPersistenceAdapter | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `574f95a` | feat: add BodyCompositionPersistenceAdapter | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `4ec76e0` | feat: add ActivityLogPersistenceAdapter | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `e33409e` | feat: add WearableConnectionPersistenceAdapter | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `700a838` | feat: add MetabolicAdaptationLogPersistenceAdapter | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `7717aa8` | feat: add SpringDataBodyMetricJpaRepository | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `6ab6a1d` | feat: add SpringDataBodyCompositionJpaRepository | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `b41885d` | feat: add SpringDataActivityLogJpaRepository | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `87a3a0f` | feat: add SpringDataWearableConnectionJpaRepository | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `c9be3e8` | feat: add SpringDataMetabolicAdaptationLogJpaRepository | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `cc9ce50` | feat: add CreateBodyMetricResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `adf12c7` | feat: add UpdateBodyMetricResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `6cc57b7` | feat: add BodyMetricResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `1021c76` | feat: add CreateBodyCompositionResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `91d400b` | feat: add UpdateBodyCompositionResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `d83fcb2` | feat: add BodyCompositionResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `724dd66` | feat: add CreateActivityLogResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `3429ac8` | feat: add ActivityLogResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `2b31ad6` | feat: add CreateWearableConnectionResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `328d933` | feat: add UpdateWearableConnectionResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `c44e918` | feat: add WearableConnectionResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `3c016bb` | feat: add CreateMetabolicAdaptationLogResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `088ce14` | feat: add MetabolicAdaptationLogResource | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `8804e4d` | feat: add LogBodyMetricsCommandFromResourceAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `6f5ee23` | feat: add LogBodyCompositionCommandFromResourceAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `0ba082c` | feat: add UpdateBodyCompositionCommandFromResourceAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `cd756a8` | feat: add UpdateBodyMetricCommandFromResourceAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `ebbe167` | feat: add LogActivityCommandFromResourceAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `e4cb6b1` | feat: add ConnectWearableCommandFromResourceAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `9406694` | feat: add UpdateWearableConnectionCommandFromResourceAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `f4e3c36` | feat: add RecordMetabolicAdaptationCommandFromResourceAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `7d242ea` | feat: add BodyMetricResourceFromEntityAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `c9e86df` | feat: add BodyCompositionResourceFromEntityAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `82d6f05` | feat: add ActivityLogResourceFromEntityAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `72eae46` | feat: add WearableConnectionResourceFromEntityAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `562b720` | feat: add MetabolicAdaptationLogResourceFromEntityAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `bca7972` | feat: add ResponseEntityFromBodyMetricCommandResultAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `62ca219` | feat: add ResponseEntityFromBodyCompositionCommandResultAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `1f748a6` | feat: add ResponseEntityFromActivityLogCommandResultAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `233e91e` | feat: add ResponseEntityFromWearableConnectionCommandResultAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `2122a2a` | feat: add ResponseEntityFromMetabolicAdaptationLogCommandResultAssembler | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `1a41aaa` | feat: add BodyMetricsController | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `260d7f1` | feat: add BodyCompositionsController | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `c11c29b` | feat: add ActivityLogsController | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `d878eb2` | feat: add WearableConnectionsController | — | 2026-06-15 |
| nutrismart-platform | feature/metabolic-adaptation | `0789833` | feat: add MetabolicAdaptationLogsController | — | 2026-06-15 |
| nutrismart-platform | feature/nutrition-tracking | `03d5c51` | feat: add CreateDailyIntakeCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `0c1fd8e` | feat: add ConfirmPlateScanCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `4c11bfb` | feat: add DeleteMealLogCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `fbacce5` | feat: add DeleteFoodItemCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `bbe28d2` | feat: add LogMealCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `431f3ba` | feat: add RegisterFoodItemCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `3105e32` | feat: add ScanMenuCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `3ece776` | feat: add ScanPlateCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `cf64d63` | feat: add UpdateDailyIntakeCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `1df16e6` | feat: add UpdateFoodItemCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `280333d` | feat: add UpdateMealEntryCommand record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `e121606` | feat: add DailyIntakeCommandFailure sealed interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `899d652` | feat: add DailyIntakeCommandService interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `8db71de` | feat: add FoodImportCommandService interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `e0be180` | feat: add FoodImportFailure sealed interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `fb9c726` | feat: add FoodItemCommandFailure sealed interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `0dc4cde` | feat: add FoodItemCommandService interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `d6308b4` | feat: add MealRecordCommandFailure sealed interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `a7646be` | feat: add MealRecordCommandService interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `b02edda` | feat: add SmartScanCommandFailure sealed interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `dcd1d63` | feat: add SmartScanCommandService interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `3763486` | feat: add DailyIntakeCommandServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `f83c3c0` | feat: add FoodImportCommandServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `97cd906` | feat: add FoodItemCommandServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `dbee8b0` | feat: add MealRecordCommandServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `548f97f` | feat: add SmartScanCommandServiceImpl implementation | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `28f709d` | feat: add DailyIntakeQueryServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `62d225b` | feat: add FoodItemQueryServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `bd2e54e` | feat: add MealRecordQueryServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `32ae40d` | feat: add DailyIntake aggregate root | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `2092866` | feat: add FoodItem aggregate root model | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `47db3c9` | feat: add MealRecord aggregate root model | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `5f097d2` | feat: add DomainInvalidExceptions runtime exception | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `2e574a0` | feat: add DailyIntakeRepository interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `28b2211` | feat: add FoodItemRepository interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `941249e` | feat: add MealRecordRepository interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `4a90ef3` | feat: add FoodRestriction enum | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `21f9694` | feat: add MealType enum for nutrition tracking | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `b6e58e2` | feat: add NutritionalRiskLevel enum | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `5fc8404` | feat: add GetAllDailyIntakesQuery record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `d1643a7` | feat: add GetAllFoodItemsQuery record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `c585e64` | feat: add GetAllMealRecordsQuery record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `8b5b8cf` | feat: add GetDailyIntakeByIdQuery record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `27e58a1` | feat: add GetDailyIntakeByUserIdAndDateQuery record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `c699313` | feat: add GetDailyIntakeByUserIdQuery record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `0ebc5b6` | feat: add DailyIntakeQueryService interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `fb9a0e2` | feat: add FoodItemQueryService interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `feebabe` | feat: add MealRecordQueryService interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `920cd90` | feat: add UserProfileLookupPort interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `fc536da` | feat: add UserProfileData record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `3fe7d22` | feat: add ExternalFoodDataPort interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `b60f8b0` | feat: add ExternalFoodData DTO record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `a70449c` | feat: add FoodEnrichmentPort interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `baa0aa8` | feat: add EnrichedFoodData record DTO | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `f302401` | feat: add ImageRecognitionPort interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `c1fcfd5` | feat: add PlateItemMatchPort interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `294f3ba` | feat: add MenuRankingPort interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `4db8fce` | feat: add DetectedFoodItem record DTO | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `ffcf966` | feat: add PlateItemMatchResult record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `34bc34e` | feat: add PlateItemResult record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `36cc70a` | feat: add RankedDishData record for dish ranking | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `f620843` | feat: add RankedMenuResult record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `211e669` | feat: add MenuDishCandidate DTO record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `9b74a1a` | feat: add FoodItemCandidate record DTO | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `b10696c` | feat: add GeneratedMenuFoodData DTO record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `9e4970d` | feat: add DeepSeek RestTemplate bean | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `a086cd3` | feat: add DeepSeekClient for DeepSeek API | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `35a6411` | feat: add DeepSeekEnrichmentRequest record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `82d088e` | feat: add DeepSeekEnrichmentResponse record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `c03a573` | feat: add DeepSeek food enrichment adapter | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `9bb9815` | feat: add DeepSeekMenuRankingAdapter for menu ranking | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `b4bf198` | feat: add DeepSeek adapter for plate item matching | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `b5d3f82` | feat: add GeminiRequest model for Vision API | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `6abd5b3` | feat: add GeminiResponse model for Gemini Vision API | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `3d60917` | feat: add GeminiVisionAdapter for image recognition | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `40e6538` | feat: add Gemini Vision client and config | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `07c4ab4` | feat: add USDAFoodDataClient for USDA API search | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `56c31b7` | feat: add USDAFoodDataAdapter for USDA API | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `f05b446` | feat: add USDA RestTemplate config bean | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `2f99914` | feat: add USDA food search response DTOs | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `f9847ed` | feat: add UserProfileLookupAdapter | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `73c5b66` | feat: add DailyIntakeJpaEntity JPA entity | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `b40364c` | feat: add FoodItem JPA entity for foods table | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `06ba083` | feat: add MealRecordJpaEntity JPA entity | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `ff8dd51` | feat: add JPA converter for MealType enum | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `773417f` | feat: add DailyIntake JPA adapter and converter | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `fba594c` | feat: add DailyIntake persistence mapper | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `5e9580d` | feat: add FoodItem JPA persistence mapper | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `3aa1495` | feat: add MealRecord persistence mapper | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `faf3129` | feat: add JPA persistence adapter for FoodItem | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `d7de554` | feat: add MealRecordPersistenceAdapter JPA adapter | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `20fd786` | feat: add SpringData JPA repository for DailyIntake | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `4722257` | feat: add JPA repositories for FoodItem and MealRecord | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `ce4d419` | feat: add NutritionTrackingContextFacadeImpl | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `2401e49` | feat: add NutritionTrackingContextFacade interface | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `0894260` | feat: add ConfirmPlateScanRequest record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `207935a` | feat: add food and daily intake resources | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `9d51497` | feat: add CreateMealRecordResource record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `90ee08e` | feat: add DailyIntakeResource record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `627cc0a` | feat: add FoodItemResource record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `c911bfa` | feat: add MealRecordResource REST DTO | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `6c6b3c5` | feat: add ScanMenuRequest record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `d68e25e` | feat: add ScanMenuResultResource record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `aa89b1b` | feat: add ScanPlateRequest record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `3bbfcf5` | feat: add ScanPlateResultResource record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `b107790` | feat: add UpdateDailyIntakeResource record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `8d17d57` | feat: add UpdateFoodItemResource record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `6b94875` | feat: add UpdateMealRecordResource record | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `e66de82` | feat: add DailyIntakeCommand resource assembler | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `964db9f` | feat: add DailyIntakeResource assembler | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `1c78c8c` | feat: add FoodItem resource/command assemblers | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `d691045` | feat: add MealRecordCommandFromResourceAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `a305e99` | feat: add MealRecordResourceFromEntityAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `3028453` | feat: add assembler for DailyIntake command results | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `772518e` | feat: add ResponseEntity assembler for FoodItem results | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `a103936` | feat: add ResponseEntity assembler for MealRecord | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `c2ec4ac` | feat: add DailyBalanceController REST endpoint | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `6cb62d2` | feat: add DailyIntakeController REST API | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `c81cf4e` | feat: add FoodsController REST endpoint | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `e2d8529` | feat: add NutritionLogController REST API | — | 2026-06-16 |
| nutrismart-platform | feature/nutrition-tracking | `cccf849` | feat: add SmartScanController REST endpoints | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `2dc9bc0` | feat: add Analytics aggregate | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `b9215bd` | feat: add DomainInvalidExceptions | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `56ee162` | feat: add AdherenceStatus value object | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `63baac2` | feat: add BmiCategory value object | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `af6c07b` | feat: add UpdateAdherenceProgressCommand | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `880b6fa` | feat: add UpdateDailyDashboardCommand | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `c2a04cc` | feat: add AnalyticsCommandFailure | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `277405c` | feat: add AnalyticsCommandService | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `cf693bd` | feat: add AnalyticsCommandServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `44c07f6` | feat: add AnalyticsQueryServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `40d0b5b` | feat: add BehavioralSummaryPort | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `1645361` | feat: add BodyMetricsSummaryPort | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `a5f656f` | feat: add NutritionSummaryPort | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `46466df` | feat: add UserDataPort | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `8781b55` | feat: add GetAnalyticsByUserIdQuery | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `6d1b796` | feat: add GetDashboardByUserIdQuery | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `77948bc` | feat: add AnalyticsQueryService | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `bfae50b` | feat: add BehavioralSummaryAdapter | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `0fa61f9` | feat: add BodyMetricsSummaryAdapter | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `017a817` | feat: add NutritionSummaryAdapter | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `616f4bd` | feat: add UserDataAdapter | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `4592c5d` | feat: add AnalyticsResource | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `68c304f` | feat: add UpdateDashboardResource | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `e728d44` | feat: add AnalyticsResourceFromEntityAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/analytics | `9b07189` | feat: add AnalyticsController | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `af21555` | feat(behavioral-consistency): add EatingBehaviorPattern aggregate | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `3cbc1e9` | feat(behavioral-consistency): add BehavioralProgress aggregate | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `c0b021e` | feat(behavioral-consistency): add RecoveryPlan aggregate | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `4eb2cdd` | feat(behavioral-consistency): add BehaviorPatternType value object | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `b1a471c` | feat(behavioral-consistency): add AdherenceStatus value object | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `81a8c57` | feat(behavioral-consistency): add AdherenceDropTrigger value object | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `b47ea1f` | feat(behavioral-consistency): add RecoveryActionType value object | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `1fd97b6` | feat(behavioral-consistency): add RecoveryPlanStatus value object | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `95c6c06` | feat(behavioral-consistency): add EatingBehaviorPatternRepository contract | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `6a2376d` | feat(behavioral-consistency): add BehavioralProgressRepository contract | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `400a964` | feat(behavioral-consistency): add RecoveryPlanRepository contract | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `f768e59` | feat(behavioral-consistency): add DomainInvalidExceptions | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `bcd1eb6` | feat(behavioral-consistency): add CreateEatingBehaviorPatternCommand | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `80edf75` | feat(behavioral-consistency): add UpdateEatingBehaviorPatternCommand | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `9afc87b` | feat(behavioral-consistency): add CreateBehavioralProgressCommand | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `e61c993` | feat(behavioral-consistency): add UpdateBehavioralProgressCommand | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `5d6e674` | feat(behavioral-consistency): add CreateRecoveryPlanCommand | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `241bef8` | feat(behavioral-consistency): add UpdateRecoveryPlanCommand | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `30977c8` | feat(behavioral-consistency): add DeleteRecoveryPlanCommand | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `8909117` | feat(behavioral-consistency): add GetAllEatingBehaviorPatternsQuery | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `4fb155b` | feat(behavioral-consistency): add GetEatingBehaviorPatternByIdQuery | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `ff39924` | feat(behavioral-consistency): add GetAllBehavioralProgressQuery | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `e38ff89` | feat(behavioral-consistency): add GetBehavioralProgressByIdQuery | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `db4376f` | feat(behavioral-consistency): add GetAllRecoveryPlansQuery | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `2b0f231` | feat(behavioral-consistency): add GetRecoveryPlanByIdQuery | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `2df81a3` | feat(behavioral-consistency): add EatingBehaviorPatternCommandService interface | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `8b094aa` | feat(behavioral-consistency): add EatingBehaviorPatternCommandFailure | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `f9b576b` | feat(behavioral-consistency): add BehavioralProgressCommandService interface | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `6d8ff5b` | feat(behavioral-consistency): add BehavioralProgressCommandFailure | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `ccf04a4` | feat(behavioral-consistency): add RecoveryPlanCommandService interface | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `fff911f` | feat(behavioral-consistency): add RecoveryPlanCommandFailure | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `2ce7498` | feat(behavioral-consistency): add EatingBehaviorPatternQueryService interface | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `5581a00` | feat(behavioral-consistency): add BehavioralProgressQueryService interface | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `4f0a341` | feat(behavioral-consistency): add RecoveryPlanQueryService interface | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `87caebc` | feat(behavioral-consistency): implement EatingBehaviorPatternCommandServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `03ed76c` | feat(behavioral-consistency): implement BehavioralProgressCommandServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `4be9e07` | feat(behavioral-consistency): implement RecoveryPlanCommandServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `acd1e86` | feat(behavioral-consistency): implement EatingBehaviorPatternQueryServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `0f783f7` | feat(behavioral-consistency): implement BehavioralProgressQueryServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `d667817` | feat(behavioral-consistency): implement RecoveryPlanQueryServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `9923e8d` | feat(behavioral-consistency): implement BehavioralConsistencyContextFacadeImpl | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `82370be` | feat(behavioral-consistency): add BehavioralConsistencyContextFacade interface | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `6793bc9` | feat(behavioral-consistency): add EatingBehaviorPatternJpaEntity | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `1d56383` | feat(behavioral-consistency): add BehavioralProgressJpaEntity | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `56c46f1` | feat(behavioral-consistency): add RecoveryPlanJpaEntity | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `46daf3d` | feat(behavioral-consistency): add BehaviorPatternTypeAttributeConverter | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `9214835` | feat(behavioral-consistency): add AdherenceStatusAttributeConverter | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `01ad5ef` | feat(behavioral-consistency): add AdherenceDropTriggerAttributeConverter | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `4141440` | feat(behavioral-consistency): add RecoveryPlanStatusAttributeConverter | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `0e621ca` | feat(behavioral-consistency): add EatingBehaviorPatternPersistenceMapper | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `36eb994` | feat(behavioral-consistency): add BehavioralProgressPersistenceMapper | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `2117adc` | feat(behavioral-consistency): add RecoveryPlanPersistenceMapper | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `20f7f19` | feat(behavioral-consistency): add SpringDataEatingBehaviorPatternJpaRepository | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `16563c8` | feat(behavioral-consistency): add SpringDataBehavioralProgressJpaRepository | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `477f046` | feat(behavioral-consistency): add SpringDataRecoveryPlanJpaRepository | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `64b3b70` | feat(behavioral-consistency): implement EatingBehaviorPatternPersistenceAdapter | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `d618fd6` | feat(behavioral-consistency): implement BehavioralProgressPersistenceAdapter | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `4e08af4` | feat(behavioral-consistency): implement RecoveryPlanPersistenceAdapter | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `104a45e` | feat(behavioral-consistency): add CreateEatingBehaviorPatternResource DTO | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `4659544` | feat(behavioral-consistency): add UpdateEatingBehaviorPatternResource DTO | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `fc6b982` | feat(behavioral-consistency): add EatingBehaviorPatternResource DTO | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `74f0177` | feat(behavioral-consistency): add CreateBehavioralProgressResource DTO | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `7692b45` | feat(behavioral-consistency): add UpdateBehavioralProgressResource DTO | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `c40e5ff` | feat(behavioral-consistency): add BehavioralProgressResource DTO | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `9b31e24` | feat(behavioral-consistency): add CreateRecoveryPlanResource DTO | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `9248ab7` | feat(behavioral-consistency): add UpdateRecoveryPlanResource DTO | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `1dc8b81` | feat(behavioral-consistency): add RecoveryPlanResource DTO | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `f15cefb` | feat(behavioral-consistency): add CreateEatingBehaviorPatternCommandFromResourceAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `5cd14df` | feat(behavioral-consistency): add UpdateEatingBehaviorPatternCommandFromResourceAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `6d77bc8` | feat(behavioral-consistency): add EatingBehaviorPatternResourceFromEntityAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `3856b3d` | feat(behavioral-consistency): add ResponseEntityFromEatingBehaviorPatternCommandResultAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `03f043b` | feat(behavioral-consistency): add CreateBehavioralProgressCommandFromResourceAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `f86bfbd` | feat(behavioral-consistency): add UpdateBehavioralProgressCommandFromResourceAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `e201914` | feat(behavioral-consistency): add BehavioralProgressResourceFromEntityAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `d611f36` | feat(behavioral-consistency): add ResponseEntityFromBehavioralProgressCommandResultAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `4190a6d` | feat(behavioral-consistency): add CreateRecoveryPlanCommandFromResourceAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `13c2927` | feat(behavioral-consistency): add UpdateRecoveryPlanCommandFromResourceAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `c1b699e` | feat(behavioral-consistency): add RecoveryPlanResourceFromEntityAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `0fc0287` | feat(behavioral-consistency): add ResponseEntityFromRecoveryPlanCommandResultAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `122087f` | feat(behavioral-consistency): add EatingBehaviorPatternsController | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `fa57582` | feat(behavioral-consistency): add BehavioralProgressController | — | 2026-06-16 |
| nutrismart-platform | feature/behavioral-consistency | `370e306` | feat(behavioral-consistency): add RecoveryPlansController | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `787109c` | feat(iam): add EmailAddress value object | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `8a3b2ab` | feat(iam): add ActivityLevel value object | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `13d7868` | feat(iam): add DietaryRestriction value object | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `94f7775` | feat(iam): add UserGoal value object | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `f9b809f` | feat(iam): add UserPlan value object | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `6343d9c` | feat(iam): add domain invalid exceptions | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `2ca7d0c` | feat(iam): add User aggregate | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `ddc6b2b` | feat(iam): add PasswordResetToken aggregate | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `05f0bfd` | feat(iam): add UserRepository port | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `4ee7e3e` | feat(iam): add PasswordResetTokenRepository port | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `db7fe59` | feat(iam): add EmailService domain service port | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `35cc6f3` | feat(iam): add RegisterAccountCommand | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `2bd4073` | feat(iam): add AuthenticateCommand | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `38db0c7` | feat(iam): add UpdateUserCommand | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `fabcbb4` | feat(iam): add DeleteUserCommand | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `cbb1c57` | feat(iam): add SubmitOnboardingProfileCommand | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `0199200` | feat(iam): add RequestPasswordResetCommand | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `a2ca324` | feat(iam): add ResetPasswordCommand | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `e113980` | feat(iam): add GetUserByIdQuery | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `8b9b402` | feat(iam): add GetUserByEmailQuery | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `07b7e79` | feat(iam): add GetAllUsersQuery | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `2ccbba9` | feat(iam): add AuthCommandService port | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `1f6c555` | feat(iam): add AuthFailure result type | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `d2df974` | feat(iam): add AuthTokenData result type | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `5e385ea` | feat(iam): add PasswordResetCommandService port | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `e7fafd5` | feat(iam): add UserCommandService port | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `5d48eb9` | feat(iam): add UserQueryService port | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `5e3153a` | feat(iam): add AuthCommandService implementation | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `e4ccad0` | feat(iam): add PasswordResetCommandService implementation | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `cbe3c6a` | feat(iam): add UserCommandService implementation | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `76690d0` | feat(iam): add UserQueryService implementation | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `7400cf7` | feat(iam): add IamContextFacade implementation | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `8636643` | feat(iam): add EmailAddress JPA attribute converter | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `2bff509` | feat(iam): add ActivityLevel JPA attribute converter | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `14c5bff` | feat(iam): add SubscriptionPlan JPA attribute converter | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `75ef453` | feat(iam): add UserGoal JPA attribute converter | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `e9d24af` | feat(iam): add User JPA entity | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `ec291ad` | feat(iam): add PasswordResetToken JPA entity | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `ba9ae1d` | feat(iam): add User persistence mapper | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `79ff188` | feat(iam): add Spring Data User JPA repository | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `e7e0386` | feat(iam): add Spring Data PasswordResetToken JPA repository | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `bf55f8e` | feat(iam): add User persistence adapter | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `ec64fb7` | feat(iam): add PasswordResetToken persistence adapter | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `ddccffd` | feat(iam): add Gmail email service adapter | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `0c7d23e` | feat(iam): add CreateUserResource REST resource | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `8699518` | feat(iam): add LoginResource REST resource | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `0edfeed` | feat(iam): add ForgotPasswordResource REST resource | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `6986ecb` | feat(iam): add ResetPasswordResource REST resource | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `f584c0d` | feat(iam): add UpdateUserResource REST resource | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `1206ef0` | feat(iam): add UserResource REST resource | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `4e9a615` | feat(iam): add AuthResponse REST resource | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `6f2ee8f` | feat(iam): add IamContextFacade ACL interface | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `2c41d6b` | feat(iam): add CreateUserCommand resource assembler | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `6c4e47b` | feat(iam): add auth command result response assembler | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `28d9b33` | feat(iam): add user command result response assembler | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `46e3e49` | feat(iam): add UpdateUserCommand resource assembler | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `cef42a9` | feat(iam): add UserResource entity assembler | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `933a3ea` | feat(iam): add AuthController REST controller | — | 2026-06-16 |
| nutrismart-platform | feature/iam | `e711f58` | feat(iam): add UsersController REST controller | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `39deb3f` | feat(subscriptions): add SubscriptionPlan value object | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `3324ec8` | feat(subscriptions): add SubscriptionStatus value object | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `0bdd5ed` | feat(subscriptions): add domain invalid exceptions | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `d264d69` | feat(subscriptions): add Subscription aggregate | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `cbe4339` | feat(subscriptions): add BillingRecord aggregate | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `90ae9b8` | feat(subscriptions): add SubscriptionRepository port | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `e613431` | feat(subscriptions): add BillingRecordRepository port | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `d1fa99a` | feat(subscriptions): add CreateSubscriptionCommand | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `e67a49f` | feat(subscriptions): add UpdateSubscriptionCommand | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `f6160fb` | feat(subscriptions): add CreateBillingRecordCommand | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `c6aa26d` | feat(subscriptions): add GetAllSubscriptionsQuery | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `797cd5a` | feat(subscriptions): add GetSubscriptionByIdQuery | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `27435b5` | feat(subscriptions): add GetAllBillingRecordsQuery | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `de92972` | feat(subscriptions): add GetBillingRecordByIdQuery | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `cc2ba8b` | feat(subscriptions): add BillingRecordQueryService interface | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `acb4ad5` | feat(subscriptions): add SubscriptionQueryService interface | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `c404df2` | feat(subscriptions): add BillingRecordCommandService interface | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `35c71b3` | feat(subscriptions): add BillingRecordCommandFailure | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `bd26110` | feat(subscriptions): add SubscriptionCommandService interface | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `3700aa2` | feat(subscriptions): add SubscriptionCommandFailure | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `a2c6093` | feat(subscriptions): add SubscriptionCommandServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `833a6cb` | feat(subscriptions): add BillingRecordCommandServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `8340772` | feat(subscriptions): add SubscriptionQueryServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `eedfd20` | feat(subscriptions): add BillingRecordQueryServiceImpl | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `23de867` | feat(subscriptions): add SubscriptionJpaEntity | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `accc75e` | feat(subscriptions): add BillingRecordJpaEntity | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `fb76ceb` | feat(subscriptions): add SubscriptionStatusAttributeConverter | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `2d91999` | feat(subscriptions): add SpringDataSubscriptionJpaRepository | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `d32129e` | feat(subscriptions): add SpringDataBillingRecordJpaRepository | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `bf10891` | feat(subscriptions): add SubscriptionPersistenceMapper | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `2792020` | feat(subscriptions): add BillingRecordPersistenceMapper | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `776ff0f` | feat(subscriptions): add SubscriptionPersistenceAdapter | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `b2dcc6d` | feat(subscriptions): add BillingRecordPersistenceAdapter | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `2e3dcd5` | feat(subscriptions): add SubscriptionResource | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `dd48568` | feat(subscriptions): add CreateSubscriptionResource | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `e48e988` | feat(subscriptions): add UpdateSubscriptionResource | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `8b001f4` | feat(subscriptions): add BillingRecordResource | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `1860ed9` | feat(subscriptions): add CreateBillingRecordResource | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `b1898f8` | feat(subscriptions): add SubscriptionCommandFromResourceAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `137825a` | feat(subscriptions): add SubscriptionResourceFromEntityAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `4c509b2` | feat(subscriptions): add ResponseEntityFromSubscriptionCommandResultAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `8d89cc9` | feat(subscriptions): add BillingRecordCommandFromResourceAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `425facd` | feat(subscriptions): add BillingRecordResourceFromEntityAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `01a3608` | feat(subscriptions): add ResponseEntityFromBillingRecordCommandResultAssembler | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `15c14e4` | feat(subscriptions): add SubscriptionsController | — | 2026-06-16 |
| nutrismart-platform | feature/subscription | `0899d1a` | feat(subscriptions): add BillingHistoryController | — | 2026-06-16 |
| nutrismart-platform | feature/smart-recommendation | `95f0cc7` | feat(smartrecommendation): add domain model aggregates, value objects, repositories, and exceptions | — | 2026-06-16 |
| nutrismart-platform | feature/smart-recommendation | `19cf4d2` | feat(smartrecommendation): add application commands and queries | — | 2026-06-16 |
| nutrismart-platform | feature/smart-recommendation | `918bf0f` | feat(smartrecommendation): add application service interfaces, port definitions, and failure types | — | 2026-06-16 |
| nutrismart-platform | feature/smart-recommendation | `b5a4541` | feat(smartrecommendation): add internal command and query service implementations | — | 2026-06-16 |
| nutrismart-platform | feature/smart-recommendation | `ee43b25` | feat(smartrecommendation): add JPA persistence layer with entities, mappers, repositories, and adapters | — | 2026-06-16 |
| nutrismart-platform | feature/smart-recommendation | `1ed1356` | feat(smartrecommendation): add external service adapters for DeepSeek and OpenWeatherMap | — | 2026-06-16 |
| nutrismart-platform | feature/smart-recommendation | `f477947` | feat(smartrecommendation): add REST controllers, resources, and assemblers | — | 2026-06-16 |
| nutrismart-platform | main | `79621ed` | feat: add @Tags on restant classes | — | 2026-06-16 |
| nutrismart-platform | main | `8ef4355` | fix: subscription error on user.plan | — | 2026-06-16 |
| nutrismart-platform | main | `a79cc24` | fix: seeder duplicate crash on restart + DDL comment fix | — | 2026-06-16 |
| nutrismart-platform | main | `396743e` | chore: update app version | — | 2026-06-16 |
| nutrismart-platform | main | `a389151` | feat: add dockerfile | — | 2026-06-16 |
| nutrismart-platform | main | `a4d6e11` | ci: add release workflow | — | 2026-06-16 |
| nutrismart-platform | main | `a6ca2d0` | docs: update README.md | — | 2026-06-16 |
| nutrismart-platform | feature/restaurant-intelligence | `4f7a447` | feat: update restaurant intelligence bounded context | — | 2026-06-17 |
| nutrismart-platform | feature/restaurant-intelligence | `4e0204b` | chore: update cors | — | 2026-06-17 |
| nutrismart-platform | main | `1f00037` | chore: update pom.xml | — | 2026-06-17 |
| nutrismart-platform | main | `863d4ea` | Merge pull request #27 from develop — release/1.1.3 | — | 2026-06-17 |

#### 5.2.3.5. Execution Evidence for Sprint Review

Durante el Sprint 3, el equipo completó la implementación del backend completo de la plataforma NutriSmart. El backend fue construido con Spring Boot 3, Java 21, JPA/Hibernate y MySQL, siguiendo la arquitectura DDD con cuatro capas por bounded context: `domain`, `application`, `infrastructure` e `interfaces`. Todos los endpoints fueron documentados con springdoc-openapi 3.0.2 y Swagger UI, y el backend fue desplegado exitosamente en producción usando Docker y Coolify bajo el dominio `smart-api.nutriproject.xyz`.

Los bounded contexts implementados cubren: autenticación y gestión de usuarios con JWT (IAM), gestión de suscripciones sin procesamiento de pagos real (Subscriptions), adherencia conductual con los cuatro estados ON_TRACK/AT_RISK/DROPPED/RECOVERED (Behavioral Consistency), registro y análisis nutricional diario (Nutrition Tracking), métricas corporales y actividad física manual con estimación MET (Metabolic Adaptation), análisis de menús de restaurante con IA DeepSeek y ranking de platos compatibles (Restaurant Intelligence), recomendaciones contextuales con clima vía OpenWeatherMap (Smart Recommendation) y dashboard analítico con historial de adherencia (Analytics).

![Swagger](../assets/img/sprint3/swagger.png)

**IAM — AuthController y UsersController:**

Los endpoints de autenticación permiten el registro de nuevos usuarios con emisión de JWT, login con validación de credenciales, solicitud de recuperación de contraseña vía Gmail y restablecimiento de contraseña mediante token. El endpoint `GET /api/v1/auth/check-email` verifica disponibilidad de email antes del registro.

**Subscriptions — SubscriptionsController y BillingHistoryController:**

Los endpoints de suscripciones permiten consultar el plan activo del usuario, actualizar el plan (upgrade/downgrade sin procesamiento Stripe) y consultar el historial de facturación. La lógica de activación y desactivación de beneficios por cambio de plan queda registrada en los agregados de dominio.

**Behavioral Consistency — BehavioralProgressController, EatingBehaviorPatternsController y RecoveryPlansController:**

Los endpoints de adherencia conductual exponen el progreso conductual del usuario con su estado actual (ON_TRACK/AT_RISK/DROPPED/RECOVERED), los patrones de comportamiento alimenticio detectados y los planes de recuperación personalizados. El estado de adherencia se actualiza automáticamente según las reglas de negocio del dominio.

**Nutrition Tracking:**

Los endpoints de registro nutricional exponen búsqueda de alimentos con filtrado por restricciones dietéticas del usuario, registro de comidas con validación de límites calóricos y consulta de balance diario con desglose de macronutrientes.

**Restaurant Intelligence:**

El endpoint `POST /api/v1/restaurant-intelligence/menu-scan` recibe una imagen en base64, la envía a la API de DeepSeek para análisis, y retorna los platos identificados rankeados por compatibilidad nutricional con las restricciones y metas del usuario. Los platos que generan conflicto con restricciones dietéticas son marcados con `RestrictedDishFlagged`.

**Smart Recommendation:**

Los endpoints de recomendación inteligente retornan recomendaciones contextuales según el estado de adherencia conductual y las condiciones climáticas obtenidas de OpenWeatherMap. Los usuarios en estado AT_RISK reciben recomendaciones preventivas y los usuarios en estado DROPPED reciben planes de intervención graduales.

**Metabolic Adaptation:**

Los endpoints de adaptación metabólica exponen el registro y consulta de métricas corporales (BMI, BMR, TDEE), historial de peso, configuración de peso objetivo con proyección de logro, y registro manual de actividad física con estimación de calorías quemadas mediante tabla MET.

**Analytics:**

Los endpoints de analytics exponen el dashboard diario del usuario con métricas consolidadas y la línea de tiempo de adherencia conductual. El endpoint de exportación PDF está restringido a usuarios con plan Premium.

**URL del video de demostración del Sprint 3:** [Video del sprint 3](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202417857_upc_edu_pe/IQALj-97MSKOTKqBTU5O-MMQATA02rRMc3bB2bv81Bco8nY?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=YrDcHj)  

`https://upcedupe-my.sharepoint.com/:v:/g/personal/u202417857_upc_edu_pe/IQALj-97MSKOTKqBTU5O-MMQATA02rRMc3bB2bv81Bco8nY?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=YrDcHj`

#### 5.2.3.6. Services Documentation Evidence for Sprint Review

Durante el Sprint 3 se documentaron todos los endpoints RESTful del backend de NutriSmart utilizando springdoc-openapi 3.0.2 con Swagger UI. La documentación fue generada automáticamente a partir de las anotaciones `@Tag`, `@Operation`, `@ApiResponse` y `@Parameter` presentes en cada controller, y el SecurityScheme Bearer JWT fue configurado globalmente en `OpenApiConfiguration`.

**URLs de Swagger UI:**

| Entorno | URL de Swagger UI |
|---------|------------------|
| Local | `http://localhost:8080/swagger-ui/index.html` |
| Producción | `https://smart-api.nutriproject.xyz/swagger-ui/index.html` |
| JSON spec (OpenAPI) | `https://smart-api.nutriproject.xyz/v3/api-docs` |

**Repositorio de Web Services:** `https://github.com/upc-pre-202610-1asi0729-17952-devteam/nutrismart-platform`

**Commits relacionados con documentación OpenAPI (Sprint 3):**

| Commit Id | Mensaje | Bounded Context |
|-----------|---------|-----------------|
| `79621ed` | feat: add @Tags on restant classes | Global |
| `933a3ea` | feat(iam): add AuthController REST controller | IAM |
| `e711f58` | feat(iam): add UsersController REST controller | IAM |
| `15c14e4` | feat(subscriptions): add SubscriptionsController | Subscriptions |
| `0899d1a` | feat(subscriptions): add BillingHistoryController | Subscriptions |
| `122087f` | feat(behavioral-consistency): add EatingBehaviorPatternsController | Behavioral Consistency |
| `fa57582` | feat(behavioral-consistency): add BehavioralProgressController | Behavioral Consistency |
| `370e306` | feat(behavioral-consistency): add RecoveryPlansController | Behavioral Consistency |
| `f477947` | feat(smartrecommendation): add REST controllers, resources, and assemblers | Smart Recommendation |
| `4f7a447` | feat: update restaurant intelligence bounded context | Restaurant Intelligence |
| `9b07189` | feat: add AnalyticsController | Analytics |

A continuación se detalla la documentación de los principales endpoints del sprint.

---

**Bounded Context: IAM**

**Endpoint: POST /api/v1/auth/register**
Descripción: Registra un nuevo usuario y retorna un JWT de acceso.
Request Body:
```json
{
  "firstName": "María",
  "lastName": "García",
  "email": "maria.garcia@email.com",
  "password": "SecurePass123!"
}
```
Responses:

| Código | Descripción |
|--------|-------------|
| 201 | Account created — JWT returned |
| 400 | Invalid request data |
| 409 | Email already registered |

---

**Endpoint: POST /api/v1/auth/login**
Descripción: Autentica un usuario existente y retorna un JWT.
Request Body:
```json
{
  "email": "maria.garcia@email.com",
  "password": "SecurePass123!"
}
```
Responses:

| Código | Descripción |
|--------|-------------|
| 200 | Authentication successful — JWT returned |
| 401 | Invalid credentials |
| 423 | Account locked after multiple failures |

---

**Endpoint: POST /api/v1/auth/forgot-password**
Descripción: Envía un correo de recuperación de contraseña. Retorna 200 independientemente de si el email existe para no revelar información.
Request Body:
```json
{ "email": "maria.garcia@email.com" }
```
Responses:

| Código | Descripción |
|--------|-------------|
| 200 | Password reset email sent (always) |
| 400 | Invalid email format |

---

**Endpoint: GET /api/v1/auth/check-email**
Descripción: Verifica si un email ya está registrado.
Parámetros: `email` (query param, string, requerido). Ejemplo: `?email=maria.garcia@email.com`
Responses:

| Código | Descripción |
|--------|-------------|
| 200 | `{ "available": true }` o `{ "available": false }` |
| 400 | Invalid email format |

---

**Bounded Context: Restaurant Intelligence**

**Endpoint: POST /api/v1/restaurant-intelligence/menu-scan**
Descripción: Escanea imagen de menú de restaurante con IA y retorna platos rankeados por compatibilidad nutricional con las restricciones y metas del usuario autenticado.
Authorization: Bearer JWT requerido.
Request Body:
```json
{
  "imageBase64": "data:image/jpeg;base64,/9j/4AAQSkZJRgAB..."
}
```
Respuesta exitosa (200):
```json
{
  "dishes": [
    {
      "rank": 1,
      "dishName": "Grilled Salmon",
      "compatibilityScore": 0.92,
      "reason": "Alta en proteína, baja en carbohidratos",
      "estimatedCalories": 350,
      "estimatedProtein": 42,
      "estimatedCarbs": 2,
      "estimatedFat": 18,
      "conflictingRestrictions": []
    }
  ],
  "scannedAt": "2026-06-17T15:30:00Z"
}
```

Responses:

| Código | Descripción |
|--------|-------------|
| 200 | Menu scanned — ranked dishes returned |
| 400 | Invalid image or request data |
| 401 | Authentication required |
| 403 | Premium or Pro plan required |

---

**Bounded Context: Behavioral Consistency**

**Endpoint: GET /api/v1/behavioral-consistency/progress/{userId}**
Descripción: Obtiene el estado de adherencia conductual actual del usuario, incluyendo estado ON_TRACK/AT_RISK/DROPPED/RECOVERED, racha activa y fecha del último registro.
Authorization: Bearer JWT requerido.
Responses:

| Código | Descripción |
|--------|-------------|
| 200 | Behavioral progress returned |
| 401 | Authentication required |
| 404 | Progress record not found |

---

**Endpoint: POST /api/v1/behavioral-consistency/progress**
Descripción: Crea un nuevo registro de progreso conductual para el usuario autenticado.
Authorization: Bearer JWT requerido.
Responses:

| Código | Descripción |
|--------|-------------|
| 201 | Behavioral progress created |
| 400 | Invalid request data |
| 401 | Authentication required |

---

**Bounded Context: Analytics**

**Endpoint: GET /api/v1/analytics/{userId}**
Descripción: Obtiene el dashboard analítico completo del usuario, incluyendo métricas consolidadas y línea de tiempo de adherencia conductual.
Authorization: Bearer JWT requerido.
Responses:

| Código | Descripción |
|--------|-------------|
| 200 | Analytics dashboard returned |
| 401 | Authentication required |
| 404 | Analytics record not found |

---

**Bounded Context: Subscriptions**

**Endpoint: GET /api/v1/subscriptions/{userId}**
Descripción: Obtiene la suscripción activa del usuario.
Authorization: Bearer JWT requerido.
Responses:

| Código | Descripción |
|--------|-------------|
| 200 | Subscription returned |
| 401 | Authentication required |
| 404 | Subscription not found |

**Endpoint: PUT /api/v1/subscriptions/{id}**
Descripción: Actualiza el plan de suscripción del usuario (upgrade o downgrade). No realiza procesamiento de pagos real en este sprint.
Authorization: Bearer JWT requerido.
Responses:

| Código | Descripción |
|--------|-------------|
| 200 | Subscription updated |
| 400 | Invalid plan data |
| 401 | Authentication required |

#### 5.2.3.7. Software Deployment Evidence for Sprint Review

Durante este sprint se realizó el despliegue del backend de NutriSmart en Coolify, utilizando el repositorio `nutrismart-platform` como fuente de despliegue continuo y el dominio `smart-api.nutriproject.xyz` como punto de acceso público a la API. A continuación se describen los pasos realizados.

**Creación y configuración del Dockerfile**

Se agregó un Dockerfile multi-stage al repositorio `nutrismart-platform`. La primera etapa compila el proyecto con Maven y la segunda etapa construye la imagen final sobre una base de Java 21-slim, copiando únicamente el JAR generado. Esto reduce el tamaño de la imagen final y acelera el despliegue.

**Configuración de rama bajo Gitflow**

Se mantuvo la estructura de ramas existente siguiendo Gitflow:
- `main` → rama de producción (fuente de despliegue)
- `develop` → rama de integración
- `feature/*` → ramas de desarrollo por bounded context

Todo el trabajo fue integrado mediante Pull Requests desde las ramas `feature/*` hacia `develop`, y finalmente desde `develop` hacia `main` como parte de la release `v1.1.3`.

**Actualización de CORS para integración con frontend**

Se actualizó la configuración de CORS en la clase `WebMvcConfigurer` del proyecto para aceptar peticiones desde el dominio `https://app-smart.nutriproject.xyz`, permitiendo el consumo del API desde el frontend desplegado en el Sprint 2.

**Configuración del despliegue en Coolify**

Para habilitar el despliegue continuo desde el repositorio se siguieron los pasos:

1. Ingresar al panel de administración de Coolify
2. Crear una nueva aplicación seleccionando **GitHub** como fuente
3. Conectar el repositorio `nutrismart-platform` de la organización `upc-pre-202610-1asi0729-17952-devteam`
4. Configurar los parámetros de build con Dockerfile
5. Configurar las variables de entorno de producción (credenciales de base de datos MySQL, secreto JWT, credenciales Gmail, API keys de DeepSeek y OpenWeatherMap)
6. Asignar el dominio personalizado `smart-api.nutriproject.xyz` en la sección **Domains**
7. Guardar la configuración y ejecutar el primer despliegue manual

**URLs de despliegue**

| Recurso | URL |
|---------|-----|
| API Backend | `https://smart-api.nutriproject.xyz` |
| Swagger UI | `https://smart-api.nutriproject.xyz/swagger-ui/index.html` |
| OpenAPI JSON | `https://smart-api.nutriproject.xyz/v3/api-docs` |
| Frontend Web App | `https://app-smart.nutriproject.xyz` |

#### 5.2.3.8. Team Collaboration Insights during Sprint

Durante el Sprint 3, todos los miembros del equipo participaron activamente en las actividades de implementación del backend, tal como se refleja en los analíticos de colaboración de GitHub. Los integrantes Nevatrix (Angel Villarreal), xJoelFMRx (Joel Mora), Emy127 (Angela Espinoza), olenkisha_14 (Olenka Del Aguila) y Brandon1677 (Brandon Soto) realizaron commits de manera constante a lo largo del sprint, cada uno liderando su bounded context asignado y colaborando en los aspectos transversales de configuración, CORS y despliegue.

![Insight](../assets/img/sprint3/insight.png)

## 5.3. Validation Interviews

### 5.3.1. Diseño de Entrevistas

**Objetivo de la entrevista:**

Los objetivos son de validar la usabilidad, efectividad y claridad de NutriSmart, asimismo de asegurar que los flujos de usuario(User flows) sean intuitivos, prácticos y funcionales para los usuarios y su correcta interaccion con la plataforma.

#### Segmento 1: Pérdida de peso

##### Estructura:

**Preguntas de introducción:**

1. ¿Cuál es su nombre?
2. ¿Cuántos años tiene?
3. ¿A qué se dedica?

**Preguntas de validación de la plataforma web:**



#### Segmento 2: Ganancia de masa muscular

##### Estructura:

**Preguntas de introducción:**

1. ¿Cuál es su nombre?
2. ¿Cuántos años tiene?
3. ¿A qué se dedica?

**Preguntas de validación de la plataforma web:**

1. ¿Te resultó fácil e intuitivo registrarte, rellenar tus datos y crear tu perfil en la plataforma?

2. ¿Hubo algo confuso o que te tomó tiempo entender?

3. ¿Qué actividades planeabas realizar al ingresar a la plataforma?

4. ¿Cuál es tu opinión sobre la funcionalidad de registro nutricional?

5. ¿Te resultaron adecuadas las recomendaciones personalizadas ofrecidas por la plataforma?

6. ¿Cómo te sentiste al visualizar tu progreso corporal?

7. ¿Consideras útil y de sencilla visualización la información brindada en analítica?

8. ¿Tienes alguna sugerencia o recomendación para mejorar la plataforma y mejorar la experiencia a futuros usuarios?

9. ¿Recomendarías NutriSmart a tus familiares o amigos? ¿Por qué?

### 5.3.2. Registro de Entrevistas

#### Segmento 1: Pérdida de peso

##### Entrevista 1:

- Nombres y Apellidos: Jorge Del Aguila Vacalla
- Edad: 49 
- Ocupación: Administrador de empresas y jefe de garantías y taller
- Tiempo: 0:01 - 4:56
- Link: [Link de las entrevistas](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202411669_upc_edu_pe/IQBWpfwIabIbTastqBaS_0gfAZZ2EhRrlW8BOVJAI1rZcuo?e=ZRy0a2&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifSwicGxheWJhY2tPcHRpb25zIjp7InN0YXJ0VGltZUluU2Vjb25kcyI6MS42M319)
- Resumen: Jorge destacó el impacto visual de las imágenes y la variedad de verduras presentadas en la plataforma. Valoró significativamente la facilidad y practicidad del registro nutricional, así como la funcionalidad que le permite visualizar en detalle las calorías, proteínas, carbohidratos, grasas y fibras consumidas. Consideró que la analítica es útil y de fácil acceso para cualquier tipo de usuario. Sugirió mejoras específicas como la inclusión de videos de ejercicios básicos de bajo impacto y testimonios de usuarios que hayan logrado resultados. Finalmente, recomendaría la plataforma a sus conocidos debido a su practicidad y utilidad en el seguimiento del progreso de pérdida de peso.

![E1S1 - Capture](../assets/img/chapter5-interviews/Entrevista1-S1.png)

##### Entrevista 2:

- Nombres y Apellidos: Tatiana Mozombite Miranda
- Edad: 25 
- Ocupación: Estudiante de idiomas
- Tiempo: 4:57 - 9:13
- Link: [Link de las entrevistas](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202411669_upc_edu_pe/IQBWpfwIabIbTastqBaS_0gfAZZ2EhRrlW8BOVJAI1rZcuo?e=vcmCTI&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifSwicGxheWJhY2tPcHRpb25zIjp7InN0YXJ0VGltZUluU2Vjb25kcyI6Mjk3LjU3fX0%3D)
- Resumen: Tatiana encontró el procedimiento general intuitivo y fácil de entender. Aprecio las funcionalidades presentadas como Smart Scan y Nutricion Gobal, considerándolas útiles para su objetivo. Valoró los precios accesibles de los planes. Durante la configuración inicial, no presentó dificultades en la comprensión de datos personales ni restricciones alimentarias. Resaltó especialmente la sección de porcentajes de macronutrientes que le ayuda a identificar qué debería consumir. La visualización del progreso corporal le pareció motivadora y de utilidad para reforzar su meta. Recomendaría la plataforma a familiares y amigos por su innovación y facilidad para mantener una vida saludable en el día a día.

![E2S1 - Capture](../assets/img/chapter5-interviews/Entrevista2-S1.png)

##### Entrevista 3:

- Nombres y Apellidos: Larisa Ramírez Del Aguila
- Edad: 19 
- Ocupación: Estudiante de Administración y Marketing
- Tiempo: 9:14 - 13:28
- Link: [Link de las entrevistas](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202411669_upc_edu_pe/IQBWpfwIabIbTastqBaS_0gfAZZ2EhRrlW8BOVJAI1rZcuo?e=CmhPWz&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifSwicGxheWJhY2tPcHRpb25zIjp7InN0YXJ0VGltZUluU2Vjb25kcyI6NTUyLjU1fX0%3D)
- Resumen: Larisa encontró la plataforma especialmente intuitiva y moderna, destacando la claridad en el flujo de registro e inicio de sesión. Se mostró entusiasmada con las recomendaciones personalizadas basadas en el clima y ubicación, considerándolas prácticas para su estilo de vida actual. Valoró la funcionalidad de agregar ingredientes disponibles en casa para recetas personalizadas, viéndola como una ventaja económica. El dashboard principal le pareció visualmente atractivo y fácil de interpretar para monitorear su progreso diario. Sugirió mejoras en la gamificación de objetivos y mayor variedad de contenido educativo sobre nutrición básica. Expresó su disposición a recomendar la plataforma a sus compañeras de universidad por su diseño amigable y funcionalidades adaptadas a jóvenes adultos con objetivos de bienestar.

![E3S1 - Capture](../assets/img/chapter5-interviews/Entrevista3-S1.png)

#### Segmento 2: Ganancia de masa muscular

##### Entrevista 1:

- Nombres y Apellidos: David Miguel Ramos Parihuamán
- Edad: 19
- Ocupación: Estudiante universitario
- Tiempo: 13:29 - 17:11
- Link: [Link de las entrevistas](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202411669_upc_edu_pe/IQBWpfwIabIbTastqBaS_0gfAZZ2EhRrlW8BOVJAI1rZcuo?e=tQffZK&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifSwicGxheWJhY2tPcHRpb25zIjp7InN0YXJ0VGltZUluU2Vjb25kcyI6ODA5LjA1fX0%3D)
- Resumen: David señalo la facilidad y semejanza que posee el registro e inicio de sesión con plataformas de su uso diario. Mostro interés por la funcionalidad de registro nutricional, las recomendaciones personalizadas y como lo ayudan en su progreso diario. Dio recomendaciones sobre la interfaz a fin de mejorar la experiencia para futuros usuarios.

![E1S2 - Capture](../assets/img/chapter5-interviews/Entrevista1-S2.png)

##### Entrevista 2:

- Nombres y Apellidos: Rando Lopez Mayta
- Edad: 22
- Ocupación: Estudiante universitario
- Tiempo: 17:12 - 21:50
- Link: [Link de las entrevistas](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202411669_upc_edu_pe/IQBWpfwIabIbTastqBaS_0gfAZZ2EhRrlW8BOVJAI1rZcuo?e=T3aD5D&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifSwicGxheWJhY2tPcHRpb25zIjp7InN0YXJ0VGltZUluU2Vjb25kcyI6MTAzMi40M319)
- Resumen: Rando menciona que le resulto fácil e intuitivo el registro e inicio de sesión a la plataforma. A pesar de un corto periodo de uso, señala que está encantado con las funcionalidades de registro nutricional y la visualización del progreso. Sugiere mayores opciones de personalización para las interfaces, y finaliza considerando que recomendaria la plataforma a todos sus conocidos.

![E2S2 - Capture](../assets/img/chapter5-interviews/Entrevista2-S2.png)

##### Entrevista 3:

- Nombres y Apellidos: Daphne Faustor
- Edad: 25
- Ocupación: Community Manager en el área de marketing (rubro gastronómico aeroportuario)
- Tiempo: 21:51 - 29:13
- Link: [Link de las entrevistas](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202411669_upc_edu_pe/IQBWpfwIabIbTastqBaS_0gfAZZ2EhRrlW8BOVJAI1rZcuo?e=Cbgv8X&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifSwicGxheWJhY2tPcHRpb25zIjp7InN0YXJ0VGltZUluU2Vjb25kcyI6MTMxMS41Nn19)
- Resumen: Daphne Faustor evaluó la plataforma con un objetivo enfocado en ganar masa muscular. Consideró que el registro es sumamente intuitivo y personalizado, y destacó como un gran acierto que el sistema calcule automáticamente las calorías y porciones diarias para evitar procesos tediosos. Asimismo, valoró positivamente las recomendaciones adaptadas al clima y la función de despensa por la practicidad que aportan al día a día, así como los paneles de analítica para monitorear su evolución. Finalmente, recomendó incorporar testimonios de usuarios para aumentar la motivación y afirmó que recomendaría la aplicación a amigos y familiares para concientizarlos sobre la importancia de comer en las proporciones correctas sin restricciones innecesarias.

![E3S2 - Capture](../assets/img/chapter5-interviews/Entrevista3-S2.png)

### 5.3.3. Evaluaciones según heurísticas

#### UX Heuristics & Principles Evaluation
**Usability – Inclusive Design – Information Architecture**

| Campo | Detalle |
|---|---|
| **CARRERA** | Ingeniería de Software |
| **CURSO** | Desarrollo de Aplicaciones Open Source |
| **SECCIÓN** | 17952 |
| **PROFESORES** | Todos |
| **AUDITOR** | PircaIndustries |
| **CLIENTE** | Francia Torres, Jhony Manuel; Montoya Nina, Paula Fernanda; Pareja Calloapaza, Marcelo Fausto; Ramos Hinostroza, Diego Antonio y Ramos Mera, Neo Daniel. |

---

##### Site o App a evaluar
**NutriSmart**

---

##### Tareas a evaluar
El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:

1. Landing Page
2. Registro e Inicio de Sesión
3. Proceso de Onboarding
4. Suscripción
5. Dashboard
6. Registro Nutricional
7. Recomendaciones
8. Progreso Corporal
9. Actividad Física
10. Analítica y Progreso
11. Configuración

**No incluidas en esta versión de la evaluación:**

- Ninguna, se revisaron todas.

---

##### Escala de severidad
Los errores serán puntuados tomando en cuenta la siguiente escala de severidad:

| Nivel | Descripción |
|:---:|---|
| **1** | Problema superficial: puede ser fácilmente superado por el usuario o ocurre con muy poca frecuencia. No necesita ser arreglado a no ser que exista disponibilidad de tiempo. |
| **2** | Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja para resolverlo de cara al siguiente release. |
| **3** | Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlo. Es importante que sea corregido y se le debe asignar una prioridad alta. |
| **4** | Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento. |

---

##### Tabla resumen

| # | Problema | Severidad | Heurística / Principio violada(o) |
|:---:|---|:---:|---|
| 1 | Etiqueta de contraseña sin traducir al español. | 2 | Consistencia y estándares. |
| 2 | Logotipo ilegible por falta de resolución y contraste. | 1 | Diseño estético y minimalista. |
| 3 | Ícono de selección sin margen y pegado al borde. | 1 | Diseño estético y minimalista. |
| 4 | Ausencia de opción para omitir suscripción. | 4 | Control y libertad del usuario. |
| 5 | Falta de botón de retroceso en el flujo de pago. | 3 | Control y libertad del usuario. |
| 6 | Desaparición del selector de idioma durante el pago. | 2 | Consistencia y estándares. |
| 7 | Proximidad riesgosa entre botón de acción y campos sensibles. | 2 | Prevención de errores. |
| 8 | Área de interacción limitada en el menú de usuario. | 3 | Flexibilidad y eficiencia de uso. |
| 9 | Falta de retroalimentación inmediata en eliminación. | 4 | Visibilidad del estado del sistema. |
| 10 | Legibilidad deficiente por tamaño de fuente. | 1 | Diseño estético y minimalista. |
| 11 | Desbordamiento visual y falta de contención en el menú desplegable de selección de actividad. | 2 | Usabilidad – Control del usuario / Diseño minimalista y estético; Diseño Inclusivo – Jerarquía visual. |
| 12 | Elemento interactivo ambiguo y no autoexplicativo ("No wearable"). | 2 | Usabilidad – Visibilidad del estado del sistema, relación entre el sistema y el mundo real; Arquitectura de la Información – Rotulado. |
| 13 | Bloqueo de la interfaz y error persistente al exportar reporte PDF. | 3 | Usabilidad – Libertad y control del usuario, Prevención de errores y Visibilidad del estado del sistema. |
| 14 | Estado vacío no interactivo ni accionable en el gráfico de evolución de peso. | 2 | Usabilidad – Ayuda a reconocer, diagnosticar y recuperarse de errores; Diseño Inclusivo – Orientación y guía al usuario. |
| 15 | Errores críticos de reproducción y carga en los videos del producto y del equipo. | 3 | Usabilidad – Visibilidad del estado del sistema / Prevención de errores. |
| 16 | Plagio de marca y contradicción de identidad en recursos gráficos. | 3 | Usabilidad – Relación entre el sistema y el mundo real / Consistencia y estándares. |
| 17 | Alta complejidad y falta de predictibilidad en el acceso a la internacionalización (i18n). | 2 | Usabilidad – Flexibilidad y eficiencia de uso; Arquitectura de la Información – Sistemas de navegación. |

---

##### Descripción de problemas

##### PROBLEMA #1: Etiqueta de contraseña sin traducir al español
- **Severidad:** 2
- **Heurística violada:** Consistencia y estándares.
- **Problema:** El texto "show" dentro del campo de la contraseña (para revelar los caracteres) se mantiene en inglés a pesar de que la interfaz está configurada en español, rompiendo la uniformidad del sistema.
- **Recomendación:** Traducir la etiqueta de acción a "Mostrar" y "Ocultar" cuando la internacionalización de la aplicación esté configurada en español.

##### PROBLEMA #2: Logotipo ilegible por falta de resolución y contraste
- **Severidad:** 1
- **Heurística violada:** Diseño estético y minimalista.
- **Problema:** El logotipo de NutriSmart carece de la nitidez, tamaño o contraste adecuado, lo que impide que el usuario lo visualice y reconozca correctamente.
- **Recomendación:** Reemplazar el recurso gráfico por una imagen de mayor resolución o ajustar sus dimensiones (ancho y alto) para que el elemento principal de marca sea legible.

##### PROBLEMA #3: Ícono de selección sin margen y pegado al borde
- **Severidad:** 1
- **Heurística violada:** Diseño estético y minimalista.
- **Problema:** El ícono (signo) para desplegar las opciones en el campo de "sexo biológico" carece de margen interno y está excesivamente pegado al borde del contenedor de texto.
- **Recomendación:** Añadir espaciado (padding/margin) entre el ícono de despliegue y los bordes del campo de selección para mejorar el diseño visual y evitar dar la impresión de saturación.

##### PROBLEMA #4: Ausencia de opción para omitir suscripción
- **Severidad:** 4
- **Heurística violada:** Control y libertad del usuario.
- **Problema:** El sistema obliga al usuario a elegir un plan de suscripción para avanzar, sin proporcionar un botón para rechazar la oferta o seleccionar una opción gratuita. Adicionalmente, si el pago es un requisito obligatorio del modelo de negocio, esta condición no se informa desde el inicio, haciendo que el usuario pierda tiempo ingresando datos previamente.
- **Recomendación:** Añadir un botón o enlace visible que indique "Omitir" o "Continuar con plan gratuito". En caso de que la aplicación sea estrictamente de pago, se debe mostrar un aviso claro de los costos en la pantalla de bienvenida o antes del registro.

##### PROBLEMA #5: Falta de botón de retroceso en el flujo de pago
- **Severidad:** 3
- **Heurística violada:** Control y libertad del usuario.
- **Problema:** Tras seleccionar un plan o avanzar a la sección de pago, la interfaz carece de un botón de retroceso. Esto impide que el usuario pueda enmendar su acción si desea cancelar la compra o cambiar a otro plan de suscripción.
- **Recomendación:** Implementar un botón de "Atrás" o "Cancelar" en una zona visible de la cabecera (header) que permita regresar a la pantalla anterior sin perder la información ya ingresada.

##### PROBLEMA #6: Desaparición del selector de idioma durante el pago
- **Severidad:** 2
- **Heurística violada:** Consistencia y estándares.
- **Problema:** El botón o menú para cambiar el idioma desaparece durante el flujo de pago, impidiendo mantener una experiencia uniforme con las pantallas previas donde sí estaba disponible.
- **Recomendación:** Mantener el selector de idiomas anclado en la misma posición a lo largo de todas las pantallas de la aplicación, incluyendo el flujo de finalización de compra.

##### PROBLEMA #7: Proximidad riesgosa entre botón de acción y campos sensibles
- **Severidad:** 2
- **Heurística violada:** Prevención de errores.
- **Problema:** El botón de "Continuar revisión" se encuentra visualmente muy cerca de los campos de entrada sensibles ("fecha de vencimiento" y "CVV"), lo que aumenta el riesgo de que el usuario lo presione accidentalmente antes de terminar de escribir.
- **Recomendación:** Aumentar la separación vertical (margin-top) del botón de "Continuar revisión" respecto a los campos del formulario para reducir el riesgo de envíos incompletos o errores de interacción física.

##### PROBLEMA #8: Área de interacción limitada en el menú de usuario
- **Severidad:** 3
- **Heurística violada:** Flexibilidad y eficiencia de uso.
- **Problema:** La zona interactiva para acceder a "Profile" y "Log out" es excesivamente reducida, limitándose exclusivamente al texto. En dispositivos con pantallas pequeñas, esta restricción dificulta la precisión táctil del usuario, impidiendo que el recuadro contenedor funcione como un área de interacción efectiva.
- **Recomendación:** Implementar un menú desplegable (dropdown) para centralizar estas acciones. Asimismo, ampliar el área de clic o toque para que abarque la totalidad del recuadro del usuario, facilitando la navegación en entornos con resoluciones pequeñas.

##### PROBLEMA #9: Falta de retroalimentación inmediata en eliminación
- **Severidad:** 4
- **Heurística violada:** Visibilidad del estado del sistema.
- **Problema:** Al interactuar con el botón de eliminación ("X") en la sección de ingredientes, el sistema no refleja ningún cambio inmediato en la interfaz. El usuario se ve forzado a recargar la página manualmente o navegar a otra sección para validar la eliminación, lo que genera incertidumbre sobre la ejecución de la acción.
- **Recomendación:** Gestionar correctamente la asincronía del proceso. Es fundamental incluir una retroalimentación visual inmediata tras la confirmación.

##### PROBLEMA #10: Legibilidad deficiente por tamaño de fuente
- **Severidad:** 1
- **Heurística violada:** Diseño estético y minimalista.
- **Problema:** El tamaño de la fuente de varias secciones presenta un tamaño reducido que no se ajusta adecuadamente a la resolución de pantalla. Esta falta de jerarquía tipográfica dificulta la lectura fluida.
- **Recomendación:** Ajustar la escala tipográfica mediante el uso de unidades relativas como `rem`, permitiendo que el tamaño de fuente sea adaptable según la resolución.

##### PROBLEMA #11: Desbordamiento visual y falta de contención en el menú desplegable de selección de actividad
- **Severidad:** 2
- **Heurística violada:** Usabilidad – Control del usuario / Diseño minimalista y estético; Diseño Inclusivo – Jerarquía visual.
- **Problema:** Al desplegar la lista de actividades para registrar un ejercicio, el contenedor se expande verticalmente de manera desmedida, sobrepasando los límites inferiores del modal e intersecando con el fondo translúcido. Esto genera una superposición visual deficiente y dificulta la navegación para usuarios con pantallas de menor resolución o en dispositivos móviles, donde el listado podría quedar cortado o ser difícil de desplazar.
- **Recomendación:** Limitar la altura máxima del menú desplegable mediante estilos en el frontend e incorporar una barra de desplazamiento interna (scrollbar). Adicionalmente, dado que la lista es muy extensa, se aconseja agregar un campo de búsqueda rápida de texto dentro del desplegable para permitir al usuario escribir y filtrar la actividad en lugar de realizar un desplazamiento largo.

##### PROBLEMA #12: Elemento interactivo ambiguo y no autoexplicativo ("No wearable")
- **Severidad:** 2
- **Heurística violada:** Usabilidad – Visibilidad del estado del sistema, relación entre el sistema y el mundo real; Arquitectura de la Información – Rotulado.
- **Problema:** El elemento "No wearable" (que incluye el ícono de un reloj inteligente) se muestra junto al botón principal de registro. Su diseño visual es idéntico al de un botón, pero al interactuar con él, no queda claro si permite vincular un dispositivo, si es un simple indicador de estado inactivo, o si es un botón deshabilitado. La falta de claridad y de respuesta interactiva confunde al usuario sobre cómo automatizar la carga de sus entrenamientos.
- **Recomendación:** Rediseñar el componente. Si su objetivo es permitir la vinculación de un reloj inteligente, el rotulado debe ser una llamada a la acción clara (ej. "Conectar dispositivo" o "Sincronizar Reloj"). Si solo actúa como un indicador pasivo de estado, debe tener un estilo visual diferenciado de los botones activos (por ejemplo, una etiqueta de estado o "badge") y acompañarse de un tooltip explicativo al pasar el cursor (ej. "No hay ningún dispositivo inteligente vinculado para importar entrenamientos automáticamente").

##### PROBLEMA #13: Bloqueo de la interfaz y error persistente al exportar reporte PDF
- **Severidad:** 3
- **Heurística violada:** Usabilidad – Libertad y control del usuario, Prevención de errores y Visibilidad del estado del sistema.
- **Problema:** Al interactuar con la opción de exportación y presionar "Generar PDF" en cualquier rango de fechas, el sistema del frontend entra en un estado de falla crítica que despliega un mensaje generalizado de error ("Failed to load analytics. Please try again."). Este error se propaga tanto en el fondo de la pantalla de analíticas como dentro de la ventana emergente. El usuario queda atrapado en este estado de bloqueo y la única forma de restablecer la vista es cambiar forzadamente de sección mediante el menú de navegación lateral (sidebar) y retornar a la sección de analíticas. Esto frustra el flujo del usuario y rompe la libertad de control del estado de navegación.
- **Recomendación:** Implementar un manejo de excepciones localizado para la exportación de reportes. Si la generación del PDF falla, el mensaje de error debe mostrarse exclusivamente dentro del contexto de la ventana emergente, sin alterar el estado del panel principal de analíticas en segundo plano.

##### PROBLEMA #14: Estado vacío no interactivo ni accionable en el gráfico de evolución de peso
- **Severidad:** 2
- **Heurística violada:** Usabilidad – Ayuda a los usuarios a reconocer, diagnosticar y recuperarse de errores; Diseño Inclusivo – Orientación y guía al usuario.
- **Problema:** Cuando no se disponen de registros de peso en el rango de fechas seleccionado, el frontend despliega el mensaje estático "Not enough weight data to display the chart." Este es un estado vacío (empty state) pasivo que no proporciona ningún enlace o botón de llamada a la acción (CTA) para que el usuario pueda registrar o actualizar su peso directamente, obligándolo a buscar en otras secciones del sistema para resolver el problema.
- **Recomendación:** Convertir el estado vacío en una zona interactiva y accionable. Se sugiere agregar un botón directo dentro de la tarjeta (por ejemplo: "Registrar peso actual") que redirija al usuario directamente a la sección de registro o despliegue un formulario de actualización de peso.

##### PROBLEMA #15: Errores críticos de reproducción y carga en los videos del producto y del equipo
- **Severidad:** 3
- **Heurística violada:** Usabilidad – Visibilidad del estado del sistema / Prevención de errores.
- **Problema:** En las secciones "About the Product" y "Meet Our Team", los contenedores multimedia incrustados muestran un mensaje de error crítico de la plataforma de origen ("Se produjo un error. Vuelve a intentarlo más tarde..."). Esto impide por completo que el usuario acceda a los videos demostrativos y testimoniales del producto, quebrantando la confianza en el sitio y limitando la información clave sobre la aplicación.
- **Recomendación:** Verificar y corregir los identificadores (IDs) de los videos en el código fuente de la Landing Page, asegurando que los enlaces apunten a recursos públicos válidos en YouTube o Microsoft Stream.

##### PROBLEMA #16: Plagio de marca y contradicción de identidad en recursos gráficos
- **Severidad:** 3
- **Heurística violada:** Usabilidad – Relación entre el sistema y el mundo real / Consistencia y estándares.
- **Problema:** En la sección "About Us", el grupo afirma que la plataforma se llama NutriSmart. Sin embargo, la imagen circular decorativa de la derecha contiene explícitamente el logotipo y el nombre de "NutriSense" (una empresa e identidad de software real y completamente ajena al proyecto). Esto rompe la correspondencia con el mundo real, confunde al usuario sobre la legitimidad del sitio y evidencia una falta de cuidado crítica (o plagio de recursos) en la maquetación.
- **Recomendación:** Reemplazar este recurso gráfico por uno propio que corresponda al rotulado e identidad de marca oficial del proyecto (NutriSmart).

##### PROBLEMA #17: Alta complejidad y falta de predictibilidad en el acceso a la internacionalización (i18n)
- **Severidad:** 2
- **Heurística violada:** Usabilidad – Flexibilidad y eficiencia de uso; Arquitectura de la Información – Sistemas de navegación.
- **Problema:** El cambio de idioma de la plataforma está excesivamente oculto para el usuario, obligándolo a realizar un flujo largo e intuitivamente complejo ("Ver perfil" => "Language" => "Elegir idioma"). Al ser el Dashboard el panel principal de control, no contar con un acceso directo o un selector rápido en el header o barra lateral penaliza la eficiencia de uso, especialmente para usuarios internacionales que necesitan adaptar la interfaz desde el primer contacto.
- **Recomendación:** Desacoplar el selector de idioma de las configuraciones profundas del perfil e integrarlo directamente como un botón de acceso rápido o menú desplegable (dropdown) en el Header principal o en la parte inferior del Sidebar lateral.


## 5.4. Video About-the-Product

### Descripción General

Esta sección presenta el Video About-the-Product, una herramienta de comunicación estratégica diseñada para dos públicos objetivo principales. En primer lugar, se dirige a los visitantes del Landing Page que desean conocer sobre el modelo de negocio y las características principales de la solución de software NutriSmart. En segundo lugar, se enfoca en los usuarios de la aplicación web que buscan comprender cómo realizar tareas específicas relacionadas con los procesos soportados por la plataforma.

El tono de comunicación utilizado es consistente con la identidad del producto: motivacional, directo y cercano, buscando transmitir confianza y facilidad de uso.

---

### Video

**Captura del Video:**

![Video About-the-Product - NutriSmart](../assets/img/chapter5-video/about-the-product.png)

---

### Información del Video

| Atributo | Contenido |
|----------|-----------|
| **Duración** | 2:20 minutos |
| **Microsoft Stream** | https://upcedupe-my.sharepoint.com/:v:/g/personal/u202417857_upc_edu_pe/IQBZsJjpaxFpSIn7Vna2BKZDAWDoPUpVPvQbJ1kLrhkd3f0 |

---

### Resumen del Video

El video inicia con un problema relatable para la audiencia: la dificultad de mantener una alimentación saludable sin saber qué comer ni cómo medir el progreso. Inmediatamente presenta a NutriSmart como la solución que transforma objetivos nutricionales en planes concretos y personalizados desde el primer día.

La propuesta de valor se desarrolla de manera progresiva, mostrando cómo el usuario puede configurar su perfil en minutos y acceder a funcionalidades clave. El proceso de registro de alimentos es presentado como simple e inmediato, destacando que NutriSmart calcula automáticamente calorías y macronutrientes en tiempo real, permitiendo correcciones sobre la marcha.

Se enfatizan las recomendaciones inteligentes basadas en la ubicación y disponibilidad de ingredientes, eliminando la incertidumbre sobre si un alimento encaja en el plan nutritivo. El video también muestra la integración con actividad física, el seguimiento del progreso corporal y un panel de analítica que visualiza la evolución a lo largo del tiempo.

Un elemento clave es la gamificación de la consistencia, presentando al usuario como alguien que puede fallar sin culpa, simplemente retomando el camino con datos reales. El cierre refuerza el llamado a la acción con un mensaje inspirador: "Empieza gratis, define tu objetivo y deja que los datos te guíen. Porque comer bien no debería ser un misterio." La marca termina con su tagline: "NutriSmart: Tu nutrición, con inteligencia."

---

### Testimonios de Usuarios

El video incluye dos testimonios de usuarios reales que participaron en las entrevistas de validación, proporcionando credibilidad y validación del impacto real del producto:

> "Empecé a usar NutriSmart hace dos meses con el objetivo de bajar 8 kilos. Lo que más me sorprendió fue que no me decía solo 'come menos', sino exactamente qué comer cada día. Perdí 5 kilos y por primera vez entiendo mi alimentación."
>
> **David R., usuario NutriSmart, segmento pérdida de peso**

> "Entreno hace años pero siempre fallaba en la nutrición. Con NutriSmart empecé a darle seguimiento real a mis proteínas y en 6 semanas noté una diferencia visible en músculo. Es la herramienta que me faltaba."
>
> **Jorge D. A., usuario NutriSmart, segmento ganancia muscular**
