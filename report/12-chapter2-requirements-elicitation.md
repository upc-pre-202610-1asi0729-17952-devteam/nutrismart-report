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

Las entrevistas fueron diseñadas con preguntas diferenciadas según cada segmento objetivo, organizadas en bloques temáticos que permiten recopilar información sobre el perfil del usuario, sus hábitos actuales y la validación de las funcionalidades propuestas.

<center>

|Enlace del video|
|---|
|https://upcedupe-my.sharepoint.com/:v:/g/personal/u202411669_upc_edu_pe/IQAaTWbVFrGSQJbryk1mXrvuAaOFuJ0aZVDyTHY-va1m7t0?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=SjFO2r|

</center>

##### Segmento 1 — Pérdida de Peso (Adultos de 25 a 60 años)

**Bloque 1: Perfil y biografía**

1. ¿Cuál es su nombre, edad y a qué se dedica?
2. ¿Cómo describiría su rutina diaria en cuanto a movimiento físico? ¿Diría que es una persona que pasa mucho tiempo sentada, o que se mueve bastante durante el día?

**Bloque 2: Control calórico y conocimiento nutricional**

3. ¿Tiene alguna meta física actualmente, como bajar de peso o mejorar su alimentación? ¿Qué es lo que más le cuesta lograr?
4. Cuando come fuera de casa, en un restaurante, en la calle o en el trabajo, ¿sabe con certeza cuánto está comiendo en términos de calorías, o simplemente calcula una cifra aproximada?

**Bloque 3: Validación de funciones**

5. Si una aplicación pudiera analizar la foto de su plato o del menú de un restaurante y decirle automáticamente qué tan saludable es esa comida para usted, ¿la usaría? ¿Por qué?
6. ¿Le parecería útil que la aplicación le sugiera qué comer según el clima del día, por ejemplo, algo más ligero cuando hace mucho calor, o algo más sustancioso cuando hace frío?

##### Segmento 2 — Ganancia de Masa Muscular (Jóvenes de 18 a 32 años)

**Bloque 1: Perfil y biografía**

1. ¿Cuál es tu nombre, edad y a qué te dedicas?
2. ¿Con qué frecuencia entrenas a la semana y hace cuánto tiempo llevas haciéndolo?
3. ¿Qué dispositivos usas normalmente? ¿Tienes smartwatch, reloj deportivo o algún accesorio que te mida los pasos o el ejercicio?

**Bloque 2: Macros, adaptabilidad y contexto**

4. ¿Llevas algún control de lo que comes, especialmente de cuánta proteína consumes al día? ¿Qué es lo que más te incomoda de las aplicaciones que has probado para registrar tu comida?
5. Cuando viajas o tu rutina cambia por algún motivo, trabajo, viaje, eventos, ¿cómo afecta eso tu alimentación y tu entrenamiento?

**Bloque 3: Validación de funciones**

6. Si estuvieras de viaje en una ciudad que no conoces y una aplicación te sugiriera automáticamente platos típicos de esa zona que encajan con tu dieta, ¿lo usarías? ¿Qué te parecería eso?
7. Si tu reloj o tu celular midiera automáticamente cuánto te moviste en el día y la aplicación ajustara sola cuánto deberías comer ese día según eso, ¿qué valor le darías a esa función?


### 2.2.2. Registro de entrevistas

#### Segmento 1: Personas que buscan perder peso


**Entrevista 1: Evelyn Del Aguila Díaz**

<center>

![Entrevista 1 Seg1](../assets/img/interviews/1_1.png)

</center>

- **Nombre y Apellidos:** Evelyn Del Aguila
- **Edad:** 54 años
- **Ocupación:** Docente universitaria de idiomas
- **Tiempo:** 0:01 - 3:48

Evelyn describe su rutina diaria como permanentemente activa debido a su labor docente, la cual le exige estar en constante movimiento entre clases y actividades con sus alumnos. Su motivación para buscar un mejor control alimenticio nace de preocupaciones de salud, específicamente por el aumento de peso relacionado con la edad y niveles elevados de azúcar, por lo cual cuenta actualmente con asesoría de un nutricionista. Al comer fuera de casa, no conoce el valor calórico exacto, pero aplica una estrategia de control basada en evitar la repetición de carbohidratos y equilibrar las proteínas y verduras. Ella califica como una "idea magnífica" la posibilidad de usar una aplicación que analice sus platos mediante fotografías, ya que le permitiría contar con una herramienta de apoyo precisa para el control riguroso de su ingesta diaria. Asimismo, aprueba totalmente la función de sugerencias según el clima como un complemento útil para su alimentación.

**Entrevista 2: Jorge Del Aguila**

<center>

![Entrevista 2 Seg1](../assets/img/interviews/1_2.png)

</center>

- **Nombre y Apellidos:** Jorge Del Aguila
- **Edad:** 49 años
- **Ocupación:** Administrador de empresas y jefe de garantías y taller
- **Tiempo**: 3:49 - 8:09

