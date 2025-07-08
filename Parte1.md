# 🧩 Guía de Estudio - Parte 1 del Examen (Preguntas y Respuestas)

---

## 1. ¿Cuáles serían las variables dependientes, independientes e intervinientes en un experimento para evaluar una nueva web de compras con IA?

La variable independiente sería el rediseño de la web o el uso del sistema inteligente (por ejemplo, recomendador personalizado). La variable dependiente podría ser el tiempo de permanencia en el sitio, el número de clics o las conversiones. Las variables intervinientes pueden incluir el perfil del usuario (edad, experiencia tecnológica), la hora del día o el dispositivo utilizado. Diseñar el experimento requiere establecer dos grupos (A/B), controlar las variables externas y medir objetivamente los resultados.

---

## 2. ¿Qué roles incluirías en el equipo de desarrollo de un chatbot con PLN y cómo organizarías el trabajo?

Incluiría roles como científico de datos (para entrenar el modelo de lenguaje), ingeniero de backend (para desplegar la API), diseñador UX (para flujos de conversación), experto en dominio (para el contenido) y un gestor de proyecto. Se trabajaría con metodología ágil, organizando tareas en sprints, con entregables iterativos como versiones del bot, pruebas de usuario y ajustes semánticos. La comunicación clara y la integración continua serían claves para el éxito.

---

## 3. Describe una estrategia para mantener actualizado y monitorizado un modelo de detección de fraude en una entidad financiera.

Se implementaría un pipeline de MLOps con: ingesta de nuevos datos, validación de calidad, test automático del modelo, reentrenamiento bajo ciertas condiciones (como cambio en la distribución), y despliegue continuo (CI/CD). La monitorización incluiría métricas de precisión y alerta ante caída de rendimiento o aumento de falsos negativos. Además, se usaría un dashboard con logs, control de versiones de modelo y procesos de rollback ante errores.

---

## 4. ¿Cómo afectan los datos sesgados a un sistema de reconocimiento facial y qué estrategias se pueden aplicar para corregirlo?

Los datos sesgados afectan la generalización del sistema. Si los datos de entrenamiento contienen mayoritariamente rostros de un grupo étnico o género, el sistema puede fallar en otros grupos. Para mitigarlo, se deben usar datasets balanceados, técnicas de fairness-aware learning, auditorías algorítmicas y validación cruzada con subgrupos. La transparencia sobre los datos usados también es clave.

---

## 5. ¿Por qué es importante garantizar la explicabilidad de un sistema de IA utilizado en el diagnóstico médico?

La explicabilidad permite que los profesionales médicos entiendan por qué el sistema sugiere un diagnóstico, lo que facilita su aceptación y validación. Además, es necesaria para detectar errores, justificar decisiones y evitar responsabilidad legal por decisiones incorrectas. Herramientas como SHAP o LIME ayudan a visualizar qué variables han sido determinantes. Un sistema opaco, aunque preciso, podría no ser confiable sin explicabilidad.

---

## 6. ¿Qué ventajas ofrece aplicar el método científico en la planificación de un proyecto de IA educativo?

Aplicar el método científico permite diseñar hipótesis comprobables (por ejemplo, “los estudiantes con tutoría IA rinden un 20% más”), organizar el experimento (grupos control y tratamiento), y analizar resultados con métricas como notas o retención. Esto proporciona rigurosidad, objetividad y la posibilidad de replicar el estudio. Además, ayuda a justificar decisiones ante revisores o financiadores.

---

## 7. ¿Qué medidas tomarías para evitar la reidentificación de usuarios en un sistema que procesa datos sensibles?

Usaría técnicas de anonimización como agregación, eliminación de atributos clave o hashing irreversible. Además, evitaría datos de localización o tiempo precisos que puedan correlacionarse con la identidad. Aplicaría el principio de privacidad por diseño, solo recolectando lo estrictamente necesario y controlando accesos. También documentaría el riesgo residual asumido y las medidas de mitigación implementadas.

---

## 8. ¿Qué tipo de aprendizaje usarías para un sistema que analiza imágenes satelitales agrícolas, y por qué?

