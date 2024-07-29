# CLASE 6 - INTRODUCCIÓN A REDES NEURONALES - DEEP LEARNING

## Temas:

01. Introducción Deep Learning

02. Componentes de una red neuronal

03. Entrenamiento de redes neuronales

04.  Transfer Learning

---

"El aprendizaje profundo es una revolución en el campo
de la inteligencia artificial, que permite a las máquinas
comprender y aprender de manera autónoma a partir
de grandes volúmenes de datos, transformando la
forma en que abordamos problemas complejos y
desbloqueando un sinfín de posibilidades en áreas
como la visión por computadora, el procesamiento del
lenguaje natural y la robótica."

---

## 01 - Introducción Deep Learning

### Reglas difíciles de explicitar

En la programación tradicional, los desarrolladores codifican reglas explícitas
para resolver problemas específicos. Sin embargo, existen situaciones donde
las reglas son demasiado complejas, ambiguas o difíciles de definir.

En estos casos, el enfoque tradicional se vuelve ineficiente o incluso inviable.
Aquí es donde el deep learning y las redes neuronales ofrecen una ventaja
significativa, ya que son capaces de aprender estas reglas implícitas
directamente de los datos.

Esto permite a las máquinas abordar tareas que antes eran consideradas
exclusivas del dominio humano, como el reconocimiento de patrones
complejos, la interpretación del lenguaje natural y la toma de decisiones en
entornos dinámicos.

### En búsqueda de reglas latentes

Las reglas latentes son patrones o relaciones ocultas en los datos que no son
evidentes a simple vista.

Estas reglas pueden ser esenciales para comprender la estructura
subyacente de los datos y para hacer predicciones precisas.

Las redes neuronales, especialmente las profundas, son excelentes para
descubrir estas reglas latentes durante el entrenamiento. Al procesar los
datos a través de múltiples capas, las redes neuronales pueden extraer
características de alto nivel y capturar la complejidad inherente a los datos.

Este proceso de aprendizaje automático permite a las redes neuronales
identificar relaciones no lineales y patrones intrincados que serían difíciles, si
no imposibles, de modelar con enfoques tradicionales.

---

## 02 - Componentes de una red neuronal

### Redes Neuronales

Las redes neuronales son modelos computacionales inspirados en la
estructura y el funcionamiento del cerebro humano, diseñados para simular
la forma en que los seres humanos aprenden y procesan la información.

Están compuestas por unidades básicas llamadas neuronas artificiales o
nodos, que están interconectadas en capas para formar una red. Cada
neurona recibe señales de entrada, las combina de manera ponderada y
aplica una función de activación para generar una señal de salida.

La información fluye a través de la red desde la capa de entrada hasta la
capa de salida, y el aprendizaje se logra ajustando los pesos de las
conexiones entre las neuronas durante un proceso de entrenamiento. Las
redes neuronales son capaces de aprender patrones complejos y no lineales,
lo que las hace adecuadas para una amplia gama de aplicaciones en
inteligencia artificial, incluyendo el reconocimiento de patrones, la
clasificación, la regresión y el procesamiento del lenguaje natural.

### La unidad de las redes Neuronales

La neurona artificial es la unidad fundamental de una red neuronal.

Inspirada en las neuronas biológicas, una neurona artificial recibe señales de
entrada, las procesa y produce una señal de salida.

La entrada a cada neurona es una combinación lineal de las salidas de las
neuronas de la capa anterior, ponderada por los pesos sinápticos. La salida
de la neurona se determina aplicando una función de activación a esta suma
ponderada.

Las funciones de activación comunes incluyen la sigmoide, la tangente
hiperbólica y la unidad lineal rectificada (ReLU), y juegan un papel crucial en
la capacidad de la red para aprender y modelar relaciones no lineales en los
datos.


### Arquitectura Red Neuronal

La arquitectura de una red neuronal se refiere a la disposición y conexión de
sus neuronas y capas. Una arquitectura típica incluye una capa de entrada,
una o más capas ocultas y una capa de salida.

