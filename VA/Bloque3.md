Seguimos ahora con el **Bloque 3**, centrado en la caracterización de texturas. Este bloque es especialmente importante porque, como se indicó en clase, contiene contenido muy probable en el examen. Además, se combina teoría clásica con elementos prácticos como el LBP y la matriz de coocurrencia.

---

### 🔷 **BLOQUE 3 – Caracterización de Texturas**

**Objetivo del bloque:** Aprender a describir texturas visuales a partir de relaciones espaciales y variaciones de intensidad, usando métodos estadísticos, estructurales y espectrales.

---

#### 📐 **1. Definición general de textura**

* Una **textura** en imágenes es una propiedad visual que representa la variación de intensidad de los píxeles en el espacio.
* Se puede describir de forma:

  * **Estadística**: distribución de valores.
  * **Estructural**: patrones repetitivos.
  * **Espectral**: frecuencia espacial (ej. análisis de Fourier).

---

#### 📊 **2. Matriz de Co-ocurrencia de Haralick (GLCM)**

* Se basa en contar cuántas veces un píxel de nivel `i` aparece junto a uno de nivel `j` en una dirección y distancia específicas.
* Normalmente se calcula en direcciones: 0°, 45°, 90°, y 135°.
* Características extraídas de la GLCM:

  * **Contraste**: mide la diferencia entre niveles de gris.
  * **Energía**: uniformidad de la imagen (más energía = más homogénea).
  * **Entropía**: desorden o aleatoriedad de la textura.
  * **Correlación**: relación lineal entre los pares de píxeles.
* Ejemplo típico de examen:

  * Se da una matriz GLCM y se pide calcular el contraste y la entropía.
  * Interpretar la textura: si es suave, rugosa, aleatoria, etc.

---

#### 🧮 **3. LBP – Patrones Binarios Locales**

* Método muy usado por su simplicidad y eficacia para describir texturas locales.
* Algoritmo básico:

  1. Se toma un píxel central y sus 8 vecinos (en una ventana 3x3).
  2. Se resta el valor del píxel central a cada vecino.
  3. Si el resultado es ≥ 0, se asigna un 1; si es < 0, se asigna un 0.
  4. Se forma un número binario con esos 8 bits (en sentido horario o antihorario).
  5. Se convierte el binario a decimal y ese valor representa el LBP del píxel.
* **Extensión LBP uniforme:**

  * Si el patrón tiene como máximo dos transiciones de 0→1 o 1→0, se considera **uniforme**.
  * Estos patrones son más frecuentes y fáciles de clasificar.
* Conclusión práctica:

  * Patrones **uniformes** → baja entropía → textura homogénea.
  * Patrones **no uniformes** → alta entropía → textura más compleja.

---

#### 🧮 **4. Transformadas unitarias de Chebyshev (Chebyshaw)**

* Método más avanzado, menos preguntado, pero relevante en contextos de firmas espectrales.
* Se utilizan polinomios ortogonales para caracterizar texturas como una especie de “huella digital”.
* Importante en análisis hiperespectral y reconocimiento basado en patrones únicos.

---

#### 🧩 **5. Comparación de métodos**

* Se mostró la diferencia entre métodos clásicos (como GLCM y LBP) y modelos de deep learning.
* Las redes neuronales convolucionales permiten describir texturas de forma automática y eficiente, pero requieren entrenamiento y mayor capacidad computacional.

---