Usaría aprendizaje supervisado si dispongo de etiquetas (por ejemplo, tipo de cultivo o grado de madurez). Técnicas como redes convolucionales permiten segmentar o clasificar regiones. Si no hay etiquetas, optaría por aprendizaje no supervisado (como clustering) para agrupar patrones similares. La elección depende de la disponibilidad de datos y del objetivo: detección de anomalías, predicción de rendimiento o mapeo de zonas.

---

## 9. ¿Qué criterios aplicarías para evaluar el rendimiento de un modelo de predicción de abandono escolar?

Aplicaría métricas como F1-score, recall y AUC-ROC, especialmente si las clases están desbalanceadas. También usaría validación cruzada y analizaría falsos negativos (estudiantes que se abandonan pero no fueron detectados). Evaluaría la robustez del modelo en diferentes centros y cohortes, y si es posible, mediría el impacto real en la toma de decisiones (por ejemplo, intervención temprana).

---

## 10. ¿Cómo aplicarías el principio de explicabilidad en un modelo de IA que recomienda productos a usuarios?

Aunque el impacto puede ser menor que en medicina, la explicabilidad sigue siendo importante para ganar confianza y evitar sesgos ocultos. Se pueden mostrar explicaciones simples (“te recomendamos esto porque compraste X”) o usar técnicas como LIME para entender los factores que más pesaron. También es útil para mejorar el modelo y detectar errores en los datos o en las reglas de negocio.

---

## 11. ¿Qué desafíos éticos presenta el uso de datos históricos para entrenar modelos de selección de personal?

Los datos históricos pueden reflejar decisiones sesgadas (por ejemplo, contratar mayoritariamente hombres). Si no se corrige, el modelo reproducirá esa discriminación. Además, puede haber falta de consentimiento informado sobre el uso original de esos datos. Se requiere una revisión ética de las variables utilizadas, auditorías periódicas, mecanismos de explicabilidad y transparencia ante los candidatos.

---

## 12. ¿Cómo se gestiona un proyecto de IA aplicando principios de metodología ágil?

El trabajo se organiza en sprints (ciclos de 1-2 semanas), con entregables incrementales: recolección de datos, primer modelo, evaluación preliminar, etc. Se hacen reuniones breves diarias (dailies), revisiones y retrospectivas. Las tareas se priorizan en un backlog y el equipo es multidisciplinar. Esta metodología permite adaptarse rápidamente a cambios en los datos, objetivos o resultados.

---

## 13. ¿Qué significa “code is the new law” en el contexto de algoritmos y responsabilidad?

Significa que el código —las reglas programadas en un sistema algorítmico— actúa como una forma de legislación: define lo que está permitido o no. Esto es relevante cuando los algoritmos toman decisiones que afectan personas, como en justicia o finanzas. Por eso, su diseño debe incorporar principios éticos, ser auditable, explicable y respetar marcos legales. El poder normativo del código exige transparencia y control.

---

## 14. ¿Cómo se evalúa la fiabilidad de un sistema de IA que se usa en conducción autónoma?

Se evalúa con métricas como tasa de error, tiempo de reacción, robustez ante condiciones adversas (lluvia, oscuridad), y capacidad de generalizar. Se usan simulaciones masivas y pruebas en carretera. Además, se audita el comportamiento en situaciones éticamente complejas. La fiabilidad también incluye aspectos de seguridad cibernética y resistencia a ataques adversarios.

---

## 15. ¿Qué papel cumple la gobernanza de datos en proyectos de IA en administración pública?

La gobernanza garantiza que los datos sean gestionados con calidad, seguridad y ética. Incluye definir quién accede a qué datos, con qué propósito, cómo se documentan y cómo se audita su uso. También implica cumplimiento legal (ej. GDPR), protección ante sesgos y trazabilidad. En administración pública, es clave para mantener la confianza ciudadana y asegurar justicia en las decisiones algorítmicas.

---

## 16. ¿Cómo puede una IA contribuir a la toma de decisiones judiciales sin reemplazar a los jueces?

La IA puede actuar como asistente que clasifica jurisprudencia, encuentra similitudes entre casos o sugiere posibles resoluciones basadas en precedentes. Sin embargo, la decisión final debe recaer en un juez humano. Para no reemplazar el juicio humano, el sistema debe ser explicable, trazable y ajustado a principios legales. También debe auditarse su funcionamiento regularmente y prohibirse su uso en decisiones críticas sin revisión.