La capa de entrada recibe los datos brutos, mientras que las capas ocultas
realizan la mayor parte del procesamiento, extrayendo características y
patrones útiles. La capa de salida produce la predicción o clasificación final.

La profundidad de la red, es decir, el número de capas ocultas, y el ancho de
la red, el número de neuronas en cada capa, son aspectos clave de la
arquitectura que influyen en la capacidad de la red para aprender y
generalizar.

### Multilayer Perceptron

El Multilayer Perceptron (MLP) es un tipo de red neuronal artificial que
consta de múltiples capas de neuronas, cada una conectada completamente
a la siguiente.

Esta estructura permite al MLP aprender representaciones complejas y no
lineales de los datos.

El MLP es ampliamente utilizado en tareas de clasificación y regresión y se
considera un modelo fundamental en el aprendizaje profundo.

A pesar de su simplicidad relativa en comparación con arquitecturas más
avanzadas, el MLP sigue siendo una herramienta poderosa para modelar
relaciones no lineales y descubrir patrones intrincados en los datos.

### Feed Forward Process

El proceso de feedforward es la forma en que la información fluye a través
de una red neuronal desde la capa de entrada hasta la capa de salida.

En cada capa, las señales de entrada se combinan linealmente con los pesos
sinápticos, se suman y luego se aplican funciones de activación no lineales.
Este proceso se repite capa por capa hasta que la señal alcanza la capa de
salida, donde se produce la predicción final.

El feedforward es un proceso unidireccional, en el sentido de que la
información se mueve hacia adelante a través de la red sin retroalimentación
entre las capas.

### Diseño de redes neuronales

El diseño de una red neuronal implica la selección de su arquitectura,
incluyendo el número de capas, el número de neuronas en cada capa, la
elección de las funciones de activación y la definición de la topología de la
red.

Este proceso es crucial ya que la arquitectura de la red determina su
capacidad para aprender patrones complejos y generalizar a nuevos datos.
El diseño de la red debe equilibrar la capacidad de modelado con la
eficiencia computacional y la prevención del sobreajuste, lo que a menudo
requiere experimentación y ajuste fino.

### Parámetros de una red neuronal

Los parámetros de una red neuronal son los pesos y sesgos que se ajustan
durante el entrenamiento para minimizar el error de predicción.

Los pesos controlan la fuerza de la conexión entre las neuronas de
diferentes capas, mientras que los sesgos permiten a las neuronas ajustar
sus salidas independientemente de las entradas.

El número total de parámetros en una red depende de su arquitectura,
incluyendo el número de neuronas en cada capa y el número de capas en la
red.

El ajuste de estos parámetros es lo que permite a la red aprender de los
datos y mejorar su rendimiento en tareas específicas.

### Hiperparámetros de una red neuronal

Los hiperparámetros de una red neuronal son configuraciones que se
establecen antes del entrenamiento y que no se ajustan automáticamente
durante el proceso de aprendizaje.

Estos incluyen la tasa de aprendizaje, el tamaño del lote, el número de
épocas, la inicialización de los pesos y la elección del optimizador.

Los hiperparámetros juegan un papel crucial en el rendimiento de la red y su
capacidad para converger a una solución óptima.

La selección adecuada de los hiperparámetros es a menudo un proceso de
prueba y error y puede requerir técnicas de búsqueda y optimización.

### Funciones de Activación

Las funciones de activación son funciones matemáticas aplicadas a las
salidas de las neuronas en una red neuronal. Estas funciones introducen no
linealidades en el modelo, lo que es esencial para que la red pueda aprender
y modelar relaciones complejas en los datos.

Algunas funciones de activación comunes incluyen la sigmoide, la tangente
hiperbólica (tanh) y la unidad lineal rectificada (ReLU).

La elección de la función de activación depende del problema específico y
puede afectar significativamente el rendimiento y la convergencia de la red.



---

## 03 - Entrenamiento de redes neuronales

### Entrenamiento de redes neuronales

El entrenamiento de una red neuronal es el proceso de ajustar los
parámetros de la red (pesos y sesgos) para minimizar el error en las
predicciones.

