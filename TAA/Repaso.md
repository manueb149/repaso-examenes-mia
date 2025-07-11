# 🗓️ Clase del 21 de marzo de 2025

### 📚 Tema: Introducción al aprendizaje automático

---

### 🎯 **Objetivos de la clase:**

1. Presentar el enfoque y estructura general de la asignatura.
2. Introducir los conceptos fundamentales del aprendizaje automático.
3. Establecer la terminología básica y la importancia del preprocesamiento de datos.
4. Explicar las expectativas de trabajo y el formato del examen.

---

### 🧠 **Contenidos tratados (resumen teórico + explicaciones del profesor):**

#### ✅ 1. ¿Qué es el aprendizaje automático (ML)?

* Se definió como la disciplina que **permite a los sistemas aprender a partir de datos sin ser programados explícitamente**.
* Se abordaron los **tres tipos principales**:

  * **Aprendizaje supervisado**: aprende a partir de datos etiquetados. Ej.: clasificación y regresión.
  * **Aprendizaje no supervisado**: trabaja sin etiquetas. Ej.: clustering.
  * **Aprendizaje por refuerzo**: basado en recompensas por acciones. Usado en agentes autónomos.

📌 **Comentario del profesor:**

> “Lo importante en supervisado es que se entrena un modelo a partir de ejemplos conocidos. La clave está en la relación entre las variables predictoras y la variable objetivo.”

---

#### ✅ 2. Componentes de un problema de aprendizaje supervisado

* **Entrada (X)**: conjunto de características o *features*.
* **Salida (y)**: variable objetivo (numérica o categórica).
* **Modelo**: función que intenta aprender la relación entre X e y.
* **Error o pérdida**: diferencia entre la predicción del modelo y el valor real.

El objetivo de un modelo es **minimizar el error**.

---

#### ✅ 3. Tipos de problemas supervisados

* **Clasificación**: la salida es una etiqueta o clase. Ej.: ¿es spam o no?
* **Regresión**: la salida es un valor numérico continuo. Ej.: ¿cuánto costará una casa?

📌 **Ejemplo discutido:**

> Predecir si un cliente cancelará un servicio → clasificación.
> Predecir el precio de un producto → regresión.

---

#### ✅ 4. Fases de un proyecto de ML (pipeline)

1. **Recolección y limpieza de datos**
2. **Análisis exploratorio (EDA)**
3. **Transformación y selección de características**
4. **Entrenamiento del modelo**
5. **Validación y evaluación**
6. **Implementación y mantenimiento**

📌 **Comentario del profesor:**

> “El preprocesamiento representa más del 70% del trabajo real. Un modelo bien entrenado con malos datos no servirá.”

---

#### ✅ 5. Representación y tipos de variables

* **Numéricas (continuas o discretas)**: edad, ingresos, temperatura.
* **Categóricas**: color, estado civil.
* **Binarias**: sí/no.
* **Ordinales**: bajo/medio/alto (tienen orden).

Es importante saber **cómo codificarlas** para que el modelo pueda utilizarlas.

---

#### ✅ 6. Introducción al tratamiento de datos

* **Valores nulos**: pueden eliminarse o imputarse.
* **Outliers**: identificarlos y tratarlos.
* **Normalización y estandarización**: para escalar valores y facilitar el entrenamiento.

📌 **Comentario del profesor:**

> “Si no escalas los datos, algunos modelos como SVM o regresión logística funcionarán mal.”

---

### 📝 Sobre la asignatura y el examen:

* Se indicó que la asignatura se evaluará con:

  * Una parte teórica de conocimiento (pregunta aplicada).
  * Preguntas tipo test.
  * Un ejercicio práctico.
  * Un análisis con razonamiento justificado.

📌 **Comentario importante:**

> “El examen **no requerirá código Python**, sino justificar el uso de modelos, técnicas o métricas.”

* También se mencionó que a lo largo del curso se proporcionarán:

  * PDFs de las sesiones.
  * Cuadernos de ejercicios.
  * Enlaces externos útiles.
  * Códigos de ejemplo con datos sintéticos.

---

### 📌 Ideas clave para repasar:

* Diferenciar bien entre **clasificación y regresión**.
* Tener claro el **pipeline de Machine Learning** y sus fases.
* Saber identificar y transformar tipos de variables.
* Recordar que **los datos mandan**: preprocesamiento y calidad son esenciales.
* Estudiar las **etapas del aprendizaje supervisado** y cómo un modelo minimiza el error.

Aquí tienes el **resumen detallado de la clase del 24 de marzo de 2025**, correspondiente a la segunda sesión del curso de *Técnicas de Aprendizaje Automático*. Esta clase continúa desarrollando el contenido del **Bloque 1**, con énfasis en el tratamiento de datos y la preparación de variables para el modelado.


# 🗓️ Clase del 24 de marzo de 2025

### 📚 Tema: Continuación del Bloque 1 — Tratamiento y transformación de datos

---

### 🎯 **Objetivos de la clase:**

1. Profundizar en el preprocesamiento de datos y su importancia en el rendimiento de los modelos.
2. Entender el tratamiento adecuado de variables categóricas y numéricas.
3. Conocer las transformaciones necesarias antes del entrenamiento.
4. Introducir conceptos de selección y generación de características.

---

### 🧠 **Contenidos tratados (teoría + aportes del profesor):**

---

#### ✅ 1. Revisión del concepto de aprendizaje automático supervisado

* Se repasan los conceptos de entrada (X), salida (y), modelo y error.
* Se recuerda la distinción entre problemas de clasificación y regresión.

📌 **Comentario del profesor:**

> “Siempre deben preguntarse: ¿qué tipo de variable tengo como salida? Eso les dirá si están frente a una regresión o clasificación.”

---

#### ✅ 2. Tratamiento de variables categóricas

* No pueden ser utilizadas directamente por modelos que requieren entrada numérica.
* **Técnicas principales:**

  * **One-hot encoding:** crea una columna binaria por cada categoría (para variables nominales sin orden).
  * **Label encoding:** asigna un número entero a cada categoría (adecuado solo si hay orden).
  * **Ordinal encoding:** útil cuando las categorías tienen jerarquía (ej.: bajo, medio, alto).

📌 **Advertencia del profesor:**

> “No codifiquen con números enteros si no hay orden en la categoría. Eso confunde al modelo.”

---

#### ✅ 3. Tratamiento de variables numéricas

* **Escalado:** importante para algoritmos sensibles a la magnitud (ej.: SVM, KNN, regresión logística).

  * **Min-Max Scaling:** transforma los valores al rango \[0,1].
  * **Z-score (standardization):** centra la media en 0 y la desviación estándar en 1.
* **Outliers:** deben identificarse y tratarse para evitar sesgos en el entrenamiento.

📌 **Comentario del profesor:**

> “Si usan SVM y no escalan, puede que el modelo falle estrepitosamente. No es opcional.”

---

#### ✅ 4. Detección y tratamiento de valores nulos

* Métodos:

  * Eliminación de filas o columnas con muchos valores nulos.
  * Imputación: media, mediana, moda o incluso modelos de predicción.

📌 **En clase se destacó:**

> “La imputación por mediana suele funcionar mejor si hay outliers. La media es sensible a ellos.”

---

#### ✅ 5. Generación y selección de características

* **Generación (Feature Engineering):** creación de nuevas variables a partir de las existentes (interacciones, combinaciones, transformaciones).
* **Selección:** elegir las variables más relevantes para el modelo.

  * Basada en estadísticas (correlación, ANOVA, chi-cuadrado).
  * Métodos automáticos (selección recursiva, regularización).