---

## 17. ¿Por qué es preferible usar modelos explicables en educación frente a redes neuronales profundas?

En educación, es importante entender por qué un alumno es clasificado como “en riesgo” o por qué se recomienda cierto material. Los modelos explicables permiten que docentes o tutores comprendan y validen las decisiones, generando confianza y mejorando la intervención pedagógica. Las redes profundas pueden ser más precisas, pero difíciles de justificar ante una familia o un comité académico.

---

## 18. ¿Cómo contribuyen las ontologías al funcionamiento de un sistema cognitivo basado en IA?

Las ontologías estructuran el conocimiento: definen conceptos, relaciones y jerarquías. En un sistema cognitivo, permiten que la IA “entienda” el dominio (por ejemplo, medicina, educación) y razone con sentido. También facilitan la interoperabilidad con otros sistemas y mejoran la capacidad de responder preguntas complejas. Son especialmente útiles en sistemas expertos y asistentes conversacionales.

---

## 19. ¿Qué ventajas ofrece el aprendizaje federado en proyectos que manejan datos sensibles?

El aprendizaje federado permite entrenar modelos sin centralizar los datos. Los datos se quedan en sus dispositivos o instituciones, y solo se comparten actualizaciones de los modelos. Esto mejora la privacidad, reduce riesgos de fuga y permite cumplir con normativas como GDPR. Es útil en salud, banca o educación, donde los datos son confidenciales.

---

## 20. ¿Cómo usarías la estrategia de fairness-aware learning en un modelo de crédito bancario?

Aplicaría técnicas que penalicen desigualdades en el desempeño del modelo según grupos demográficos. Por ejemplo, ajustes en la función de pérdida para equilibrar false positives entre hombres y mujeres. También podría utilizar técnicas de preprocesamiento (remuestreo), inprocesamiento (algoritmos justos) o postprocesamiento (ajuste de scores). El objetivo es que el modelo sea igual de preciso sin discriminar por edad, género u origen.

---

## 21. ¿Cómo influye la calidad del dataset en la validez de un proyecto de investigación en IA?

La calidad del dataset es fundamental para garantizar que los resultados del modelo sean válidos y útiles. Datos incompletos, mal etiquetados o sesgados pueden llevar a conclusiones erróneas y comprometer la generalización del modelo. Es necesario evaluar el origen, limpieza, balance, y representatividad de los datos, ya que un modelo entrenado sobre datos deficientes producirá decisiones poco confiables y con potenciales riesgos sociales o éticos.

---

## 22. ¿Cuál es la diferencia entre una hipótesis descriptiva y una predictiva en un proyecto de IA?

Una hipótesis descriptiva busca observar y describir una relación entre variables, sin necesariamente anticipar un resultado. Por ejemplo, “los estudiantes con más participación obtienen mejores calificaciones”. En cambio, una hipótesis predictiva plantea una relación que será validada empíricamente mediante modelos, como “una red neuronal puede predecir el abandono escolar con un 90% de precisión”. La predictiva es más común en proyectos de IA por su enfoque experimental.

---

## 23. ¿Cómo se aplica el principio de transparencia en el desarrollo de proyectos de IA?

La transparencia exige que las decisiones tomadas durante el diseño, desarrollo y despliegue de un sistema de IA sean documentadas y comprensibles. Implica explicar cómo funciona el algoritmo, de dónde provienen los datos, qué métricas se usan y cómo se evalúa el sistema. También incluye informar a los usuarios si están interactuando con una IA, y permitir auditorías externas. Es esencial para garantizar confianza y responsabilidad en entornos sensibles como justicia, salud o educación.

---

## 24. ¿Qué problemas puede generar el sobreajuste en modelos de IA aplicados a educación?

El sobreajuste ocurre cuando un modelo aprende demasiado bien los patrones del conjunto de entrenamiento, incluso el ruido, y pierde capacidad de generalización. En educación, esto puede traducirse en sistemas que solo funcionan con una cohorte específica de estudiantes, generando intervenciones erróneas en nuevos contextos. Además, puede reforzar patrones no generalizables y comprometer decisiones pedagógicas. Es crucial aplicar regularización, validación cruzada y revisión continua.

