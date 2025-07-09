### 🔷 **BLOQUE 2 – Filtros, Morfología y Operadores Espaciales**

**Objetivo del bloque:** Comprender cómo aplicar filtros espaciales, operadores de convolución/correlación y transformaciones morfológicas para el procesamiento de imágenes y detección de características.

---

#### 🧰 **1. Filtros espaciales: convolución vs correlación**

* Se explicó la diferencia entre **convolución** (el kernel se invierte) y **correlación** (el kernel no se invierte).
* La operación más común en imágenes digitales es la correlación por su simplicidad.
* Aplicaciones típicas:

  * **Detección de bordes**: se usan filtros como Sobel, Prewitt, etc.
  * **Suavizado o desenfoque**: kernels promedio o gaussianos.
* Ejemplo práctico:

  * Se aplicaron filtros `h1` y `h2` para detectar bordes horizontales (de claro a oscuro y viceversa).
  * Resultado observado en imágenes filtradas.

---

#### 🌿 **2. Morfología matemática**

* Aplicada principalmente a **imágenes binarias**, aunque extensible a escala de grises.
* Operaciones básicas:

  * **Erosión**: elimina píxeles en los bordes de los objetos. Reduce regiones claras.
  * **Dilatación**: añade píxeles a los bordes de los objetos. Engrosa regiones claras.
  * **Apertura**: erosión seguida de dilatación. Elimina detalles pequeños.
  * **Cierre**: dilatación seguida de erosión. Rellena huecos.
* Ejercicios típicos:

  * Eliminar objetos pequeños manteniendo los grandes (ejemplo: monedas grandes vs pequeñas).
  * Aplicar apertura con disco de radio 25 y luego dilatación para destacar objetos deseados.
  * Operaciones lógicas tipo `AND` tras aplicar morfología para segmentar regiones específicas.

---

#### 🧪 **3. Transformaciones de intensidad**

* Transformaciones puntuales sobre el valor de los píxeles:

  * **Umbralización**: binariza la imagen según un valor de corte.
  * **Ley de potencia (gamma)**: realza zonas claras u oscuras.
  * **Transformación logarítmica**: mejora detalles en zonas oscuras.
  * **`double(I)`**: escala valores a rango \[0,1] y permite aplicar operaciones continuas.
* Se analizaron los efectos en el histograma y en la entropía.

---

#### 📌 **4. Operadores prácticos en ejercicios**

* Uso de elementos estructurantes:

  * **Cuadrado 3x3**
  * **Cruz 3x3**
  * **Disco de radio r**
* Ejercicios abordados:

  * Aplicar apertura y cierre a una imagen binaria.
  * Interpretar resultados morfológicos.
  * Comparar efectos sobre imágenes de distintos tamaños y formas.

---