📌 **Comentario del profesor:**

> “Más variables no significa mejor modelo. Muchas veces empeoran el rendimiento si hay ruido.”

---

#### ✅ 6. Representación de datos en el entorno de desarrollo

* Breve mención a librerías como `pandas`, `scikit-learn` y `numpy`.
* Uso de DataFrames para manejo estructurado de datos.

---

### 📌 Ideas clave para repasar:

* Dominar el uso correcto de one-hot vs label encoding.
* Comprender por qué el escalado es fundamental para ciertos algoritmos.
* Saber cuándo imputar o eliminar datos faltantes.
* Reconocer el valor del *feature engineering* y la selección de variables.
* Identificar cómo los datos deben transformarse antes de alimentar un modelo.

---

### 📝 Consejos del profesor:

* Practicar con datasets pequeños para observar cómo las transformaciones afectan al modelo.
* Entender que **el preprocesamiento es parte esencial del aprendizaje automático**, no un paso opcional.
* Usar datos sintéticos para controlar variaciones y aprender el impacto de las decisiones de transformación.

Aquí tienes el **resumen detallado de la clase del 31 de marzo de 2025**, donde se inicia el **Bloque 2: Evaluación de modelos de aprendizaje supervisado**. Esta clase marca un punto de transición del preprocesamiento a la valoración formal de modelos, centrada en entender qué tan bien funciona un modelo y por qué.

# 🗓️ Clase del 31 de marzo de 2025

### 📚 Tema: Inicio del Bloque 2 — Evaluación de modelos de aprendizaje automático supervisado

---

### 🎯 **Objetivos de la clase:**

1. Comprender por qué es necesario evaluar los modelos y no confiar únicamente en la métrica global.
2. Introducir las métricas de evaluación para clasificación y regresión.
3. Explicar conceptos clave como matriz de confusión, sobreajuste y generalización.
4. Familiarizarse con errores comunes al evaluar modelos.

---

### 🧠 **Contenidos tratados (teoría + refuerzo del profesor):**

---

#### ✅ 1. ¿Por qué evaluar un modelo?

* El rendimiento en entrenamiento **no es garantía** de que el modelo generalice bien.
* La evaluación permite detectar **sobreajuste (overfitting)** o **subajuste (underfitting)**.
* Un buen modelo no es el que acierta todo en entrenamiento, sino el que se comporta bien con datos nuevos.

📌 **Comentario del profesor:**

> “Si tu modelo tiene 100% de acierto en entrenamiento, sospecha. Probablemente ha memorizado, no aprendido.”

---

#### ✅ 2. Conjunto de datos: partición

* Se divide el dataset en:

  * **Entrenamiento**
  * **Validación** (opcional)
  * **Test** (evaluación final del modelo)
* Introducción al **cross-validation (validación cruzada)** como técnica para evaluar con mayor robustez.

📌 **Explicación clave:**

> “La validación cruzada da una estimación más estable del rendimiento. Es lo que usamos para ajustar hiperparámetros.”

---

#### ✅ 3. Métricas para clasificación

* **Accuracy (exactitud):** proporción de aciertos.

  * ⚠️ Puede ser engañosa si las clases están desbalanceadas.
* **Precision:** qué proporción de los positivos predichos eran verdaderos.
* **Recall (sensibilidad):** qué proporción de positivos reales fueron capturados.
* **F1-score:** media armónica entre precision y recall (equilibrio).
* **Matriz de confusión:** tabla que compara las predicciones con los valores reales.

📌 **Comentario del profesor:**

> “No usen accuracy en datasets desbalanceados. Les dará una falsa sensación de éxito.”

---

#### ✅ 4. Métricas para regresión

* **MAE (Mean Absolute Error):** error promedio sin penalizar en exceso grandes errores.
* **MSE (Mean Squared Error):** penaliza más los errores grandes.
* **RMSE (Root MSE):** raíz cuadrada del MSE, en misma unidad que y.
* **R² (Coeficiente de determinación):** qué proporción de la varianza de y es explicada por el modelo.

📌 **Consejo del profesor:**

> “R² es muy intuitivo, pero puede ser engañoso si el modelo está mal especificado.”

---

#### ✅ 5. Overfitting y underfitting

* **Overfitting:** modelo demasiado complejo que aprende incluso el ruido.
* **Underfitting:** modelo demasiado simple que no logra capturar el patrón.

📌 **Ejemplo práctico en clase:**

> Comparación visual de curvas: un modelo que se ajusta exactamente a cada punto vs uno que captura la tendencia.

---

#### ✅ 6. Introducción al concepto de curva ROC y AUC

* **ROC (Receiver Operating Characteristic):** representa la relación entre TPR (recall) y FPR.
* **AUC (Área bajo la curva):** mide la capacidad del modelo para separar clases.

📌 **Nota del profesor:**

> “La AUC se vuelve muy útil cuando tenemos que comparar clasificadores distintos. Cuanto más cerca de 1, mejor.”

---

### 📌 Ideas clave para repasar:

* No quedarse solo con accuracy: entender en qué contexto es útil cada métrica.
* Saber interpretar una matriz de confusión.
* Aprender a elegir métricas según el problema: clasificación vs regresión.
* Entender por qué y cuándo usar validación cruzada.
* Tener claro el comportamiento del modelo frente a overfitting y underfitting.

---

### 📝 Comentarios adicionales del profesor:

* Las métricas serán parte **fundamental de la sección de análisis** en el examen.
* “Tienen que saber justificar por qué eligen una métrica y qué les está diciendo sobre el modelo.”
* Se anticipa que se presentarán **resultados de modelos reales** en ejercicios prácticos para ser interpretados.

Aquí tienes el **resumen completo y detallado de la clase del 7 de abril de 2025**, continuación del Bloque 2, centrada en la profundización de las **métricas de evaluación**, su interpretación y la conexión con el comportamiento del modelo en distintos contextos prácticos.

# 🗓️ Clase del 7 de abril de 2025

### 📚 Tema: Continuación del Bloque 2 — Evaluación de modelos de clasificación y regresión

---

### 🎯 **Objetivos de la clase:**

1. Profundizar en el uso e interpretación de métricas para clasificación y regresión.
2. Identificar cuándo una métrica es más adecuada que otra.
3. Introducir la validación cruzada (cross-validation) como método de evaluación.
4. Relacionar las métricas con decisiones prácticas y el rendimiento del modelo.

---

### 🧠 **Contenidos tratados (teoría + énfasis del profesor):**

---

#### ✅ 1. Evaluación de modelos de **clasificación**

* Se retoman las métricas principales:

  * **Precision:** útil cuando el coste de un falso positivo es alto (ej.: detección de fraude).
  * **Recall:** útil cuando no se deben perder positivos (ej.: detección de cáncer).
  * **F1-score:** equilibrio entre precision y recall.
* **Matriz de confusión** como herramienta para calcular todas estas métricas.

📌 **Comentario del profesor:**

> “Lo importante no es solo saber calcular el F1, sino saber **cuándo usarlo y cómo interpretarlo**.”

---

#### ✅ 2. Evaluación de modelos de **regresión**

* Revisión de métricas:

  * **MAE:** robusto frente a outliers, fácil de interpretar.
  * **MSE/RMSE:** penalizan errores grandes, útiles cuando se prioriza precisión fina.
  * **R²:** interpretabilidad intuitiva como proporción de varianza explicada.