---

## 25. ¿Qué factores considerarías para elegir entre aprendizaje supervisado y no supervisado en un proyecto?

La decisión depende de si se tienen etiquetas o no. Si contamos con datos clasificados (por ejemplo, éxito o fracaso escolar), usamos aprendizaje supervisado. Si no hay etiquetas pero queremos encontrar estructuras ocultas, como perfiles de usuarios, se aplica el no supervisado. Otros factores incluyen la cantidad de datos disponibles, la complejidad de la tarea y los recursos técnicos y humanos. A veces se combinan ambos enfoques.

---

## 26. ¿Qué características hacen que una investigación en IA sea considerada replicable?

Una investigación replicable debe documentar todo: datasets utilizados, código fuente, configuración de modelos, métricas, entorno de ejecución y semilla aleatoria. También se deben explicar claramente los pasos de preprocesamiento y criterios de evaluación. Publicar el código en repositorios abiertos y proporcionar instrucciones claras son prácticas clave. La replicabilidad fortalece la credibilidad científica y permite mejorar modelos existentes de forma colaborativa.

---

## 27. ¿Cuál es el impacto del sesgo de confirmación en la interpretación de resultados de IA?

El sesgo de confirmación puede llevar a que investigadores o equipos interpreten los resultados de un modelo de manera parcial, privilegiando las métricas que confirman sus expectativas y desestimando las que las contradicen. Esto puede resultar en modelos sobrevalorados, errores metodológicos no detectados, o decisiones basadas en supuestos equivocados. Para mitigarlo, es importante contrastar con líneas base, realizar pruebas A/B y fomentar revisiones por pares.

---

## 28. ¿Qué beneficios aporta el uso de simulaciones en fases tempranas de un proyecto de IA?

Las simulaciones permiten experimentar con escenarios hipotéticos sin los costos o riesgos asociados al uso de datos reales. Son útiles cuando los datos son escasos, confidenciales o costosos de obtener. Además, ayudan a validar hipótesis, probar modelos preliminares, optimizar parámetros y evaluar el rendimiento bajo diferentes condiciones. Son especialmente valiosas en educación, salud y transporte, donde las pruebas en entornos reales pueden ser delicadas.

---

## 29. ¿Cómo justificarías la elección de un tipo de red neuronal en un proyecto de clasificación de texto?

La elección depende del problema específico. Si se trata de clasificar opiniones o sentimientos en textos cortos, un modelo tipo LSTM o GRU puede captar dependencias temporales. Si se busca analizar contexto profundo en textos largos, modelos basados en Transformers como BERT ofrecen mejor rendimiento. También se consideran los recursos disponibles, la interpretabilidad y la experiencia del equipo. Justificar esta elección implica vincularla a la literatura y a las características del dataset.

---

## 30. ¿Qué función cumple la revisión bibliográfica en la definición del marco teórico de un proyecto de IA?

La revisión bibliográfica permite ubicar el problema en el estado del arte, evitar duplicaciones, identificar metodologías efectivas y vacíos de conocimiento. También orienta sobre qué métricas usar, qué modelos son más adecuados y qué problemas han sido previamente abordados. Una buena revisión aporta justificación teórica, enriquece la formulación de hipótesis y da credibilidad al planteamiento científico.

---

## 31. ¿En qué consiste la trazabilidad en un proyecto de IA y por qué es relevante?

La trazabilidad es la capacidad de seguir el rastro de todos los elementos del proyecto: desde los datos crudos hasta los resultados finales. Permite auditar decisiones, corregir errores, explicar resultados y asegurar la integridad del sistema. Es clave para la reproducibilidad, el cumplimiento regulatorio y la confianza de usuarios y autoridades. Incluye versionado de datasets, seguimiento de experimentos y documentación clara.

---

## 32. ¿Cómo puede una IA generar conocimiento nuevo en un campo científico?

La IA puede analizar grandes volúmenes de datos y detectar patrones que no son evidentes para los investigadores humanos. Esto permite generar hipótesis novedosas, descubrir relaciones ocultas y proponer nuevas líneas de investigación. Por ejemplo, modelos en biología han predicho interacciones entre proteínas aún no documentadas. La IA complementa la intuición científica y expande la frontera del conocimiento cuando se usa con sentido crítico y validación empírica.