Jorge es un profesional cuya jornada laboral transcurre mayoritariamente en una oficina, permaneciendo sentado aproximadamente el 90% de su tiempo, mientras que el resto lo dedica a la coordinación en taller. A pesar de este sedentarismo laboral, mantiene una rutina de ejercicio nocturno de lunes a viernes con el objetivo de combatir su sobrepeso actual mediante un déficit calórico. En cuanto a su alimentación, suele consumir menús diarios calculando las porciones de manera visual o "al ojo", sin tener certeza sobre el valor calórico real de sus platos. Se muestra muy interesado en utilizar una herramienta tecnológica que analice su metabolismo y las fotos de su comida, asegurando que, de ser efectiva, la recomendaría a su círculo cercano. Respecto a las sugerencias por clima, aunque vive en una zona predominantemente cálida, considera que podrían ser útiles en momentos específicos de lluvia para elegir alimentos como café o sándwiches.

**Entrevista 3: Daniela Larisa Ramírez**

<center>

![Entrevista 3 Seg1](../assets/img/interviews/1_3.png)

</center>

- **Nombre y Apellidos:** Larisa Ramírez
- **Edad:** 19 años
- **Ocupación:** Estudiante de Administración y Marketing
- **Tiempo**: 8:08 - 12:08

Daniela mantiene una rutina mayoritariamente sedentaria debido a sus estudios universitarios, aunque intenta realizar pausas activas y camina diariamente hacia el transporte público. Su principal desafío para perder peso y mejorar su alimentación es un diagnóstico médico de Síndrome de Ovario Poliquístico (SOP), lo cual dificulta la pérdida de peso y le genera constantes antojos de alimentos poco saludables. Al igual que los otros entrevistados, suele medir sus porciones de forma estimada cuando come en restaurantes, pero carece de información calórica real. Ella utilizaría la aplicación propuesta para mantener la disciplina en su alimentación, especialmente cuando sale a comer fuera. Además, destaca que la función de sugerencias por clima sería muy innovadora, mencionando que durante el invierno suele sentir más hambre y deseos de consumir dulces, por lo que una guía adecuada le ayudaría a evitar alimentos que no son saludables.

#### Segmento 2: Personas con metas de ganancia de masa muscular

**Entrevista 1: David Ramos**

<center>

![Entrevista 1 Seg2](../assets/img/interviews/2_1.png)

</center>

- **Nombre y Apellidos:** David Miguel Ramos Parihuamán
- **Edad:** 19 años
- **Ocupación:** Estudiante universitario
- **Tiempo:** 12:10 - 16:08

David es un estudiante universitario que entrena en el gimnasio de dos a tres veces por semana con el objetivo de aumentar su masa muscular, proceso que inició hace aproximadamente dos meses. Su mayor dificultad para mantener la constancia radica en los viajes y en las alteraciones de su rutina debidas a responsabilidades académicas y laborales, lo que le complica identificar alimentos locales adecuados y mantener su ritmo de entrenamiento fuera de su entorno habitual. Actualmente monitorea sus pasos con un smartwatch y sigue una dieta basada en las recomendaciones de sus instructores para controlar calorías y proteínas. David ve en la aplicación propuesta una solución para reducir la carga mental durante sus viajes, valorando especialmente las sugerencias de platos típicos adaptados a su dieta y el ajuste automático de porciones según su actividad física, lo cual le permitiría regular su alimentación con precisión incluso cuando sus estudios le impiden asistir al gimnasio.

**Entrevista 2: Rando López**

<center>

![Entrevista 2 Seg2](../assets/img/interviews/2_2.png)

</center>

- **Nombre y Apellidos:** Rando López
- **Edad:** 22 años
- **Ocupación:** Estudiante universitario
- **Tiempo:** 16:09 - 19:09

Rando es un joven universitario que entrena cuatro veces por semana con el enfoque de ganar masa muscular. Su principal desafío es la gestión del tiempo, ya que sus deberes académicos suelen interferir con su capacidad para asistir al gimnasio y ajustar su ingesta calórica diaria. Aunque ya utiliza tecnología como un smartwatch para medir pasos y pulsaciones, y lleva un control manual de sus proteínas, manifiesta que las aplicaciones de nutrición convencionales le resultan confusas o poco atractivas. Considera que la aplicación propuesta sería de gran valor para mantener su disciplina, destacando la importancia de contar con sugerencias de gastronomía local que encajen con su dieta al viajar. Asimismo, resalta como una herramienta fundamental la automatización en el ajuste de porciones basada en la actividad física registrada por sus dispositivos, lo que facilitaría significativamente el seguimiento de su régimen alimenticio.

**Entrevista 3: Daphne Faustor**

<center>

![Entrevista 3 Seg2](../assets/img/interviews/2_3.png)

</center>

- **Nombre y Apellidos:** Daphne Faustor
- **Edad:** 25 años
- **Ocupación:** Profesional en Comunicaciones, Marketing y Publicidad
- **Tiempo:** 19:10 - 23:01