* Se enfatiza que estas métricas **pueden dar resultados diferentes** y no hay una única mejor en todos los casos.

📌 **Explicación clave:**

> “No es lo mismo predecir el precio de casas que la temperatura. **El error tolerable depende del contexto**.”

---

#### ✅ 3. Validación cruzada (Cross-Validation)

* Técnica de evaluación más robusta que usar un solo conjunto de test.
* **K-Fold Cross Validation:** el dataset se divide en K partes; se entrena con K-1 y se prueba con la restante.
* Se calcula la métrica en cada iteración y se hace la media.

📌 **Comentario del profesor:**

> “La validación cruzada es **obligatoria** cuando haces tuning de hiperparámetros. Si no, estás sobreajustando al test.”

---

#### ✅ 4. Selección de métrica según el problema

* Para clasificación balanceada: accuracy puede ser razonable.
* Para clasificación desbalanceada: **mejor usar precision, recall, F1 o AUC.**
* Para regresión: **usar varias métricas** y comparar.

📌 **Ejemplo práctico del profesor:**

> “Imagina que predices si una pieza está defectuosa y solo el 1% lo están. Un accuracy del 99% puede ser basura.”

---

#### ✅ 5. Curvas ROC y AUC

* Se discute su uso cuando el modelo genera **probabilidades** en lugar de etiquetas.
* AUC mide la capacidad de un modelo para **distinguir entre clases**.
* ROC permite **comparar modelos** independientemente del umbral.

📌 **Nota del profesor:**

> “Es probable que en el examen les den una tabla de resultados o una curva. **Tienen que saber interpretarla.**”

---

#### ✅ 6. Métricas y coste de error

* Introducción a **análisis de coste-beneficio** de errores:

  * Falsos positivos vs falsos negativos.
  * Dependencia del problema real (negocios, salud, etc.).
* Se enfatiza que no hay métrica mágica, sino adecuada al **objetivo del sistema**.

📌 **Reflexión en clase:**

> “Un modelo no es bueno o malo por su F1-score, sino por **cómo impacta su error en la vida real**.”

---

### 📌 Ideas clave para repasar:

* Saber cuándo usar cada métrica.
* Entender las implicaciones de un alto recall vs alta precisión.
* Ser capaz de leer una matriz de confusión y extraer métricas de ella.
* Aplicar validación cruzada para evitar overfitting.
* Relacionar la métrica con el objetivo del problema (negocio, salud, industria, etc.).

---

### 📝 Consejos del profesor:

* “En el examen, si les dan una tabla con valores de precision y recall, **no digan cuál es mejor sin explicar por qué**.”
* Repasar ejemplos prácticos donde el modelo predice mal y justificar qué métrica sería más justa.
* Practicar interpretación de métricas en casos de clasificación desbalanceada.


Aquí tienes el **resumen completo y detallado de la clase del 22 de abril de 2025**, correspondiente al inicio del **Bloque 3: Modelos estadísticos y modelos no lineales**. Esta sesión marca el paso de la evaluación de modelos al estudio de los algoritmos de aprendizaje supervisado en sí, comenzando con los **modelos lineales y sus limitaciones**.

# 🗓️ Clase del 22 de abril de 2025

### 📚 Tema: Inicio del Bloque 3 — Modelos estadísticos y modelos no lineales

---

### 🎯 **Objetivos de la clase:**

1. Introducir los modelos lineales como punto de partida en aprendizaje supervisado.
2. Comprender sus supuestos, ventajas y limitaciones.
3. Explorar la diferencia entre modelos lineales y no lineales.
4. Analizar cuándo un modelo lineal es adecuado y cuándo no lo es.

---

### 🧠 **Contenidos tratados (teoría + énfasis del profesor):**

---

#### ✅ 1. Modelos estadísticos y su lógica

* Se introducen como modelos con una base teórica **probabilística o estadística**, con **supuestos fuertes sobre los datos**.
* Ejemplo: **regresión lineal** asume que la relación entre las variables es lineal, que los residuos son normales, homocedásticos, e independientes.

📌 **Comentario del profesor:**

> “La regresión lineal funciona muy bien… cuando se cumplen sus supuestos. Si no, es un desastre.”

---

#### ✅ 2. Regresión lineal simple y múltiple

* **Regresión lineal simple:** una variable independiente.

  * Modelo: y = β₀ + β₁·x + ε

* **Regresión lineal múltiple:** varias variables independientes.

  * Modelo: y = β₀ + β₁·x₁ + β₂·x₂ + ... + βₙ·xₙ + ε

* Los coeficientes (β) se ajustan para minimizar el error cuadrático (mínimos cuadrados ordinarios).

* **Interpretación de los coeficientes:** cuánto cambia y ante una unidad de cambio en x.

📌 **Aclaración importante:**

> “Una de las grandes virtudes de la regresión lineal es que es **fácil de interpretar**.”

---

#### ✅ 3. Limitaciones de los modelos lineales

* **No capturan relaciones no lineales** entre las variables.
* Son **muy sensibles a outliers**.
* Requieren que las variables no estén fuertemente correlacionadas entre sí (**colinealidad**).
* Generalmente **no funcionan bien con variables categóricas** sin una codificación adecuada.

📌 **Comentario del profesor:**

> “Un modelo lineal con muchas variables categóricas mal codificadas es como una receta con los ingredientes equivocados.”

---

#### ✅ 4. Introducción a modelos no lineales

* Se define un modelo no lineal como aquel en el que la relación entre los parámetros y la salida **no es una combinación lineal**.
* **Ventaja:** pueden capturar relaciones complejas y patrones no evidentes.
* **Desventaja:** suelen ser menos interpretables y más propensos al sobreajuste.

📌 **Transición clave:**

> “Aquí es donde aparecen los **árboles de decisión**, que veremos en la próxima clase.”

---

#### ✅ 5. Aplicación práctica de modelos lineales

* Casos donde **sí es recomendable** usar un modelo lineal:

  * Relación simple y clara entre variables.
  * Necesidad de interpretabilidad.
  * Datos bien comportados, sin ruido excesivo.

* Casos donde **NO se recomienda**:

  * Relación no lineal entre variables.
  * Gran cantidad de variables categóricas.
  * Datos con outliers o distribución no normal.

📌 **Ejemplo práctico:**

> Predecir precios de viviendas en un barrio homogéneo → regresión lineal podría funcionar.
> Predecir preferencias de usuario en un sistema de recomendación → mejor un modelo no lineal.

---

### 📌 Ideas clave para repasar:

* Saber **formular** un modelo de regresión y estimar coeficientes.
* Entender **qué significan los coeficientes** de un modelo lineal.
* Conocer **los supuestos** de la regresión y cómo verificarlos.
* Identificar **cuándo conviene usar un modelo lineal y cuándo no.**
* Distinguir claramente entre modelos **lineales** y **no lineales**.

---

### 📝 Consejos del profesor:

* “No usen regresión lineal por costumbre. Pregúntense siempre si tiene sentido con los datos que tienen.”
* “En el examen podrían pedirles que justifiquen si un modelo lineal sería adecuado o no para un caso dado.”
* Se recomienda practicar con datasets donde la relación entre variables sea tanto lineal como no lineal para observar diferencias.

Aquí tienes el **resumen completo y detallado de la clase del 29 de abril de 2025**, continuación del Bloque 3, dedicada a los **árboles de decisión**, uno de los modelos no lineales más importantes y versátiles del aprendizaje supervisado.