---

## 33. ¿Por qué es importante evitar variables redundantes o colineales al entrenar un modelo?

Las variables redundantes no aportan nueva información y pueden aumentar el tiempo de entrenamiento, mientras que la colinealidad puede generar inestabilidad en modelos lineales, dificultando la interpretación y provocando varianzas elevadas en los coeficientes. Esto puede afectar negativamente el rendimiento del modelo y dar lugar a resultados engañosos. Técnicas como PCA, selección de características y análisis de correlación ayudan a detectarlas y eliminarlas.

---

## 34. ¿Qué riesgos éticos implica la hiperpersonalización basada en IA?

La hiperpersonalización puede generar burbujas informativas, sesgos reforzados y manipulación del comportamiento del usuario. También puede violar la privacidad si no se informa ni controla adecuadamente el uso de datos. En e-commerce, puede llevar a decisiones de compra basadas en presión algorítmica. Por tanto, debe garantizarse el consentimiento informado, la transparencia sobre el perfilado, y ofrecer mecanismos de control al usuario.

---

## 35. ¿Qué diferencias existen entre validación cruzada y validación holdout?

La validación holdout consiste en separar una porción fija de los datos para prueba, entrenando el modelo en el resto. Es rápida, pero sensible al azar del split. La validación cruzada (k-fold) divide el dataset en múltiples particiones, entrena en k-1 y prueba en 1, repitiendo k veces. Ofrece una estimación más robusta del rendimiento y reduce la varianza de la evaluación. Es preferible en proyectos donde se requiere rigor.

---

## 36. ¿Por qué es importante diseñar el proyecto con reproducibilidad desde el inicio?

Diseñar con reproducibilidad garantiza que los resultados puedan ser verificados y extendidos por otros. Esto incluye fijar semillas aleatorias, usar entornos virtuales controlados, documentar decisiones, versionar datos y compartir el código. La reproducibilidad no solo refuerza la credibilidad científica, sino que permite auditar el proceso, detectar errores y facilitar el trabajo colaborativo.

---

## 37. ¿Cómo afecta el uso de métricas inadecuadas a la evaluación de un modelo de IA?

El uso de métricas incorrectas puede dar una falsa impresión del rendimiento del modelo. Por ejemplo, en problemas desbalanceados, la accuracy puede ser alta aunque el modelo falle en detectar la clase minoritaria. Elegir métricas apropiadas (F1-score, precision-recall, AUC) según el objetivo y el contexto es crucial para una evaluación justa y útil. También se recomienda reportar varias métricas complementarias.

---

## 38. ¿Qué aporta la combinación de múltiples modelos (ensembles) a un proyecto de IA?

Los modelos de conjunto (ensembles) como Random Forest, XGBoost o modelos stacking combinan predicciones de varios modelos base para reducir el error y mejorar la estabilidad. Mitigan el riesgo de que un solo modelo esté sesgado o sobreajustado. Aunque requieren más recursos, ofrecen mejor generalización y suelen ganar en competencias prácticas como Kaggle. Son útiles en contextos críticos que exigen precisión robusta.

---

## 39. ¿Cómo se diferencia un sistema experto de una red neuronal en términos de conocimiento y explicabilidad?

Un sistema experto se basa en reglas explícitas creadas por humanos expertos. Su ventaja es la trazabilidad y la explicabilidad total. En cambio, una red neuronal aprende patrones complejos de forma automática, pero su funcionamiento interno es difícil de interpretar. En aplicaciones donde se requiere justificar decisiones (por ejemplo, medicina o derecho), se suele preferir la transparencia de sistemas expertos o usar modelos híbridos.

---

## 40. ¿Por qué es importante distinguir entre correlación y causalidad en análisis con IA?

La IA puede identificar correlaciones, pero eso no implica causalidad. Si no se distingue entre ambas, se pueden tomar decisiones erróneas. Por ejemplo, que los usuarios que compran paraguas también compren sopa no significa que uno cause el otro. Establecer causalidad requiere diseños experimentales, modelos estructurales o intervenciones controladas. Ignorar esta distinción puede llevar a sesgos, falsas atribuciones y modelos inútiles.

---
