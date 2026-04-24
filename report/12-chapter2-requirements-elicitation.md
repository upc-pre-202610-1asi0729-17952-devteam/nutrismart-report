# CAPÍTULO II: REQUIREMENTS ELICITATION & ANALYSIS

## 2.1. Competidores
El ecosistema de aplicaciones de bienestar en Perú se encuentra en un punto de inflexión, donde la saturación de herramientas globales choca con la creciente demanda de una experiencia más automatizada y adaptada a la realidad local. Si bien existen gigantes tecnológicos que han dominado el conteo de calorías por años, el usuario peruano se enfrenta constantemente a la fricción de bases de datos ajenas a nuestra gastronomía o interfaces que exigen un registro manual exhaustivo. En este escenario, **NutriSmart** no solo compite en funcionalidad, sino que busca resolver las brechas de personalización contextual y eficiencia que los líderes actuales han dejado desatendidas.

A continuación, se describen los tres competidores más relevantes:

- **MyFitnessPal:**
Es considerada la plataforma líder a nivel mundial en el seguimiento de nutrición y actividad física, destacando principalmente por poseer la base de datos de alimentos más extensa del mercado. Su enfoque es mayoritariamente cuantitativo y comunitario, permitiendo a los usuarios registrar calorías y macronutrientes de forma manual. Aunque es una herramienta poderosa, su interfaz puede resultar abrumadora para quienes buscan una experiencia minimalista o altamente automatizada mediante inteligencia artificial.
- **Fitia**
De origen peruano, esta aplicación ha ganado una tracción significativa en Latinoamérica al enfocarse en la generación de planes de alimentación automatizados que se ajustan a los objetivos específicos del usuario. A diferencia de las apps de conteo puro, Fitia propone qué comer basándose en la disponibilidad de ingredientes locales y recetas regionales. Se posiciona como un asistente nutricional directo que simplifica la planificación, siendo el competidor más cercano en cuanto a relevancia geográfica.
- **Cronometer**
Se distingue en el mercado por su rigor científico y la precisión extrema en el seguimiento no solo de calorías, sino de micronutrientes (vitaminas y minerales). Es la herramienta predilecta para usuarios con un perfil analítico avanzado, biohackers o atletas de alto rendimiento que requieren una integración profunda con biometría y dispositivos de salud. Su ventaja competitiva reside en la veracidad de su información nutricional, la cual es verificada por expertos, priorizando la exactitud sobre la rapidez del registro.

### 2.1.1. Análisis competitivo

