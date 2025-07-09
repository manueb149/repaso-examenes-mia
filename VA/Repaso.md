Perfecto. A continuación te presento una **guía final de estudio** para el examen de *Visión Artificial*, basada en todo el contenido visto durante las clases, presentaciones y ejercicios tipo.

---

## 🧾 GUÍA FINAL DE ESTUDIO – Visión Artificial 2025

### 🧠 1. Conceptos y Fórmulas Clave

#### 📏 Digitalización de señales

* **Teorema de Nyquist-Shannon**:
  $f_{\text{muestreo}} \geq 2 \cdot f_{\text{máxima}}$
* **Nivel de intensidad sonora (dB)**:
  $L(dB) = 10 \cdot \log_{10} \left(\frac{I}{I_0}\right)$
* **Resolución de cuantificación**:
  $N = 2^b$, donde `b` = bits.
  Paso = $\frac{rango}{N}$

#### 🧮 Entropía e intensidad

* **Entropía**:
  $H = -\sum p_i \log_2(p_i)$
  (Se usa en imágenes para medir dispersión de niveles de gris)
* **Relación clave**:

  * Imagen **uniforme** → **baja entropía**
  * Imagen **aleatoria o compleja** → **alta entropía**

#### 🔁 Filtros

* **Convolución**: el kernel se invierte.
* **Correlación**: el kernel se aplica tal cual.
* Filtros comunes:

  * `h1` = bordes de claro a oscuro
  * `h2` = bordes de oscuro a claro (opuesto a h1)

#### 🧱 Morfología matemática

* **Erosión**: reduce regiones claras → mínimo local.
* **Dilatación**: expande regiones claras → máximo local.
* **Apertura** = erosión + dilatación → elimina detalles pequeños.
* **Cierre** = dilatación + erosión → rellena huecos.

#### 📊 Texturas y LBP

* **LBP paso a paso**:

  1. Se toman 8 vecinos (sentido antihorario desde derecha).
  2. Se resta el centro → vector binario.
  3. Se convierte en número decimal → valor LBP.
  4. Se analiza si el patrón es **uniforme** (máx. 2 transiciones 0↔1).
* **GLCM**:

  * Se construye contando pares de niveles (i,j).
  * Características:

    * **Contraste**
    * **Energía**
    * **Entropía**
    * **Correlación**

---

### 🔬 2. Tipos de ejercicios típicos del examen

* Calcular bits necesarios para transmitir una imagen con compresión.
* Aplicar LBP paso a paso y decidir si es uniforme.
* Analizar GLCM y calcular contraste/entropía.
* Interpretar histogramas antes y después de transformaciones de intensidad.
* Aplicar operaciones morfológicas (apertura, dilatación, etc.).
* Comparar transformaciones: potencia (gamma), logarítmica, umbralización.
* Determinar frecuencia mínima de muestreo según Nyquist.
* Distinguir entre convolución y correlación en filtros.

---

### 📚 3. Estrategia de repaso

1. **Memoriza las fórmulas esenciales** (Nyquist, entropía, paso de cuantificación).
2. **Domina los pasos de LBP**: este ejercicio casi siempre entra.
3. **Practica con las matrices GLCM**: entiende qué significa cada celda.
4. **Rehaz todos los ejemplos de los PDFs de preparación**.
5. **Ensaya explicaciones escritas**: el examen no incluye código, sino desarrollo conceptual y numérico.
6. **Revisa los efectos visuales de cada transformación de imagen**.

---