Daphne es una profesional con una rutina física exigente de cinco a seis días de entrenamiento semanal enfocados en fuerza y cardio. A pesar de su alta disciplina, enfrenta obstáculos significativos en el manejo del tiempo y el estrés que le genera el pesaje meticuloso de alimentos, especialmente la distinción entre peso en crudo y cocido, práctica que decidió abandonar tras un periodo de déficit estricto. Actualmente prioriza el consumo proteico pero busca una alternativa de monitoreo nutricional menos demandante. Ve en la aplicación un aliado estratégico para resolver el "dilema del viajero", donde la comida saludable suele ser escasa o costosa frente a la comida chatarra, apreciando la función de platos típicos que permita disfrutar la cultura local sin comprometer sus metas. Finalmente, considera fundamental la integración con su Apple Watch para el ajuste automático de macronutrientes, lo que le permitiría mantener sus objetivos en "piloto automático" dentro de su ajetreada vida profesional.

### 2.2.3. Análisis de entrevistas

#### Segmento 1: Personas que buscan perder peso

El análisis integral de las entrevistas realizadas al Segmento Objetivo 1 revela una homogeneidad total en la necesidad de herramientas de control calórico: el 100% de los participantes busca perder peso o mejorar su salud, pero desconoce los valores nutricionales exactos de los alimentos consumidos fuera del hogar. Existe una clara diferencia generacional y situacional en las motivaciones. Mientras que los adultos mayores de 40 años se enfocan en el control metabólico preventivo y la salud clínica, como niveles elevados de azúcar o sobrepeso derivado del sedentarismo laboral, el perfil joven enfrenta obstáculos fisiológicos específicos como el SOP y la gestión de la ansiedad alimentaria vinculada a antojos.

En términos de comportamiento tecnológico, se identifica una apertura absoluta hacia el uso de la cámara del dispositivo móvil como interfaz principal para el análisis nutricional. Todos los entrevistados validaron la utilidad de la fotografía para obtener exactitud en el control de ingesta, lo que sugiere que la facilidad de uso es un factor crítico para el éxito de la herramienta. Un hallazgo relevante es la validación unánime de la funcionalidad de recomendaciones según el clima; este factor no solo se percibe como una novedad, sino como una respuesta a disparadores psicológicos y físicos reales, como el aumento del apetito en climas fríos o la necesidad de hidratación y ligereza en climas cálidos.

Finalmente, el análisis demuestra que el segmento requiere una solución que trascienda el simple conteo de calorías, buscando un soporte que se adapte a estilos de vida variados, desde el sedentarismo de oficina hasta la actividad docente, y que ofrezca un respaldo educativo sobre la composición de los platos. La influencia del entorno y las condiciones de salud preexistentes actúan como los principales movilizadores para la adopción de la plataforma, consolidando a este segmento como usuarios potenciales que valoran la precisión, la innovación en la personalización y el acompañamiento constante en sus metas físicas.

#### Segmento 2: Personas con metas de ganancia de masa muscular

El análisis de las entrevistas realizadas al Segmento Objetivo 2 revela una homogeneidad absoluta en la adopción de tecnología vestible: el 100% de los participantes utiliza dispositivos como smartwatches o Apple Watch para monitorear su actividad física. A diferencia de otros segmentos, este grupo no busca únicamente perder peso, sino una optimización de macronutrientes que se adapte a un estilo de vida de alto rendimiento y alta demanda de tiempo. Existe un consenso en que el mayor obstáculo para la disciplina no es la falta de voluntad, sino la fricción generada por factores externos como la carga académica y laboral, los cuales interrumpen la regularidad de sus entrenamientos y su planificación alimentaria.

En el ámbito tecnológico, se identifica un rechazo hacia las aplicaciones de nutrición tradicionales por ser percibidas como confusas o excesivamente demandantes en cuanto al registro manual de datos. Los entrevistados valoran la automatización como el diferencial de mayor valor en la propuesta, específicamente la capacidad de la aplicación para ajustar porciones y macronutrientes de forma reactiva a la actividad física del día. Esto evidencia que el usuario de este segmento busca soluciones que operen en "piloto automático", eliminando la carga mental y el estrés asociado al pesaje meticuloso de alimentos, y permitiendo que la nutrición se integre de forma fluida con sus dispositivos de salud preexistentes.

Finalmente, surge un patrón crítico relacionado con la alimentación fuera de casa y los viajes, identificado como el "dilema del viajero". Los tres participantes coinciden en que viajar representa un punto de quiebre en su progreso debido a la dificultad para encontrar opciones saludables y al desconocimiento de la gastronomía local en términos nutricionales. La validación de una función que sugiera platos típicos locales alineados a sus metas nutricionales confirma que este segmento busca una herramienta que les otorgue libertad y flexibilidad cultural sin sacrificar sus objetivos físicos, consolidando la necesidad de una plataforma que funcione tanto como monitor inteligente de actividad como guía gastronómico personalizado.

## 2.3. Needfinding

### 2.3.1. User Personas

### 2.3.2. User Task Matrix

### 2.3.3. User Journey Mapping

### 2.3.4. Empathy Mapping

## 2.4. Big Picture EventStorming

## 2.5. Ubiquitous Language