# 🗓️ Clase del 29 de abril de 2025

### 📚 Tema: Bloque 3 (II) — Árboles de decisión: estructura, funcionamiento y problemas

---

### 🎯 **Objetivos de la clase:**

1. Comprender la estructura y lógica de los árboles de decisión.
2. Explicar cómo se construyen y cómo toman decisiones.
3. Identificar ventajas y desventajas del modelo.
4. Introducir el concepto de sobreajuste y su relación con los árboles.
5. Explicar los criterios de división y técnicas de poda.

---

### 🧠 **Contenidos tratados (teoría + explicaciones del profesor):**

---

#### ✅ 1. ¿Qué es un árbol de decisión?

* Modelo predictivo que **representa decisiones como una estructura jerárquica de preguntas**.
* Se construye dividiendo el conjunto de datos en subconjuntos más homogéneos.
* Cada **nodo interno** representa una condición sobre una variable.
* Cada **hoja** representa una predicción final.

📌 **Ejemplo comentado en clase:**

> Si temperatura > 30 → sí → humedad > 70 → sí → “no jugar tenis”.

---

#### ✅ 2. Construcción del árbol (crecimiento)

* Se parte de la raíz con todos los datos.
* En cada nodo se busca **la variable y el umbral que mejor separen los datos**.
* El proceso continúa **recursivamente** hasta cumplir un criterio de parada.

---

#### ✅ 3. Criterios de división

* En clasificación:

  * **Índice Gini**
  * **Entropía (Information Gain)**
* En regresión:

  * **Error cuadrático medio**
  * **Reducción de varianza**

📌 **Comentario del profesor:**

> “El índice Gini y la entropía suelen dar resultados similares, pero es útil saber cómo se calculan ambos.”

---

#### ✅ 4. Poda del árbol

* **Árboles muy grandes tienden al sobreajuste**: aprenden ruido del entrenamiento.
* La **poda** reduce el tamaño del árbol para mejorar generalización.

  * **Pre-poda:** limitar profundidad, número mínimo de muestras por nodo, etc.
  * **Post-poda:** construir árbol completo y luego eliminar nodos con bajo aporte.

📌 **Comentario destacado:**

> “Si no podan el árbol, se puede ajustar perfecto al entrenamiento… y fallar completamente con datos nuevos.”

---

#### ✅ 5. Ventajas de los árboles de decisión

* Intuitivos y fáciles de interpretar.
* Manejan variables numéricas y categóricas sin requerir normalización.
* No necesitan escalado.
* Capacidad de capturar relaciones no lineales y jerárquicas.

---

#### ✅ 6. Desventajas y riesgos

* **Alta varianza:** pequeñas variaciones en los datos pueden cambiar mucho el árbol.
* **Sobreajuste (overfitting):** especialmente si no se controla su crecimiento.
* **No son los mejores en precisión bruta**, aunque sí en interpretabilidad.

---

#### ✅ 7. Aplicaciones típicas

* Clasificación médica (sí/no enfermo), decisiones de riesgo, segmentación de clientes, etc.

📌 **Comentario del profesor:**

> “El árbol por sí solo no suele ser el mejor, pero es muy útil y forma la base de muchos modelos ensemble.”

---

### 📌 Ideas clave para repasar:

* Saber cómo se construye un árbol: criterios de división, nodos, hojas.
* Entender bien los conceptos de entropía e índice Gini.
* Conocer técnicas de **poda** para evitar sobreajuste.
* Identificar cuándo usar árboles de decisión y qué tipo de datos requieren.
* Reconocer que los árboles **pueden sobreajustarse fácilmente si no se limitan**.

---

### 📝 Consejos del profesor:

* “Sepan interpretar un árbol: si les dan uno en el examen, deben poder explicar cómo clasifica una observación.”
* “Practiquen con ejemplos para entender cómo varían las predicciones si cambian los datos de entrada.”
* “Recuerden: árboles no necesitan normalizar, pero sí controlar su profundidad.”

Aquí tienes el **resumen detallado de la clase del 5 de mayo de 2025**, en la que se inicia el **Bloque 4: Métodos de Ensemble**. Esta sesión introduce uno de los pilares de los modelos avanzados de clasificación y regresión: la combinación de múltiples modelos para mejorar el rendimiento predictivo.

# 🗓️ Clase del 5 de mayo de 2025

### 📚 Tema: Bloque 4 — Métodos de Ensemble (I): Bagging, Boosting, Stacking

---

### 🎯 **Objetivos de la clase:**

1. Comprender qué es un método de ensemble y por qué se utiliza.
2. Diferenciar entre Bagging, Boosting y Stacking.
3. Identificar los beneficios de combinar modelos frente a usar uno solo.
4. Introducir el concepto de variación y sesgo en modelos.

---

### 🧠 **Contenidos tratados (teoría + énfasis del profesor):**

---

#### ✅ 1. ¿Qué es un método de ensemble?

* Técnica que **combina múltiples modelos** para mejorar la precisión y estabilidad de las predicciones.
* Principio general: **“la unión hace la fuerza”**.
* Dos grandes objetivos:

  * **Reducir la varianza** (mejor estabilidad).
  * **Reducir el sesgo** (mejor ajuste a los datos).

📌 **Comentario del profesor:**

> “Un modelo débil se puede volver potente si se combina bien con otros.”

---

#### ✅ 2. Bagging (Bootstrap Aggregating)

* Técnica de reducción de varianza.
* Se entrenan múltiples modelos sobre distintos subconjuntos aleatorios (con reemplazo) del conjunto de entrenamiento (**bootstrap**).
* Cada modelo vota (clasificación) o promedia (regresión).
* Ejemplo clásico: **Random Forest** (conjunto de árboles entrenados con bagging).

📌 **Ventajas:**

* Reduce el sobreajuste al suavizar las predicciones.
* Fácil de paralelizar.
* Robusto ante datos ruidosos.

📌 **Comentario del profesor:**

> “El Bagging es ideal cuando tienes un modelo con **alta varianza**, como un árbol sin poda.”

---

#### ✅ 3. Boosting

* Técnica de reducción de sesgo.
* Los modelos se entrenan **secuencialmente**: cada uno se enfoca en los errores del anterior.
* Se asignan **pesos mayores a los errores** cometidos para que el siguiente modelo intente corregirlos.
* Modelos representativos:

  * **AdaBoost**
  * **Gradient Boosting Machines (GBM)**

📌 **Ventajas:**

* Puede lograr **mayor precisión** que Bagging.
* Enfoca el aprendizaje en los casos difíciles.

📌 **Riesgos:**

* Mayor propensión al **sobreajuste** si no se controlan los hiperparámetros.
* Mayor coste computacional.

📌 **Comentario del profesor:**

> “El Boosting es muy potente, pero si te pasas, se ajusta tanto que aprende el ruido.”

---

#### ✅ 4. Stacking (Stacked Generalization)

* Técnica que combina **diferentes tipos de modelos** (heterogéneos).
* Se entrena un **meta-modelo final** que decide qué predicción usar entre los modelos base.
* Cada modelo base predice, y esas predicciones se convierten en variables de entrada para el meta-modelo.

📌 **Ventajas:**

* Aprovecha lo mejor de varios algoritmos.
* Suele mejorar el rendimiento si los modelos base son diversos y bien configurados.

📌 **Comentario del profesor:**