Esto se logra mediante el uso de un conjunto de datos de entrenamiento,
donde se conoce la salida deseada para cada entrada.

El entrenamiento implica calcular el error o la pérdida entre las predicciones
de la red y las salidas reales, y luego utilizar un algoritmo de optimización,
como el descenso de gradiente, para actualizar los parámetros de la red en
la dirección que reduce el error.

Este proceso se repite iterativamente hasta que la red alcanza un nivel
satisfactorio de precisión

### Algoritmo de Backpropagation

El backpropagation es un algoritmo fundamental para entrenar redes
neuronales, optimizando los pesos de las conexiones para mejorar el
rendimiento de la red. Utiliza la regla de la cadena (derivadas) para calcular
el gradiente de la función de pérdida (error) respecto a cada peso,
ajustándolos para minimizar el error.

El algoritmo comienza con el cálculo del error entre la salida obtenida y la
deseada. Luego, usa este error para determinar los gradientes de los pesos
mediante derivadas parciales, y actualiza los pesos para reducir el error. Este
proceso se repite con múltiples ejemplos de entrenamiento.

La eficacia del backpropagation depende de la elección de la tasa de
aprendizaje y la inicialización de los pesos. Ajustar estos parámetros y aplicar
técnicas como el momentum o la regularización puede mejorar la
convergencia y prevenir el sobreajuste, optimizando el entrenamiento de la
red.

### Descenso por Gradiente

El descenso por gradiente es un algoritmo de optimización utilizado para
minimizar una función objetivo, como una función de pérdida o costo,
mediante la actualización iterativa de los parámetros del modelo en la
dirección opuesta al gradiente de la función. Este enfoque permite al modelo
aprender de manera efectiva y converger hacia el mínimo de la función.

El descenso por gradiente se utiliza ampliamente en el aprendizaje
automático y la inteligencia artificial para entrenar una amplia gama de
modelos, incluyendo redes neuronales. Su eficacia radica en su simplicidad y
flexibilidad, ya que puede adaptarse a diferentes tipos de funciones objetivo
y restricciones. Sin embargo, la elección de la tasa de aprendizaje y la
inicialización de los parámetros pueden influir significativamente en su
convergencia y eficiencia.

### Desvanecimiento de gradiente

El desvanecimiento de gradiente es un problema común en redes
neuronales profundas donde el gradiente de la función de pérdida
disminuye exponencialmente a medida que se propaga hacia atrás a través
de las capas, lo que resulta en actualizaciones insignificantes de los pesos en
las capas iniciales. Este fenómeno puede ralentizar el proceso de aprendizaje
o incluso impedir la convergencia.

El desvanecimiento de gradiente es especialmente problemático en
arquitecturas de redes neuronales profundas con muchas capas ocultas.
Para mitigar este problema, se han propuesto varias soluciones además de
ReLU, como la inicialización de pesos cuidadosa (por ejemplo, inicialización
de He) y el uso de arquitecturas de red especializadas (como las redes
neuronales recurrentes con puertas de olvido en LSTM).

### Solución: Funciones ReLU

La función de activación Rectified Linear Unit (ReLU) es una solución popular
al problema del desvanecimiento de gradiente. ReLU introduce no linealidad
en el modelo y permite un flujo más eficiente del gradiente, ya que su
derivada es constante y no se desvanece para valores positivos de entrada,
lo que facilita el entrenamiento de redes neuronales profundas.

A pesar de su popularidad, ReLU no está exenta de limitaciones. Una de ellas
es el problema de las neuronas "muertas", donde las neuronas pueden
quedar inactivas y dejar de contribuir al aprendizaje si reciben valores
negativos durante el entrenamiento. Para abordar esto, se han propuesto
variantes de ReLU como Leaky ReLU y Parametric ReLU (PReLU) que
permiten un pequeño gradiente para valores negativos de entrada.

### Técnica Dropout

Dropout es una técnica de regularización utilizada para prevenir el
sobreajuste en redes neuronales. Consiste en desactivar aleatoriamente
algunas neuronas durante el entrenamiento, lo que obliga a la red a
aprender representaciones más robustas y generalizables, ya que no puede
depender de la presencia de ninguna neurona en particular.

