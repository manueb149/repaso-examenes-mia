### 🔷 **BLOQUE 4 – Aplicaciones de Visión Artificial y Toma de Decisiones**

**Objetivo del bloque:** Entender cómo se aplican los algoritmos de visión artificial en entornos reales, analizando factores técnicos, éticos y de decisión relacionados con el modelo elegido.

---

#### 👁️‍🗨️ **1. Biometría**

* Aplicación clave: identificación de individuos mediante rasgos físicos únicos.
* **Tipos de datos biométricos:**

  * **Faciales** (rostro): segmentación, extracción de características (eigenfaces, PCA), y reconocimiento.
  * **Iris**: extremadamente distintivo, se considera una firma única por su complejidad (alta entropía).
  * **Huella dactilar**: método tradicional, muy usado por su simplicidad y precisión.
* Arquitectura típica de un sistema biométrico:

  1. Captura de la señal (sensor).
  2. Extracción de características.
  3. Comparación con una base de datos.
  4. Verificación (¿es quien dice ser?) o identificación (¿quién es?).

---

#### 🤖 **2. Reconocimiento facial**

* Se analizó el pipeline de un sistema real:

  * Dataset (ej: VGG-Face, Casia WebFace).
  * **Data Augmentation**: rotaciones, reflejos, variaciones de iluminación y geometría.
  * Uso de redes neuronales convolucionales (CNNs) para entrenamiento.
  * Fine-tuning y **transfer learning** para adaptar modelos preentrenados.
* Se explicó el concepto de “eigenfaces” y el uso de PCA para representar rostros.

---

#### 🚗 **3. Conducción autónoma**

* Ejemplo clave de visión artificial aplicada.
* Los coches autónomos capturan señales del entorno mediante múltiples sensores:

  * Cámaras, radares, LiDAR, GPS, sensores de proximidad, etc.
* El coche debe procesar estas señales en tiempo real y tomar decisiones:

  * Detección de peatones, señales, obstáculos.
  * Mantenimiento en el carril, frenado, giros.
* Se discutieron los riesgos:

  * Latencia, puntos ciegos, errores en la identificación.
  * Dilemas éticos en la toma de decisiones.

---

#### 📊 **4. Toma de decisiones y selección de modelo**

* Se explicó cómo elegir un modelo según:

  * **Complejidad del problema**.
  * **Requisitos de hardware**.
  * **Calidad y cantidad de datos disponibles**.
* No siempre el modelo más complejo es el más adecuado; a veces, modelos simples (como k-means) pueden funcionar bien si el problema lo permite.
* Se mostraron ejemplos de segmentación con `k-means` comparados con modelos de segmentación por deep learning (ej: Segment Anything de Meta).

---
