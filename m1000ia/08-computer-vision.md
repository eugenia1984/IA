# CLASE 8 - COMPUTER VISION

## TEMAS:

01. ¿Qué es computer vision?

02. Tareas dentro de computer vision

03 . Redes neuronales convolucionales

04 . Métricas de evaluación y datasets

---

"La visión por computadora es el proceso mediante el
cual dotamos a las máquinas de la capacidad de
interpretar y entender el entorno visual, convirtiendo
datos visuales en decisiones informadas y acciones
concretas, lo que está revolucionando la forma en que
interactuamos con la tecnología y abriendo nuevas
fronteras en aplicaciones prácticas en diversos campos" 

---

## 01 -  ¿Qué es computer vision?

### Definición

Disciplina científica que incluye métodos para adquirir, procesar, analizar y
comprender las imágenes del mundo real o generadas sintéticamente con el
fin de producir información numérica o simbólica para que puedan ser
tratados por una computadora

### Objetivo

El objetivo último de la visión artificial es conseguir el desarrollo de
estrategias automáticas para el reconocimiento de patrones complejos en
imágenes de múltiples dominios”

### ¿Qué tipos de problemas puede solucionar?

Extracción de características: Proceso de identificar y seleccionar atributos
relevantes en imágenes para su análisis y clasificación.

Detección de objetos: Técnica para identificar y localizar instancias de
objetos específicos dentro de imágenes o vídeos.

Clasificación de objetos: Método para asignar una etiqueta de categoría a
objetos detectados en imágenes o vídeos.

Segmentación de objetos: Proceso de dividir una imagen en regiones o
segmentos, cada uno representando un objeto o parte de él.

Trackeo de objetos: Técnica para seguir el movimiento de objetos a lo largo
del tiempo en secuencias de imágenes o vídeos.

---

## 02 -  Tareas dentro de computer vision