Dropout es una técnica simple pero efectiva que ha demostrado mejorar el
rendimiento de los modelos en diversas tareas de aprendizaje automático.
Sin embargo, su uso debe ser equilibrado, ya que una tasa de dropout
demasiado alta puede llevar a un aprendizaje insuficiente, mientras que una
tasa demasiado baja puede no proporcionar suficiente regularización. La
selección de la tasa de dropout adecuada suele requerir experimentación y
validación cruzada.


### Funciones de Error

Las funciones de error (de pérdida), son vitales para evaluar la eficacia la red
neuronal. Estas funciones cuantifican la diferencia entre las predicciones
realizadas por el modelo y los valores reales esperados, proporcionando una
función objetivo clara para la optimización durante el entrenamiento.

Existen varias funciones de error, cada una adecuada para diferentes tipos
de problemas. La función de error cuadrático medio (MSE) es común en
tareas de regresión, mientras que la entropía cruzada se utiliza
frecuentemente en problemas de clasificación. Cada tipo de función de error
tiene ventajas específicas dependiendo del contexto del problema y la
naturaleza de los datos.

Seleccionar la función de error adecuada es crucial para el rendimiento del
modelo. Una elección inapropiada puede llevar a un entrenamiento
ineficiente o convergencia hacia soluciones subóptimas. Además, algunas
funciones son más sensibles a las muestras atípicas, lo que puede influir en
cómo el modelo generaliza a partir de los datos de entrenamiento a
situaciones reales.

### Steps y Learning Rate Step

Un 'step' es una iteración donde la red neuronal procesa un batch de datos,
calcula el error usando una función de pérdida y actualiza sus pesos
mediante backpropagation. Este proceso es fundamental para ajustar los
parámetros del modelo y mejorar su rendimiento.
Learning Rate

El 'learning rate' determina la magnitud de las actualizaciones de los pesos
en cada step. Un valor adecuado es crucial para un entrenamiento efectivo;
un learning rate alto puede causar inestabilidad, mientras que uno bajo
puede ralentizar el aprendizaje. Ajustar correctamente este parámetro
facilita una rápida y efectiva convergencia hacia la solución óptima.

### Batch Size Epochs

El tamaño de lote (batch size) se refiere al número de muestras de
entrenamiento utilizadas en una iteración del descenso por gradiente. Un
tamaño de lote más pequeño puede proporcionar una estimación más
ruidosa del gradiente, lo que puede ayudar a escapar de mínimos locales,
mientras que un tamaño de lote más grande proporciona una estimación
más precisa y puede conducir a una convergencia más estable.

La elección del tamaño de lote es un compromiso entre la eficiencia
computacional y la calidad de la estimación del gradiente. Los tamaños de
lote más grandes pueden aprovechar mejor las capacidades de
paralelización de hardware moderno, como las GPU, pero pueden requerir
más memoria y pueden conducir a una convergencia más lenta. Por otro
lado, los tamaños de lote más pequeños pueden proporcionar una
actualización más frecuente de los parámetros, pero con un mayor ruido en
la estimación del gradiente.

### Espacio de búsqueda Mínimos locales y globales

En el contexto del entrenamiento de redes neuronales, el espacio de
búsqueda se refiere al conjunto de todos los posibles valores de los
parámetros de la red.

Dentro de este espacio, el objetivo es encontrar el conjunto de parámetros
que minimice la función de pérdida. Sin embargo, este espacio de búsqueda
es a menudo complejo y multidimensional, lo que puede llevar a la existencia
de múltiples mínimos locales.

Estos son puntos donde la función de pérdida es menor que en sus
alrededores inmediatos, pero no necesariamente el mínimo global.
La presencia de mínimos locales puede dificultar la convergencia del
algoritmo de entrenamiento hacia la solución óptima.

### Técnica Momentum (inercia)

La técnica de momentum es una modificación del algoritmo de descenso de
gradiente que tiene como objetivo acelerar la convergencia y evitar mínimos
locales.

