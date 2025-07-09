### 🔷 **BLOQUE 1 – Fundamentos de percepción y digitalización de señales**

**Objetivo del bloque:** Comprender cómo se capturan, representan, cuantifican y procesan señales visuales y auditivas, desde un enfoque de percepción humana hasta su tratamiento digital.

---

#### 🧠 **1. Percepción sensorial (visual y auditiva)**

* Se abordó la fisiología básica del ojo y del oído.
* Se explicó cómo el cerebro interpreta las señales sensoriales.
* Se introdujeron conceptos como umbral auditivo (Io = 10⁻¹² W/m²) y cómo se mide la intensidad sonora en decibelios:
  `L(dB) = 10·log10(I / Io)`
* Ejemplo típico: al duplicar la intensidad del sonido, este aumenta en 3 dB.

---

#### 📏 **2. Digitalización de señales**

* Introducción al **teorema de Nyquist-Shannon**: la frecuencia de muestreo debe ser al menos el doble de la frecuencia máxima de la señal (para evitar aliasing).
* Conceptos clave:

  * **Muestreo**: convertir una señal continua en una secuencia de muestras.
  * **Cuantificación**: asignar niveles discretos a esas muestras.
  * **Resolución del cuantificador**: 2ⁿ niveles (n = número de bits).
  * **Paso de cuantificación**: tamaño del intervalo que cubre cada nivel.
* Se realizaron ejercicios para calcular:

  * Número de bits requeridos para transmitir una imagen.
  * Frecuencia de muestreo óptima para diferentes señales.
  * Efectos de reducir la tasa de muestreo en la fidelidad de representación.

---

#### 🌐 **3. Entropía y compresión**

* Se introdujo la entropía como medida de la **incertidumbre** o **información** de una señal.
* Cuanto mayor la entropía, más impredecible o rica en información es una señal.
* Relación con compresión: señales con baja entropía pueden comprimirse mejor.
* Ejemplo práctico: comparar histogramas de imágenes modificadas con diferentes leyes de potencia o ecualización y deducir su entropía.

---

#### ⚠️ **4. Ruido y detección de anomalías**

* Tipos de ruido:

  * Ruido interno (sensorial, térmico)
  * Ruido externo (del entorno o canal de transmisión)
* Aplicación de **algoritmos no supervisados** para detectar **anomalías** (outliers, patrones inusuales).
* Introducción al uso de la entropía y la variación local como indicadores de anomalía.

---

#### 📊 **5. Señales e intensidad visual**

* Se analizaron transformaciones de intensidad (ley de potencia, logarítmica, etc.).
* Se mostraron efectos visuales de estas transformaciones en imágenes, junto con su impacto sobre el histograma.
* Ejemplo de preguntas prácticas del examen:

  * ¿Cuál de estas imágenes tiene mayor entropía?
  * Identificar la operación realizada en una imagen según su histograma.

---