![image](https://github.com/user-attachments/assets/9c2a98aa-53b6-40bb-9802-a1a2f9a05071)

### ¿Cómo podemos definir una imagen?

Para una computadora, una imagen es una representación digital compuesta
por una matriz de píxeles, donde cada píxel almacena valores numéricos que
indican su color e intensidad.

Estos valores suelen representarse en sistemas de color como RGB (rojo,
verde, azul) para imágenes a color o en escala de grises para imágenes en
blanco y negro.

La computadora procesa y analiza estas matrices numéricas para realizar
operaciones de visión por computadora, como detección de objetos,
reconocimiento de patrones y edición de imágenes.
En resumen, una imagen para la computadora es un conjunto estructurado
de datos numéricos que representan información visual.

### Imagen: Una matriz de píxeles con distinta intensidad

![image](https://github.com/user-attachments/assets/6e758a59-38b4-4596-91f8-425ac129400d)

### Imágenes en colores ¿Cómo se almacenan?

![image](https://github.com/user-attachments/assets/b059b451-8304-44fb-bad8-8a46623c35a3)

### Transformaciones sobre imágenes

**Transformaciones geométricas**

- Rotación: Girar la imagen en torno a un punto.

- Traslación: Mover la imagen en el espacio.

- Escalado: Cambiar el tamaño de la imagen.

- Reflexión: Invertir la imagen horizontal o verticalmente.

- Cizallamiento: Desplazar los píxeles de la imagen de forma angular.

**Transformaciones de intensidad:**

- Ajuste de brillo: Modificar la luminosidad de la imagen.

- Ajuste de contraste: Cambiar la diferencia entre los valores de intensidad más altos y más bajos.

- Ecualización del histograma: Mejorar el contraste distribuyendo uniformemente la intensidad de los píxeles.

**Transformaciones espaciales:**

- Filtrado espacial: Aplicar filtros para suavizar, realzar bordes o reducir
ruido.

- Morfología matemática: Operaciones como dilatación, erosión,
apertura y cierre para procesar formas en la imagen.

**Transformaciones de dominio de frecuencia:**

- Transformada de Fourier: Convertir la imagen al dominio de frecuencia
para análisis o filtrado.

- Transformada de ondícula (wavelet): Descomponer la imagen en
diferentes escalas de frecuencia para análisis o compresión.

**Transformaciones de color:**

- Conversión de espacios de color: Cambiar la representación de color de
la imagen (por ejemplo, de RGB a HSV o YCbCr).

- Ajuste de saturación: Modificar la intensidad de los colores en la
imagen.

---

## 03 - Redes neuronales convolucionales

Las redes neuronales convolucionales (CNN, por sus siglas en inglés) son una
clase de redes neuronales profundas (deep learning) diseñadas
específicamente para procesar datos con una estructura en forma de rejilla
(matriz), como las imágenes.

Estas redes utilizan múltiples capas denominadas convolucionales que
aplican filtros o núcleos (kernels) para extraer características visuales
relevantes, como bordes, texturas y formas.

Las CNN también incluyen capas de agrupamiento (pooling) para reducir la
dimensionalidad de los datos y capas completamente conectadas para, por
ejemplo, una tarea de clasificación.

![image](https://github.com/user-attachments/assets/425a8768-72e1-4a46-9c3f-61863341b44b)

### CNN: ¿En dónde radica su importancia?

Las CNN son fundamentales en el área de visión por computadora debido a
su capacidad para aprender automáticamente jerarquías de características
visuales a partir de grandes cantidades de datos de imágenes.

Esto las hace excepcionalmente buenas en tareas como la clasificación de
imágenes, la detección de objetos y la segmentación semántica.
Su eficacia en el procesamiento de imágenes y la extracción de
características relevantes (feature extraction) ha llevado a avances
significativos en aplicaciones como el reconocimiento facial, la conducción
autónoma y la interpretación de imágenes médicas.

### Filtros / Núcleos / Kernels ¿Qué son? ¿Qué hacen?

En el contexto de las redes neuronales convolucionales, los kernels, también
conocidos como filtros, son matrices pequeñas de valores (pesos/weights)
que se utilizan para aplicar la operación de convolución a los datos de
entrada (imágenes).

Cada kernel se desliza sobre la imagen de entrada, realizando un producto
punto entre los valores del kernel y los valores de píxeles correspondientes
en la imagen.

Esto resulta en un mapa de características que resalta ciertas características
visuales, como bordes o patrones de textura, dependiendo de los valores del
kernel.

Durante el entrenamiento de la red, los valores de los kernels se ajustan
para extraer las características más relevantes para la tarea específica.
Veamos un ejemplo gráfico a continuación

### Funcionamiento del Kernel

![image](https://github.com/user-attachments/assets/2cfef4c0-14ab-476d-a419-72b46a2d6034)

### Imagen a color - Kernel

![image](https://github.com/user-attachments/assets/ed87afa6-997a-4b7a-951f-616a5d803a68)

### Capa de pooling - ¿Para qué sirve?

El pooling, también conocido como agrupamiento, sirve para reducir la
dimensionalidad espacial de los mapas de características en una red
neuronal convolucional, lo que disminuye la cantidad de parámetros y
cálculos necesarios para el entrenamiento.

Esto ayuda a prevenir el sobreajuste y mejora la eficiencia computacional. El
pooling funciona aplicando una operación de reducción, como el máximo
(max pooling) o la media (average pooling), a regiones no superpuestas de
los mapas de características.

Por ejemplo, en el max pooling con un tamaño de ventana de 3x3, se
selecciona el valor máximo de cada región de 3x3 píxeles y se forma un
nuevo mapa de características reducido.

![image](https://github.com/user-attachments/assets/3a961e0c-935e-42d2-a43b-5067ccc4a1a2)

### Más Capas: Upsampling (Deconvolución)

La capa de deconvolución, también conocida como convolución transpuesta
o upsampling, se utiliza en redes neuronales convolucionales para aumentar
la resolución espacial de los mapas de características.

Esto es especialmente importante en tareas de segmentación de imágenes,
donde se requiere una salida detallada a nivel de píxel.

La deconvolución funciona de manera inversa a la convolución: en lugar de
combinar múltiples entradas en una salida, distribuye una entrada en
múltiples salidas, expandiendo así las dimensiones de los mapas de
características.

Esto se logra mediante la aplicación de un kernel de deconvolución que
interpola entre los píxeles de entrada, rellenando los espacios con valores
calculados para reconstruir la resolución original de la imagen.
Veamos un ejemplo gráfico a continuación

### Deconvolución

![image](https://github.com/user-attachments/assets/deae5827-c3f3-450b-8932-89a472c9eceb)

### Variantes de deconvolución

![image](https://github.com/user-attachments/assets/bfbae4d0-5eab-4bc9-874a-131c1672fff3)

### Más Capas: Skip Connection

Las capas de concatenación, o conexiones directas, son una característica
importante en arquitecturas de segmentación como U-Net.

Estas capas conectan directamente los mapas de características de capas
anteriores con capas posteriores de igual resolución espacial.

El objetivo es preservar la información espacial y de contexto que podría
perderse durante las operaciones de pooling y convolución debido a la
reducción de dimensionalidad.

Al concatenar estos mapas de características, la red puede utilizar tanto la
información de alto nivel (características abstractas) como la de bajo nivel
(detalles finos) para mejorar la precisión de la segmentación.

---

## 04 - Métricas de evaluación y datasets

---