En lugar de actualizar los parámetros de la red solo en función del gradiente
actual, el momentum incorpora una fracción del cambio de parámetros de la
iteración anterior.

Esto permite que el algoritmo acumule velocidad en direcciones con
gradientes consistentes y suavice las fluctuaciones en direcciones con
gradientes variables.

El momentum es un hiperparámetro que controla la cantidad de historia que
se incorpora en la actualización de los parámetros.

### Técnica Random Start

La técnica de random start, o inicio aleatorio, es una estrategia utilizada para
mitigar el problema de los mínimos locales en el entrenamiento de redes
neuronales.

Consiste en iniciar el algoritmo de optimización desde múltiples puntos
aleatorios en el espacio de parámetros y realizar el entrenamiento desde
cada uno de estos puntos de inicio. Luego, se selecciona la solución que
resulta en el menor error de validación.

Esta técnica aumenta las probabilidades de encontrar el mínimo global o un
mínimo local aceptable, ya que explora diferentes regiones del espacio de
búsqueda.

### Redes Neuronales Regresión

Las redes neuronales se utilizan en tareas de regresión para predecir valores
continuos a partir de datos de entrada.

En este contexto, la capa de salida de la red suele tener una sola neurona
para la predicción del valor objetivo, y se utiliza una función de activación
lineal o una función de identidad.

La función de pérdida más común para problemas de regresión es el error
cuadrático medio (MSE), que mide la diferencia cuadrada entre las
predicciones de la red y los valores reales.

Las redes neuronales pueden modelar relaciones complejas y no lineales
entre las variables de entrada y la variable objetivo, lo que las hace
adecuadas para una amplia gama de problemas de regresión.

### Transfer Learning

El transfer learning es una técnica en la que un modelo entrenado en una
tarea se reutiliza como punto de partida para una segunda tarea
relacionada.

Esto es especialmente útil en deep learning, donde entrenar redes
neuronales desde cero puede ser costoso en términos de tiempo y recursos
computacionales.

Al transferir los pesos aprendidos de una red preentrenada, se puede
acelerar el proceso de entrenamiento y mejorar el rendimiento en la nueva
tarea, incluso con un conjunto de datos más pequeño

### Tipos de Transfer Learning

Existen varios tipos de transfer learning, dependiendo de cómo se reutiliza el
modelo preentrenado.

El enfoque más común es el fine-tuning, donde se ajustan los pesos de toda
o parte de la red preentrenada durante el entrenamiento en la nueva tarea.
Otra técnica es el feature extraction, donde se utilizan las capas inferiores de
la red preentrenada para extraer características, mientras que las capas
superiores se entrenan desde cero para la nueva tarea. Estos enfoques
permiten aprovechar el conocimiento previo y adaptarlo a problemas
específicos.


### Especialización de modelos Fine Tuning

El finetuning, o ajuste fino, es un proceso de transfer learning donde se
realiza un ajuste adicional de los pesos de una red preentrenada en una
nueva tarea.

Este proceso permite especializar la red para la tarea específica, mejorando
su rendimiento en comparación con el entrenamiento desde cero.
Durante el finetuning, se suelen utilizar tasas de aprendizaje más bajas para
evitar alterar demasiado los pesos aprendidos previamente.
Esta técnica es particularmente efectiva cuando la nueva tarea es similar a la
tarea original, pero se dispone de un conjunto de datos más pequeño o
específico.

### Modelos Generalistas Pretraining

El pretraining, o entrenamiento previo, es el proceso de entrenar una red
neuronal en una tarea grande y general antes de aplicarla a una tarea
específica.

Los modelos resultantes, a menudo llamados modelos fundacionales,
aprenden representaciones ricas y versátiles que pueden ser transferidas a
una variedad de tareas posteriores.

Este enfoque es común en el procesamiento del lenguaje natural y la visión
por computadora, donde modelos como BERT y ResNet se preentrenan en
grandes conjuntos de datos antes de ser afinados para tareas específicas.
El pretraining aprovecha el aprendizaje no supervisado o semi-supervisado
para extraer conocimientos generales que son útiles en múltiples contextos.

---

## 04 - Transfer Learning

---
