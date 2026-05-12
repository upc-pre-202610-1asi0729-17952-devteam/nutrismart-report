# Conclusiones
 
## Conclusiones y Recomendaciones
 
### Conclusiones
 
#### Sobre los Problem Statements y los resultados obtenidos
 
El primero de los Problem Statements planteaba el registro manual de calorías como una carga que genera frustración y abandono temprano. Esta hipótesis quedó ampliamente validada durante el proceso de investigación: ninguno de los seis entrevistados realizaba un conteo calórico preciso en su vida diaria, todos operaban con estimaciones visuales o reglas heurísticas propias, precisamente porque el costo cognitivo del registro exacto superaba el beneficio percibido. El diseño de NutriSmart, centrado en el análisis visual de alimentos mediante fotografías y el Smart Scan, responde directamente a esta brecha. La solución propuesta reduce la fricción del registro al punto en que el usuario solo necesita tomar una foto para obtener datos nutricionales, lo que representa una transformación sustancial respecto al proceso manual tradicional.
 
El segundo Problem Statement señalaba que las aplicaciones existentes ignoran factores contextuales como la ubicación y el clima, generando desconexión entre el plan nutricional y la realidad del usuario. El análisis de entrevistas confirmó que este es uno de los quiebres más frecuentes: los usuarios fallan consistentemente fuera del hogar, no dentro de él. David y Rando, del segmento de ganancia muscular, identificaron los viajes como el detonante principal de abandono, y Daniela mencionó que el invierno incrementa sus antojos y que una guía contextual sería de gran utilidad. La arquitectura desarrollada para el Bounded Context de Smart Recommendations, con integración a OpenWeatherMap y APIs de geolocalización, valida técnicamente que esta capacidad es implementable, y los prototipos desarrollados demuestran que la experiencia de usuario para esta funcionalidad es intuitiva y accesible.
 
El tercer Problem Statement abordaba la dificultad de analizar menús en restaurantes como fuente de decisiones alimenticias incompatibles con los objetivos del usuario. Esta problemática fue transversal a ambos segmentos: todos los entrevistados coincidieron en que comer fuera de casa es el contexto de mayor riesgo nutricional. La funcionalidad de Restaurant Intelligence, materializada en el escaneo de menús físicos y el filtrado de platos según el perfil del usuario, constituye la respuesta más diferenciadora de NutriSmart frente a sus competidores directos como MyFitnessPal, Fitia y Cronometer, ninguno de los cuales ofrece esta capacidad de forma integrada con el perfil metabólico del usuario en tiempo real.
 
El cuarto Problem Statement planteaba la fragmentación de información entre herramientas de salud y plataformas de dieta como obstáculo para la visión del progreso real. Los entrevistados del segmento de ganancia muscular, particularmente Daphne y Rando, ya utilizaban wearables pero sin integración efectiva con su seguimiento nutricional. El diseño del Bounded Context de Metabolic Adaptation, con sincronización a Google Fit para usuarios Premium, cierra esta brecha al emitir ajustes automáticos del objetivo calórico diario en función de la actividad registrada, eliminando la necesidad de recalcular manualmente tras cada sesión de entrenamiento.
 
---
 
#### Sobre los Assumptions y el comportamiento real de los segmentos
 
Los Business Assumptions establecieron que los usuarios tienen necesidad de automatizar el seguimiento de dieta y ejercicio porque el registro manual genera alta tasa de abandono. Esta suposición se confirmó de manera contundente: los seis entrevistados exhibieron, sin excepción, comportamientos de abandono o simplificación extrema del registro en contextos de alta carga cognitiva o ruptura de rutina. El assumption fue conservador, ya que la realidad mostró que el abandono no es gradual sino abrupto y situacional, especialmente en el segmento de ganancia muscular.
 
El assumption que proyectaba que los usuarios iniciales serían jóvenes y adultos con metas de composición corporal y acceso a smartphones resultó preciso. Sin embargo, las entrevistas revelaron un matiz importante: el segmento de pérdida de peso abarca perfiles de mayor edad (Evelyn, 54 años, y Jorge, 49 años) con condiciones médicas preexistentes como niveles elevados de azúcar o SOP, lo que amplía la propuesta de valor de NutriSmart más allá del usuario fitness joven y demanda que la plataforma modele condiciones fisiológicas específicas, no solo objetivos estéticos.
 
El User Assumption que anticipaba que el quiebre nutricional ocurre fuera del hogar fue uno de los más sólidamente validados por el trabajo de campo. El análisis de entrevistas y la User Task Matrix revelaron que la tarea "decidir qué comer fuera de casa" es de alta frecuencia e importancia para ambos segmentos, mientras que el entorno doméstico representa un contexto controlado donde los usuarios mantienen mayor consistencia. Este hallazgo orientó correctamente el énfasis arquitectónico en el Restaurant Intelligence Context y las Smart Recommendations con datos geográficos.
 