> “El stacking es como tener expertos en distintas áreas y un jefe que decide a cuál hacerle caso.”

---

#### ✅ 5. Comparación general entre métodos

| Método   | Entrenamiento | Objetivo principal    | Riesgo de overfitting |
| -------- | ------------- | --------------------- | --------------------- |
| Bagging  | Paralelo      | Reducir varianza      | Bajo                  |
| Boosting | Secuencial    | Reducir sesgo         | Medio/Alto            |
| Stacking | Combinado     | Combinar modelos base | Medio                 |

📌 **Comentario del profesor:**

> “En el examen, podrían preguntarles cuál usar según el tipo de problema o comportamiento del modelo.”

---

### 📌 Ideas clave para repasar:

* Entender las diferencias entre Bagging, Boosting y Stacking.
* Saber cuál técnica aplicar según si hay **alto sesgo o alta varianza**.
* Recordar que:

  * Bagging = modelos independientes en paralelo.
  * Boosting = secuencia de modelos dependientes.
  * Stacking = mezcla con meta-modelo.

---

### 📝 Consejos del profesor:

* “Practiquen interpretar gráficos de aprendizaje de boosting para ver si está sobreajustando.”
* “No digan en el examen que un método es mejor sin **justificar para qué caso específico**.”
* “Aprender a identificar si un modelo tiene más sesgo o más varianza puede ser lo que les haga ganar ese punto extra.”

Aquí tienes el **resumen completo y detallado de la clase del 19 de mayo de 2025**, que continúa con el **Bloque 4**, profundizando de forma técnica y aplicada en los dos métodos ensemble más utilizados en la práctica: **Bagging y Boosting**.

# 🗓️ Clase del 19 de mayo de 2025

### 📚 Tema: Bloque 4 (II) — Bagging y Boosting en detalle

---

### 🎯 **Objetivos de la clase:**

1. Analizar en profundidad cómo funcionan internamente los métodos de Bagging y Boosting.
2. Comprender sus ventajas y limitaciones prácticas.
3. Estudiar algoritmos específicos: Random Forest y AdaBoost.
4. Preparar criterios para saber cuándo usar cada método según el problema.

---

### 🧠 **Contenidos tratados (teoría + énfasis del profesor):**

---

#### ✅ 1. Bagging: Revisión técnica

* Reafirma que **Bagging es ideal para modelos de alta varianza** (como árboles de decisión).
* Cada modelo se entrena con un **bootstrap sample** (subconjunto aleatorio con reemplazo).
* Los resultados se combinan por **votación (clasificación)** o **promedio (regresión)**.

📌 **Comentario del profesor:**

> “Con Bagging no buscamos mejorar el sesgo, sino estabilizar modelos que fluctúan mucho con los datos.”

---

#### ✅ 2. Random Forest

* Ejemplo clásico de Bagging aplicado a árboles de decisión.
* Añade **aleatoriedad en la selección de atributos** al construir cada árbol.
* Esto evita que todos los árboles sean iguales y mejora la diversidad.
* Se utilizan **muchos árboles pequeños y no podados**.

📌 **Ventajas clave:**

* Robustez al ruido y a datos faltantes.
* Buena precisión sin sobreajuste.
* No requiere escalar datos ni transformar variables.

📌 **Comentario del profesor:**

> “El Random Forest es uno de los modelos más utilizados en la industria por su fiabilidad general.”

---

#### ✅ 3. Boosting: Revisión técnica

* Modelo secuencial: cada nuevo modelo intenta **corregir los errores del anterior**.
* Los errores se **ponderan más fuertemente** en el siguiente paso.
* Usa modelos débiles (por ejemplo, árboles pequeños o ‘stumps’).

📌 **Estrategia general:**

1. Entrenar primer modelo.
2. Evaluar errores.
3. Ajustar pesos.
4. Entrenar nuevo modelo.
5. Repetir.

---

#### ✅ 4. AdaBoost (Adaptive Boosting)

* Asigna pesos a las observaciones.
* Al inicio, todos los datos tienen el mismo peso.
* Después de cada iteración, **los errores se penalizan más**.
* La predicción final es un **voto ponderado** de todos los modelos.

📌 **Ventajas:**

* Fuerte rendimiento con pocos modelos.
* Enfoca el aprendizaje en los casos difíciles.

📌 **Limitaciones:**

* Sensible a outliers y ruido.
* Si no se regula, tiende a sobreajustar.

📌 **Comentario del profesor:**

> “AdaBoost es como un alumno que presta más atención a los errores del examen anterior.”

---

#### ✅ 5. Diferencias prácticas clave entre Bagging y Boosting

| Característica    | Bagging          | Boosting                     |
| ----------------- | ---------------- | ---------------------------- |
| Entrenamiento     | En paralelo      | Secuencial                   |
| Objetivo          | Reducir varianza | Reducir sesgo                |
| Modelo base       | Independiente    | Depende del anterior         |
| Sobrecarga        | Baja             | Alta (riesgo de overfitting) |
| Robustez al ruido | Alta             | Baja                         |

📌 **Comentario del profesor:**

> “Si tienen poco tiempo y datos ruidosos, usen Bagging. Si quieren afinar mucho con datos limpios, prueben Boosting.”

---

### 📌 Ideas clave para repasar:

* Comprender el mecanismo de **muestreo con reemplazo** en Bagging.
* Entender cómo **se ajustan los pesos en AdaBoost**.
* Saber cuándo usar Random Forest (robustez) vs AdaBoost (precisión).
* Recordar que Bagging mejora estabilidad y Boosting mejora ajuste.
* Identificar cuándo cada técnica podría fallar: Boosting con outliers, Bagging con modelos de alto sesgo.

---

### 📝 Consejos del profesor:

* “En el examen les pueden plantear un caso con un dataset ruidoso o muy lineal. Sepan justificar qué técnica ensemble usarían.”
* “Tienen que demostrar que entienden el impacto de la secuencia en Boosting: **no es lo mismo entrenar todo a la vez que aprender del error anterior.**”
* “Practiquen interpretar salidas de Random Forest: importancia de variables, predicción promedio, etc.”

Aquí tienes el **resumen completo y detallado de la clase del 30 de mayo de 2025**, que cierra el recorrido temático del curso y está enfocada en ofrecer una visión global del aprendizaje automático visto hasta el momento, con un **énfasis claro en el formato del examen**, cómo prepararse y qué esperar.

---

# 🗓️ Clase del 30 de mayo de 2025

### 📚 Tema: Cierre del curso — Repaso general y estructura del examen

---

### 🎯 **Objetivos de la clase:**

1. Hacer un resumen de los bloques temáticos del curso.
2. Explicar detalladamente la estructura del examen.
3. Ofrecer consejos prácticos para enfrentarlo con éxito.
4. Aclarar dudas frecuentes sobre lo que se evaluará (y lo que no).

---

### 🧠 **Contenidos tratados (resumen global + instrucciones clave del profesor):**

---

#### ✅ 1. Revisión global de bloques del curso

* **Bloque 1: Introducción y tratamiento de datos**

  * Tipos de problemas: clasificación vs regresión.
  * Tipos de variables, limpieza, escalado, codificación.
  * Importancia del preprocesamiento.

* **Bloque 2: Evaluación de modelos**

  * Métricas de clasificación y regresión.
  * Validación cruzada.
  * Elección adecuada de métrica según el problema.

* **Bloque 3: Modelos estadísticos y no lineales**

  * Regresión lineal: ventajas y limitaciones.
  * Árboles de decisión: estructura, crecimiento, poda.