<table border="2" cellspacing="0" cellpadding="5">
  <tr>
    <th colspan="7">Análisis Competitivo</th>
  </tr>
  <tr>
    <td colspan="2" rowspan="1">¿Por qué llevar a cabo este análisis?</td>
    <td colspan="5">Identificar características, funciones y estrategias similares y diferentes entre nuestro producto y 3 competidores clave.</td>
  </tr>
  <tr>
    <td colspan="3"></td>
    <td style="text-align: center;">
      NutriSmart<br>
      <img src="../assets/img/nutrismart-logo.png" alt="Logo NutriSmart" style="width:auto; height:100px;">
    </td>
    <td style="text-align: center;">
      MyFitnessPal<br>
      <img src="../assets/img/MyfitnessPal-Logo.jpg" alt="Logo MyFitnessPal" style="width:auto; height:100px;">
    </td>
    <td style="text-align: center;">
      Fitia<br>
      <img src="../assets/img/fitia-logo.png" alt="Logo Fitia" style="width:auto; height:100px;">
    </td>
    <td style="text-align: center;">
      Cronometer<br>
      <img src="../assets/img/cronometer-logo.png" alt="Logo Cronometer" style="width:auto; height:100px;">
    </td>
  </tr>
  <tr>
    <td rowspan="2">Perfil</td>
    <td colspan="2">Overview</td>
    <td>Plataforma SaaS con IA para registro visual y contexto real.</td>
    <td>Líder mundial basado en una base de datos masiva generada por usuarios.</td>
    <td>App enfocada en planes de alimentación con sabor local.</td>
    <td>Herramienta de alta precisión centrada en micronutrientes.</td>
  </tr>
  <tr>
    <td colspan="2">Ventaja competitiva ¿Qué valor ofrece a los clientes?</td>
    <td>Registro por fotos y recomendaciones según clima/ubicación.</td>
    <td>Base de datos de alimentos insuperable y comunidad global.</td>
    <td>Automatización de menús adaptados a la gastronomía local.</td>
    <td>Exactitud de datos verificada y seguimiento de salud profundo.</td>
  </tr>
  <tr>
    <td rowspan="2">Perfil de Marketing</td>
    <td colspan="2">Mercado objetivo</td>
    <td>Jóvenes y adultos peruanos (18-60 años).</td>
    <td>Público general global interesado en pérdida de peso.</td>
    <td>Población hispanohablante que busca planes de comida fáciles.</td>
    <td>Atletas, biohackers y personas con necesidades clínicas.</td>
  </tr>
  <tr>
    <td colspan="2">Estrategias de marketing</td>
    <td>Marketing a través de redes sociales y recomendación de usuarios.</td>
    <td>Alianzas con marcas deportivas y SEO de alto volumen.</td>
    <td>Marketing de contenidos y testimonios de transformación real.</td>
    <td>Podcasts de salud y foros de nutrición científica.</td>
  </tr>
  <tr>
    <td rowspan="3">Perfil de Producto</td>
    <td colspan="2">Productos & Servicios</td>
    <td>SaaS Web, escáner de menús e integración con wearables.</td>
    <td>App móvil, registro de ejercicio y recetas premium.</td>
    <td>App móvil, generador de listas de compras y recetas.</td>
    <td>App móvil y versión Pro para profesionales de la salud.</td>
  </tr>
  <tr>
    <td colspan="2">Precios & Costos</td>
    <td>Freemium (Suscripción mensual/anual proyectada).</td>
    <td>Freemium ($19.99/mes o $79.99/año aprox).</td>
    <td>Freemium (Suscripción premium accesible en soles).</td>
    <td>Freemium ($8.99/mes subscripcion Gold aprox).</td>
  </tr>
  <tr>
    <td colspan="2">Canales de distribución (Web y/o Móvil)</td>
    <td>Plataforma Web y App Móvil </td>
    <td>Móvil (iOS/Android) y Web.</td>
    <td>Principalmente Móvil (iOS/Android).</td>
    <td>Móvil y Web.</td>
  </tr>
  <tr>
    <td rowspan="5">Análisis SWOT</td>
  </tr>
  <tr>
    <td colspan="2">Fortalezas</td>
    <td>Innovación tecnológica (IA) y relevancia contextual local.</td>
    <td>Reconocimiento de marca y red social integrada.</td>
    <td>Curaduría de alimentos locales y facilidad de uso.</td>
    <td>Calidad de la información y detalle en micronutrientes.</td>
  </tr>
  <tr>
    <td colspan="2">Debilidades</td>
    <td>Marca nueva en fase de introducción.</td>
    <td>Muchos datos erróneos subidos por usuarios.</td>
    <td>Menor enfoque en el seguimiento de micronutrientes.</td>
    <td>Interfaz menos amigable para usuarios principiantes.</td>
  </tr>
  <tr>
    <td colspan="2">Oportunidades</td>
    <td>Crecimiento exponencial debido a innovaciones tecnológicas orientadas al usuario.</td>
    <td>Expansión a servicios de salud corporativos.</td>
    <td>Crecimiento en otros mercados de Latinoamérica.</td>
    <td>Crecimiento en el nicho de nutrición para longevidad.</td>
  </tr>
  <tr>
    <td colspan="2">Amenazas</td>
    <td>Copia de funciones por parte de competidores grandes.</td>
    <td>Surgimiento de nuevas apps gratuitas con IA básica.</td>
    <td>Apps de delivery integrando sus propios planes de salud.</td>
    <td>Cambios en las políticas de privacidad de datos médicos.</td>
  </tr>
</table>

### 2.1.2. Estrategias y tácticas frente a competidores

Diferenciación en el análisis de fotografías: Nosotros innovaríamos frente a nuestros competidores en los análisis de platos mediante fotos, ya que integraríamos IA para la rápida detección de alimentos, obtención de datos y además, generar estimaciones más acordes en base a la información obtenida, que resultara en recomendaciones más adecuadas para el usuario. Asimismo, se considera el escaneo y análisis de menú, un punto fuerte nuestro frente a la competencia, ya que recomendaría el platillo más acorde con el seguimiento nutricional del usuario, facilitando la elección.

Modelo freemium: Nuestro producto se adaptaría más a la realidad del sector y la economía de los usuarios, ofreciendo planes más accesibles y con las funciones de personalización básicas necesarias para un buen régimen nutricional. Además de ofrecer increíbles ventajas a través de funcionalidades en subscripciones de mayor rango.

Estrategia de Retención: Diferenciándonos de nuestros rivales en el mercado, NutriSmart ofrecería un ajuste dinámico contextual, lo que significa que las recomendaciones que se ofrecen hacia el usuario dependerán en gran medida de su contexto. Según el clima, ubicación o historial lo que se recomiende variará, ya que normalmente solo se realizan desde aspectos generales y sin profundizar en la conveniencia del usuario. Por lo que nosotros no solo mejoramos en este aspecto, sino cambiamos las reglas del juego, buscando el beneficio del consumidor.

Marketing y promoción: Es necesario comprender que debido a ser un producto nuevo y en crecimiento, se nos dificultará en un inicio rivalizar contra los competidores ya establecidos. Sin embargo, mediante estrategias de publicidad y marketing digital aumentaremos la visibilidad del producto, considerando también la publicidad indirecta gracias a recomendaciones de los usuarios y la expansión en círculos locales o comunidades que nos beneficiará en el crecimiento.

## 2.2. Entrevistas

### 2.2.1. Diseño de entrevistas

### 2.2.2. Registro de entrevistas

### 2.2.3. Análisis de entrevistas

## 2.3. Needfinding

### 2.3.1. User Personas

### 2.3.2. User Task Matrix

### 2.3.3. User Journey Mapping

### 2.3.4. Empathy Mapping

## 2.4. Big Picture EventStorming

## 2.5. Ubiquitous Language