El assumption sobre la reducción del tiempo de registro también fue validado positivamente. Los User Outcomes esperados, es decir, menos minutos dedicados a corroborar información nutricional, se materializan en el diseño de onboarding de NutriSmart, que consolida en un único flujo los datos de peso, talla, meta, alergias y condición médica, y en el Smart Scan que elimina la búsqueda manual de alimentos en bases de datos.
 
---
 
#### Sobre los Hypothesis Statements y los criterios de éxito
 
La primera hipótesis afirmaba que implementar análisis de alimentos por fotografía reduciría la tasa de abandono durante los primeros 30 días en al menos un 30% respecto a usuarios que solo usan búsqueda de texto. Las entrevistas del segmento de pérdida de peso confirman cualitativamente la dirección de esta hipótesis: Evelyn calificó la función de análisis fotográfico como una herramienta de apoyo de gran valor para su control riguroso diario, y Jorge indicó que la usaría y la recomendaría a su círculo cercano si resultaba efectiva. La validación cuantitativa del umbral del 30% requiere una fase de prueba con usuarios reales en producción, la cual debe priorizarse en el roadmap inmediato post-lanzamiento.
 
La segunda hipótesis planteaba que las sugerencias basadas en ubicación y clima permitirían que los usuarios mantuvieran su meta nutricional incluso al comer fuera de casa. El criterio de éxito, consistente en que el porcentaje de días en que se cumple el objetivo calórico fuera de casa sea comparable al de los días en casa, es ambicioso pero fundado en evidencia cualitativa sólida: cuatro de los seis entrevistados validaron esta funcionalidad como una solución directa a un problema real que experimentan frecuentemente. La integración con OpenWeatherMap y la geolocalización en el Bounded Context de Smart Recommendations establece la base técnica necesaria para medir este indicador una vez que la plataforma entre en operación.
 
La tercera hipótesis sostenía que el escaneo de menús físicos reduciría al menos un 40% los excesos calóricos o déficits de proteína en comidas fuera de casa. Este es el criterio de éxito más específico y medible del proceso Lean UX. La arquitectura del Restaurant Intelligence Context, con su capacidad de filtrar platos por restricciones y rankear opciones compatibles con el perfil del usuario, provee la instrumentación técnica necesaria para rastrear este indicador. Su validación dependerá de contar con una masa crítica de usuarios que utilicen el escaneo de menú con regularidad, lo que refuerza la importancia de diseñar la experiencia de esta funcionalidad para minimizar la fricción de activación.
 
La cuarta hipótesis afirmaba que la sincronización con relojes inteligentes reduciría la desviación calórica diaria a menos del 10% respecto al objetivo en días de actividad física intensa. El caso de Daphne, usuaria de Apple Watch con entrenamiento de cinco a seis días semanales, es el perfil de referencia para esta hipótesis. Su necesidad de mantener los objetivos en funcionamiento automático valida tanto la dirección de la hipótesis como el diseño del evento CaloricTargetAdjusted del Bounded Context de Metabolic Adaptation. El criterio del 10% de desviación será medible a través del módulo de Analytics & Reporting una vez que la sincronización con Google Fit esté operativa en el plan Premium.
 
---
 
#### Sobre los criterios de éxito del Lean UX
 
El criterio de negocio que proyectaba un crecimiento sostenido en la tasa de usuarios registrados mensualmente, validado por el valor de las recomendaciones personalizadas, encuentra sustento en el tamaño del mercado identificado: aproximadamente 3,87 millones de usuarios mensuales de aplicaciones de fitness y nutrición en Perú, de los cuales una proporción significativa no está satisfecha con las soluciones actuales dado el gap entre el 49% de peruanos que sigue algún tipo de restricción alimenticia y la penetración real de estas aplicaciones. El diferencial contextual y de personalización de NutriSmart, que abarca gastronomía local, clima y condiciones médicas, representa una propuesta de valor no atendida que puede traducirse en captación de usuarios insatisfechos con MyFitnessPal o Fitia.
 
El criterio de reducir el porcentaje de usuarios que abandonan sus regímenes nutricionales es el más directamente alineado con los hallazgos de campo. El patrón de abandono abrupto y situacional identificado en ambos segmentos sugiere que NutriSmart debe enfocar sus métricas de retención no en el uso diario promedio, sino en la recuperación del usuario tras episodios de ruptura de rutina: el Bounded Context de Behavioral Consistency, con su sistema de rachas y detección de caídas conductuales, está técnicamente diseñado para actuar exactamente en esos momentos críticos.
 
El criterio de conversión a planes superiores, proyectando más del 10% de usuarios que migran del plan básico a planes de mayor beneficio, depende directamente de que las funcionalidades Premium y Pro demuestren valor tangible antes de que el usuario alcance el límite del plan básico. El Smart Scan en planes Pro y la sincronización con Google Fit en Premium son las funcionalidades con mayor potencial de conversión según las preferencias expresadas por los entrevistados, especialmente en el segmento de ganancia muscular.
 
---
 
### Recomendaciones
 

---
 
## Video About-the-Team