* **Bloque 4: Ensemble**

  * Bagging, Boosting, Stacking: diferencias conceptuales, ventajas y riesgos.
  * Random Forest, AdaBoost: mecanismos y aplicaciones.

* **Bloque 5: Optimización de hiperparámetros**

  * Parámetros vs hiperparámetros.
  * Grid Search vs Random Search.
  * Coste computacional, criterio de parada.

📌 **Comentario del profesor:**

> “Todo esto lo tienen que tener en mente, pero con especial foco en los conceptos, no en memorizar fórmulas.”

---

#### ✅ 2. Estructura del examen

🧾 El examen constará de **4 partes**, con un total de **10 puntos**:

1. **Conocimiento (1 punto)**

   * Pregunta teórica de desarrollo breve.
   * Se valorará la **comprensión** de conceptos clave, no la extensión.
   * Ejemplo: ¿Cuándo usarías F1-score en lugar de accuracy?

2. **Test (3 puntos)**

   * Seis preguntas tipo test (respuesta única).
   * Puntuación:

     * +0.5 respuesta correcta
     * –0.25 respuesta incorrecta
     * 0 sin contestar
   * Basadas en definiciones, conceptos y diferenciación de técnicas.

3. **Ejercicio práctico (3 puntos)**

   * Ejercicio similar a los del cuaderno o actividades prácticas.
   * Puede implicar cálculos sencillos o interpretación de resultados.

4. **Análisis con razonamiento (3 puntos)**

   * Caso práctico con preguntas asociadas.
   * Hay que **justificar respuestas, comparar modelos, evaluar métricas**.

📌 **Aclaraciones importantes:**

* ❌ **No se pedirá código.**
* ✅ Se podrá usar bolígrafo, calculadora simple, y plantilla de respuestas para el test.
* 🧠 Se valorará el razonamiento, la claridad, y el uso correcto de los términos técnicos.

---

#### ✅ 3. Consejos para preparar el examen

* **Domina los conceptos clave**, especialmente:

  * ¿Qué modelo usarías y por qué?
  * ¿Qué métrica es adecuada en cada contexto?
  * ¿Cuándo un modelo tiene sobreajuste?
  * ¿Qué técnica ensemble aplicarías y por qué?

* **Revisa los ejercicios de clase**:

  * Preguntas sobre tipos de variables.
  * Interpretación de métricas.
  * Diferenciación de problemas (regresión vs clasificación).
  * Justificación de transformaciones.

* **En la parte de análisis**:

  * Lee con calma el enunciado.
  * Subraya lo relevante.
  * Justifica cada respuesta con lógica, aunque no sepas el cálculo exacto.

📌 **Comentario clave del profesor:**

> “Una respuesta incompleta pero bien razonada puede valer más que una completa sin sentido.”

---

### 📌 Ideas clave para repasar:

* Enfócate en **saber explicar conceptos**: no memorices, comprende.
* Aprende a **distinguir entre modelos y cuándo usarlos.**
* Sé capaz de **relacionar los conceptos del curso con un caso práctico**.
* No olvides que el examen valora **criterio, no código**.

---

### 📝 Últimas recomendaciones del profesor:

* “Lean bien las preguntas. A veces lo que cambia es una palabra, y eso cambia la respuesta correcta.”
* “Practiquen con los tests corregidos, pero no los memoricen sin entender.”
* “Tengan en cuenta que lo más importante es **argumentar con propiedad**.”

Aquí tienes el **resumen completo y detallado de la clase del 2 de junio de 2025**, dedicada a la **revisión de actividades anteriores, dudas frecuentes y preparación orientada al examen**. Esta clase funciona como una sesión de entrenamiento práctico, enfocada en refinar criterios de evaluación, análisis de ejercicios y estructura de respuesta.

# 🗓️ Clase del 2 de junio de 2025

### 📚 Tema: Revisión de actividades — Preparación y simulación para el examen

---

### 🎯 **Objetivos de la clase:**

1. Revisar actividades prácticas realizadas durante el curso.
2. Identificar errores comunes en las respuestas de los estudiantes.
3. Entrenar la interpretación de resultados y justificación de decisiones.
4. Simular preguntas de análisis similares a las del examen.

---

### 🧠 **Contenidos tratados (repaso + enfoque estratégico):**

---

#### ✅ 1. Revisión de actividades anteriores

* Se repasaron ejercicios donde el alumnado debía:

  * Identificar el tipo de problema (clasificación o regresión).
  * Escoger un modelo apropiado.
  * Aplicar métricas de evaluación correctamente.
  * Transformar variables antes de modelar.

📌 **Comentario del profesor:**

> “La mayoría de errores vienen de **no justificar bien la elección de métrica o modelo**, no de hacer mal los cálculos.”

---

#### ✅ 2. Casos comunes discutidos en clase

**Caso 1:**

> *Predecir la cancelación de un contrato de cliente (sí/no), con variables como edad, consumo y localización.*

* Se esperaba identificarlo como **clasificación**.
* Justificación del uso de modelos como árboles de decisión, regresión logística, etc.
* Evaluar con **F1-score** o **AUC** por posible desbalance de clases.

**Caso 2:**

> *Predecir el importe mensual que un cliente gastará en el servicio.*

* Identificado como **regresión**.
* Aplicación de **regresión lineal**, Random Forest Regressor, etc.
* Evaluación con **MAE o RMSE**.

📌 **Refuerzo del profesor:**

> “Cada elección debe ir acompañada de un **por qué**. No vale decir ‘uso Random Forest’ sin justificación.”

---

#### ✅ 3. Práctica con preguntas estilo examen

Se presentaron preguntas similares a las de la parte 4 del examen (análisis):

**Ejemplo:**

> “Se entrena un modelo SVM para clasificar clientes y se obtiene un accuracy de 95%, pero el recall es de 50%. ¿Cómo lo interpretarías?”

**Discusión esperada:**

* Alta precisión global, pero **mala capacidad para detectar positivos reales**.
* Indica un problema de **desequilibrio de clases o umbral de decisión inadecuado**.
* Posibles soluciones: cambiar métrica de evaluación, rebalancear clases, ajustar hiperparámetros.

📌 **Comentario clave:**

> “Si tienen este tipo de pregunta en el examen, **analicen, comparen, propongan cambios y justifíquenlos**.”

---

#### ✅ 4. Evaluación de transformaciones

**Errores frecuentes:**

* Aplicar label encoding a variables sin orden.
* No escalar datos antes de SVM.
* Usar accuracy como única métrica.

📌 **Refuerzo del profesor:**

> “Transformar mal los datos puede invalidar el modelo. Eso sí que se penaliza.”

---

### 📌 Ideas clave para repasar:

* Practicar interpretación de métricas con matrices de confusión y resultados ambiguos.
* Justificar **por qué se elige una métrica**, **cuándo se usa una técnica de ensemble**, y **qué transformación aplicar según el tipo de variable**.
* Leer cuidadosamente los enunciados de preguntas tipo análisis: subrayar variables, identificar salidas y estructuras de los datos.

---

### 📝 Consejos finales del profesor:

* “En el examen, si no saben calcular, al menos **expliquen bien lo que representa una métrica o decisión**.”
* “No necesitan memorizar todos los métodos, pero sí entender **para qué sirve cada uno**.”
* “Practiquen pensar como si fueran ustedes quienes diseñan el sistema de predicción.”

Aquí tienes el **resumen completo y detallado de la clase del 10 de junio de 2025**, correspondiente al inicio del **Bloque 5: Optimización de modelos de aprendizaje supervisado**. Esta sesión introduce la diferencia entre parámetros e hiperparámetros y los métodos sistemáticos para encontrar la mejor configuración de un modelo.

# 🗓️ Clase del 10 de junio de 2025

### 📚 Tema: Bloque 5 — Optimización de modelos: hiperparámetros, búsqueda y validación

---

### 🎯 **Objetivos de la clase:**

1. Distinguir entre parámetros internos del modelo e hiperparámetros definidos por el usuario.
2. Conocer técnicas de búsqueda de hiperparámetros: Grid Search y Random Search.
3. Comprender el uso de validación cruzada para evaluar configuraciones.
4. Analizar el coste computacional y el criterio de parada de estas búsquedas.

---

### 🧠 **Contenidos tratados (teoría + énfasis práctico del profesor):**

---

#### ✅ 1. Parámetros vs. Hiperparámetros

* **Parámetros**: valores aprendidos automáticamente durante el entrenamiento.
  Ejemplo: coeficientes β en regresión lineal, pesos en una red neuronal.

* **Hiperparámetros**: valores definidos **antes del entrenamiento**.
  Ejemplo: profundidad máxima de un árbol, número de estimadores en Random Forest, C y γ en SVM.

📌 **Comentario del profesor:**

> “Elegir bien los hiperparámetros es tan importante como elegir el modelo. Afectan directamente al rendimiento.”

---

#### ✅ 2. Búsqueda en rejilla (Grid Search)

* Estrategia exhaustiva: explora todas las combinaciones posibles de hiperparámetros en una rejilla predefinida.
* Requiere definir los valores a probar para cada hiperparámetro.
* Se evalúa cada combinación mediante validación cruzada.

📌 **Ventajas:**

* Fácil de implementar.
* Garantiza que se prueban todas las opciones.

📌 **Desventajas:**

* Coste computacional elevado.
* Poca eficiencia cuando hay muchas combinaciones o hiperparámetros continuos.

---

#### ✅ 3. Búsqueda aleatoria (Random Search)

* En lugar de evaluar todas las combinaciones, selecciona aleatoriamente un número fijo de combinaciones dentro del espacio definido.
* Ideal cuando se tienen **muchos hiperparámetros o rangos amplios**.

📌 **Ventajas:**

* Cobertura más diversa del espacio con menor coste.
* Probabilidad alta de encontrar una buena configuración en menos tiempo.

📌 **Comentario del profesor:**

> “En la práctica, Random Search es más eficiente que Grid Search si no tienes idea de por dónde empezar.”

---

#### ✅ 4. Validación cruzada para evaluar combinaciones

* Se utiliza para estimar el rendimiento de cada combinación de hiperparámetros.
* Divide el conjunto de entrenamiento en K partes: entrena en K–1 y valida en la restante.
* Se calcula el rendimiento promedio de cada configuración.

📌 **Refuerzo del profesor:**

> “Nunca usen el conjunto de test para elegir hiperparámetros. Para eso está la validación cruzada.”

---

#### ✅ 5. Coste computacional y criterios de parada

* Cuanto mayor sea el número de combinaciones, mayor será el coste.
* Criterios de parada:

  * Número máximo de iteraciones.
  * Tiempo máximo de búsqueda.
  * Ausencia de mejora en cierto número de pasos.

📌 **Advertencia del profesor:**

> “Buscar el mejor modelo está bien, pero no a cualquier precio. Hay que **compensar coste y ganancia**.”

---

#### ✅ 6. Casos comunes en modelos reales

* Ejemplo: **Random Forest**

  * n\_estimators (número de árboles)
  * max\_depth (profundidad máxima)
  * max\_features (número de atributos a considerar en cada división)

* Ejemplo: **SVM**

  * C (complejidad)
  * gamma (influencia del ejemplo en el kernel)

📌 **Comentario práctico:**

> “Con pocos datos, tal vez no haga falta optimizar nada. Pero con problemas reales, el ajuste fino puede marcar la diferencia.”

---

### 📌 Ideas clave para repasar:

* Tener clara la diferencia entre parámetros y **hiperparámetros**.
* Saber cómo funciona **Grid Search** y **Random Search**, con ventajas y limitaciones.
* Comprender la importancia de la **validación cruzada** para no sobreajustar.
* Conocer ejemplos reales de hiperparámetros relevantes para modelos comunes.
* Entender el **balance entre precisión del modelo y coste computacional**.

---

### 📝 Consejos del profesor:

* “En el examen les pueden pedir que propongan un proceso de optimización para un modelo.”
* “Tienen que justificar qué buscarían, cómo y por qué. No basta con decir ‘haría Grid Search’.”
* “Practiquen con configuraciones de Random Forest y vean cómo cambia el rendimiento según el número de árboles.”

Aquí tienes el **resumen completo y detallado de la clase del 16 de junio de 2025**, centrada en **casos prácticos aplicados**, con especial énfasis en cómo se estructuran las preguntas de examen en su parte de análisis, ejercicio y test. Esta clase tiene un valor estratégico porque **anticipa tipos de ejercicios y errores comunes** que los estudiantes deben evitar.

# 🗓️ Clase del 16 de junio de 2025

### 📚 Tema: Aplicación práctica — Casos de examen, análisis, errores frecuentes y consejos

---

### 🎯 **Objetivos de la clase:**

1. Entrenar la resolución de casos similares a los del examen.
2. Mostrar cómo razonar respuestas justificadas para preguntas abiertas.
3. Repasar temas propensos a aparecer en el test.
4. Identificar errores frecuentes en la interpretación de resultados.

---

### 🧠 **Contenidos tratados (casos reales + pautas del examen):**

---

#### ✅ 1. Simulación de preguntas del examen

Se revisaron **preguntas estructuradas como las del examen** (especialmente análisis y conocimiento). Ejemplos:

---

**❓Pregunta 1 (conocimiento)**

> “¿Cómo determinarías si un problema es de clasificación o de regresión?”

**Respuesta esperada:**

* Observar el tipo de variable objetivo:

  * Numérica continua → regresión.
  * Categórica o binaria → clasificación.
* Ejemplo práctico para justificar.

📌 **Comentario del profesor:**

> “Esta puede ser la pregunta 1 del examen. Tiene que estar razonada, no solo nombrada.”

---

**❓Pregunta 2 (test)**

> “¿Qué métrica usarías si la clase positiva es mucho menos frecuente que la negativa?”

* Correcta: **F1-score** o **Recall**.
* Incorrecta: Accuracy (porque puede inducir a error si el modelo predice siempre la clase mayoritaria).

📌 **Refuerzo del profesor:**

> “No usen accuracy a ciegas. ¡Es una trampa!”

---

**❓Pregunta 3 (ejercicio)**

> Dado un conjunto de métricas de evaluación y resultados para tres modelos, ¿cuál seleccionarías?

* Se esperaba razonamiento: justificar elección según precisión, recall, complejidad, tipo de problema, etc.
* Mencionar ventajas o riesgos (overfitting, interpretabilidad, tiempo de entrenamiento).

📌 **Enfoque del profesor:**

> “Les van a dar datos, y tendrán que analizarlos como si fueran ustedes los que deciden qué modelo implantar.”

---

#### ✅ 2. Evaluación de relaciones entre variables

El profesor hizo especial énfasis en técnicas estadísticas según el tipo de variables:

| Tipo de variables       | Técnica recomendada |
| ----------------------- | ------------------- |
| Continua ↔ Continua     | Correlación         |
| Categórica ↔ Continua   | ANOVA               |
| Categórica ↔ Categórica | Chi-cuadrado        |

📌 **Comentario importante:**

> “Esto cae casi seguro en el examen. ¡Y lo hacen mal todo el tiempo!”

---

#### ✅ 3. Pregunta tipo análisis con caso real

> *Se entrenó un modelo SVM con C=10 y se obtuvo una AUC de 0.71. ¿Qué podrías hacer para mejorarlo?*

* Ajustar hiperparámetros (modificar C, probar otro kernel).
* Escalar bien los datos (si no se hizo).
* Probar otras técnicas de selección de características.
* Considerar otro modelo si los resultados siguen bajos.

📌 **Lo esperado:**
Justificar, razonar y proponer mejoras concretas.

---

#### ✅ 4. Análisis de errores comunes

* Usar Label Encoding en variables nominales sin orden → error.
* No escalar datos para SVM o KNN → mala predicción.
* Elegir modelo complejo cuando uno simple basta → sobreajuste.
* Confundir precisión con recall → interpretación errónea.

📌 **Consejo del profesor:**

> “No se trata de saberlo todo. Se trata de **entender qué hacer con lo que saben**.”

---

#### ✅ 5. Comparación entre métodos de ensemble

Repaso práctico:

* **Bagging**: modelos en paralelo, ideal para reducir varianza.
* **Boosting**: modelos en secuencia, enfocados en reducir sesgo.
* **Stacking**: combinación heterogénea con meta-modelo.

Se preguntó a los estudiantes:

> “¿Qué método usarías si tu modelo tiene alta varianza? ¿Y si tiene alto sesgo?”

📌 **Respuestas esperadas:**

* Alta varianza → Bagging (Random Forest).
* Alto sesgo → Boosting (AdaBoost, Gradient Boosting).

---

### 📌 Ideas clave para repasar:

* Saber **cuándo aplicar una métrica y por qué**.
* Justificar **la elección de modelos según el tipo de error o rendimiento esperado**.
* Practicar lectura e interpretación de salidas del modelo (matrices, gráficos, métricas).
* Entender relaciones entre variables y qué pruebas estadísticas aplicar.

---

### 📝 Consejos del profesor:

* “En la parte de análisis, no hay respuestas únicas. Hay argumentos mejores.”
* “Pueden equivocarse en una fórmula, pero si explican el razonamiento, puntúa.”
* “Si no recuerdan un nombre exacto, **describan la función o comportamiento del modelo.**”

Aquí tienes el **resumen completo y detallado de la clase del 23 de junio de 2025**, correspondiente al cierre del **Bloque 5: Optimización de modelos supervisados**. Esta clase se enfocó en técnicas avanzadas de búsqueda de hiperparámetros, consideraciones estratégicas de ajuste fino y recomendaciones finales para abordar problemas reales con sentido práctico.

# 🗓️ Clase del 23 de junio de 2025

### 📚 Tema: Bloque 5 (II) — Técnicas avanzadas de optimización, ajuste fino y consejos finales

---

### 🎯 **Objetivos de la clase:**

1. Profundizar en estrategias avanzadas de optimización de modelos.
2. Aprender a ajustar configuraciones de hiperparámetros con criterio y sin sobrecoste.
3. Entender la lógica detrás de Random Search y su ventaja en espacios grandes.
4. Anticipar preguntas aplicadas de examen sobre rendimiento y tuning.

---

### 🧠 **Contenidos tratados (teoría avanzada + aplicación práctica):**

---

#### ✅ 1. Recordatorio: Grid Search vs Random Search

* **Grid Search**:

  * Explora todo el espacio de forma exhaustiva.
  * Alto coste si hay muchos hiperparámetros o valores.
  * No siempre mejora los resultados si el espacio está mal definido.

* **Random Search**:

  * Selecciona combinaciones aleatorias.
  * Más eficiente en espacios grandes y de alta dimensión.
  * Alta probabilidad de encontrar buenas soluciones con menos pruebas.

📌 **Comentario del profesor:**

> “En muchos estudios, Random Search supera a Grid Search en eficiencia práctica. No por probar más, se encuentra mejor.”

---

#### ✅ 2. Estrategia de optimización por etapas

* **Fase 1:** búsqueda amplia (random) para ubicar regiones prometedoras.
* **Fase 2:** refinamiento en torno a los mejores resultados encontrados (rejilla localizada).
* **Fase 3 (opcional):** tuning de hiperparámetros secundarios o ajuste fino.

📌 **Ejemplo discutido:**

> Buscar inicialmente en C ∈ \[0.01, 1000] y gamma ∈ \[1e–5, 1], luego refinar en torno a C = 10 y gamma = 0.1.

📌 **Consejo del profesor:**

> “No hagan Grid Search sobre todo el espacio. Usen Random Search primero, luego profundicen.”

---

#### ✅ 3. Métricas de evaluación para seleccionar la mejor configuración

* Métricas distintas llevan a diferentes “mejores” modelos.

  * Ej.: optimizar para F1-score ≠ optimizar para accuracy.
* El **criterio de evaluación debe coincidir con el objetivo del sistema**.

📌 **Comentario clave:**

> “Si el problema es detectar fraude, optimiza recall, no accuracy. Cada métrica cuenta una historia distinta.”

---

#### ✅ 4. Criterios de parada

* Para evitar exceso de coste:

  * Máximo de iteraciones.
  * Tiempo límite.
  * Número de pasos sin mejora.

* Algunos frameworks permiten **Early Stopping**, especialmente útil en redes neuronales y boosting.

---

#### ✅ 5. Elección de modelo en base al contexto

El profesor repasó factores que deben influir en la elección final del modelo:

* Interpretabilidad.
* Velocidad de entrenamiento y predicción.
* Robustez al ruido.
* Capacidad de generalización.

📌 **Ejemplo práctico:**

> En un entorno médico, mejor un modelo ligeramente menos preciso pero más interpretable (como regresión logística o árbol).

---

#### ✅ 6. Consideraciones éticas y prácticas

* Evitar sesgos en la selección de datos.
* No sobreoptimizar el modelo para un conjunto de validación concreto.
* Pensar en el coste computacional vs beneficio obtenido.

📌 **Comentario final del profesor:**

> “Optimizar no es hacer magia. Es encontrar un buen equilibrio entre rendimiento, coste y comprensión del modelo.”

---

### 📌 Ideas clave para repasar:

* Saber explicar **por qué Random Search es útil en problemas de muchos hiperparámetros**.
* Comprender cómo diseñar una **búsqueda en dos fases**: amplia + refinada.
* Tener claro que el **criterio de evaluación define qué es ‘mejor’**.
* Conocer **criterios de parada razonables** para no consumir recursos innecesarios.
* Relacionar el ajuste de modelos con el **contexto del problema y los objetivos del sistema**.

---

### 📝 Consejos finales del profesor:

* “Si en el examen les piden proponer una estrategia de optimización, no se limiten a decir ‘Grid Search’. Expliquen su razonamiento.”
* “Elijan las métricas en función del problema. No hay una ‘mejor’. Hay una más coherente con lo que se busca.”
* “No hace falta encontrar el modelo perfecto. Hace falta encontrar uno bueno y robusto, que sepan explicar y aplicar.”
