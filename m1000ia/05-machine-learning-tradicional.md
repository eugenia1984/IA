# <img width="64" height="64" src="https://img.icons8.com/pieces/64/experimental-machine-learning-pieces.png" alt="machine learning"/> Machine learning tradicional

## Machine Learning

- 01 **Algoritmos de Aprendizaje Supervisado**

- 02 **Entrenamiento y métricas de evaluación**

- 03 **Algoritmos de Aprendizaje No Supervisado**

- 04 **PCA y detección de anomalías**

 --- 

## <img width="40" height="40" src="https://img.icons8.com/pieces/40/experimental-machine-learning-pieces.png" alt="machine learning"/>  Machine Learning Tradicional

"Con sus algoritmos clásicos y técnicas estadísticas, sigue siendo una piedra angular en el campo de la inteligencia artificial, proporcionando herramientas esenciales para el análisis y la comprensión de datos.

A pesar del auge del aprendizaje profundo, estos métodos tradicionales mantienen su relevancia, ofreciendo soluciones eficientes y interpretables que son cruciales en numerosas aplicaciones actuales."

---

## <img width="40" height="40" src="https://img.icons8.com/pieces/40/experimental-machine-learning-pieces.png" alt="machine learning"/>  Aprendizaje Supervisado

El aprendizaje supervisado es un enfoque del aprendizaje automático donde se utilizan datos etiquetados para entrenar modelos. Estos modelos aprenden a predecir salidas a partir de entradas, ajustando sus parámetros para minimizar errores y mejorar la precisión en predicciones futuras. Este método es fundamental para aplicaciones que requieren reconocimiento de
patrones o decisiones automáticas basadas en datos históricos.

En práctica, el aprendizaje supervisado se usa en una amplia gama de áreas, desde la detección de fraude hasta diagnósticos médicos. Al proporcionar ejemplos con entradas y salidas conocidas, los modelos pueden identificar relaciones y dependencias complejas en los datos, lo que les permite predecir resultados para nuevos conjuntos de datos de manera efectiva.

### Aprendizaje Supervisado - Regresión


La regresión, dentro del aprendizaje supervisado, implica la predicción de una variable continua basada en variables independientes. Este método es ampliamente usado en escenarios donde es necesario estimar valores futuros, como precios de vivienda, temperaturas, o niveles de ventas, basándose en datos históricos. Los modelos de regresión se ajustan a los
datos para encontrar una relación que minimice el error entre las predicciones y los valores reales.

Los algoritmos de regresión, como la regresión lineal y la regresión logística, son fundamentales en estadística y aprendizaje automático por su capacidad para modelar relaciones entre variables. Estos modelos proporcionan una base para entender cómo las variables independientes influyen en la variable dependiente, permitiendo no solo predecir, sino también explicar fenómenos.

### Aprendizaje Supervisado - Clasificación

La clasificación en el aprendizaje supervisado es un proceso donde el objetivo es asignar categorías discretas a las observaciones basándose en sus características. Esta técnica es esencial para tareas como el reconocimiento de imágenes, la detección de spam en correos electrónicos o la identificación de clientes potenciales para un producto. Los modelos de
clasificación utilizan datos etiquetados para aprender a diferenciar entre las distintas categorías y hacer predicciones sobre datos nuevos.

Los algoritmos comunes de clasificación incluyen árboles de decisión, máquinas de vector soporte, y redes neuronales, entre otros. Cada uno de estos algoritmos tiene sus propias fortalezas y se adapta mejor a diferentes tipos de problemas de clasificación. Por ejemplo, las redes neuronales son particularmente útiles en patrones complejos y datos no estructurados, como el lenguaje natural o imágenes.

Para asegurar la efectividad de un modelo de clasificación, es crucial implementar una meticulosa evaluación de su rendimiento. Métricas como precisión, recall, y la matriz de confusión son fundamentales para entender cómo se comporta el modelo en diferentes clases.

### Regresión lineal

La regresión lineal es uno de los métodos más simples y ampliamente utilizados en estadísticas y aprendizaje automático para predecir una variable dependiente continua a partir de una o más variables independientes. Este modelo asume que existe una relación lineal entre las variables de entrada y salida. Es particularmente útil para entender el
impacto directo de una variable sobre otra, lo que facilita la interpretación y la toma de decisiones basada en los coeficientes del modelo.

En la práctica, la regresión lineal puede aplicarse en diversos contextos, como en economía para predecir el PIB, en negocios para estimar ventas, o en salud para evaluar los efectos de un tratamiento médico. La simplicidad del modelo permite un análisis rápido y eficiente, aunque su precisión depende de cuán adecuada sea la suposición lineal para los datos en
cuestión.

Para mejorar el desempeño de un modelo de regresión lineal, es crucial realizar una buena selección de características y gestionar posibles problemas como la multicolinealidad, donde las variables independientes están altamente correlacionadas entre sí.

### Regresión logística

La regresión logística es un método de aprendizaje supervisado utilizado principalmente para problemas de clasificación binaria, donde el objetivo es predecir categorías discretas, como sí/no o verdadero/falso. A diferencia de la regresión lineal que predice valores continuos, la regresión logística estima la probabilidad de que una observación pertenezca a una categoría en particular, utilizando la función logística para mapear valores predichos a un rango entre 0 y 1.

Este modelo es particularmente útil en campos como la medicina para predecir la probabilidad de una enfermedad, o en finanzas para evaluar el riesgo de incumplimiento de un crédito. La regresión logística no solo ofrece predicciones en forma de clasificaciones, sino que también proporciona probabilidades que pueden ser cruciales para tomar decisiones informadas
cuando los resultados tienen diferentes grados de importancia o riesgo.

La interpretación de los coeficientes en un modelo de regresión logística es directa logrando que no solo sea efectiva para la predicción, sino también valiosa para entender la influencia relativa de las variables.

### <img width="40" height="40" src="https://img.icons8.com/pieces/40/experimental-machine-learning-pieces.png" alt="machine learning"/>  Árboles de decisión

Los árboles de decisión son modelos de aprendizaje supervisado quE funcionan dividiendo un conjunto de datos en subconjuntos más pequeños. En cada nodo del árbol, se toma una decisión basada en una pregunta o condición, que guía al algoritmo por diferentes caminos hasta llegar a un nodo hoja con una predicción de resultado.

Una de las principales ventajas de los árboles de decisión es su facilidad de interpretación y visualización, incluso para personas sin un profundo conocimiento técnico en análisis de datos. Esto los hace particularmente útiles en entornos empresariales o médicos donde las decisiones deben ser explicadas y justificadas claramente. Además, pueden manejar tanto datos numéricos como categóricos y son capaces de tratar con variables que tienen interacciones complejas que pueden ser difíciles de modelar con otros enfoques como los lineales.

Sin embargo, los árboles de decisión son susceptibles al sobreajuste, especialmente cuando no se limita la profundidad del árbol. Técnicas como la poda del árbol o el uso de ensambles de árboles pueden ayudar a mejorar la generalización del modelo y evitar que este se ajuste demasiado a los datos de entrenamiento.

### Random forest

Random Forest utiliza un conjunto de árboles para mejorar la robustez y precisión de las predicciones. Cada árbol se construye a partir de una muestra aleatoria de los datos de entrenamiento, y se toman decisiones basadas en la mayoría de votos para clasificación, o el promedio de las salidas para regresión. Este enfoque de ensamble ayuda a reducir la varianza sin aumentar significativamente el sesgo, lo que mejora considerablemente el rendimiento del modelo comparado con un solo árbol de decisión.

Tiene capacidad de manejar automáticamente interacciones complejas entre características y evitar el sobreajuste. A diferencia de un árbol de decisión único, donde decisiones profundas pueden aprender detalles demasiado específicos del conjunto de entrenamiento, se promedia múltiples árboles para equilibrar la decisión y generalizar mejor sobre datos no vistos.

Es eficaz tanto en problemas de clasificación como de regresión y proporciona indicadores útiles como la importancia de las características, que mide el impacto de cada característica en la precisión de la predicción.

### K-Nearest Neighbor

Algoritmo de aprendizaje supervisado que no requiere un modelo explícito para hacer predicciones. KNN realiza predicciones para un nuevo dato basándose en las similitudes con los más cercanos en el espacio de features del conjunto de entrenamiento.

Este método se basa en la premisa de que los datos similares existen en proximidad cercana y utiliza una métrica de distancia, como la distancia
euclidiana, para encontrar los 'k' vecinos más cercanos.

Una de las principales ventajas de KNN es su simplicidad y efectividad, especialmente en sistemas de recomendación y clasificación donde la relación entre las características es intuitivamente comprensible. Sin embargo, la elección del número 'k' es crucial; un valor demasiado bajo puede hacer que el algoritmo sea susceptible al ruido, y un valor demasiado
alto puede incluir puntos que son, de hecho, bastante irrelevantes para la clasificación, llevando a decisiones erróneas.

---


## <img width="40" height="40" src="https://img.icons8.com/pieces/40/experimental-machine-learning-pieces.png" alt="machine learning"/>  Métricas de Evaluación - Regresión

Existen métricas específicas que miden el error entre las predicciones y los valores reales.

Las métricas más comunes incluyen el Error Cuadrático Medio (MSE, por sus siglas en inglés), el Error Absoluto Medio (MAE), Error Absoluto Medio Porcentual (MAPE) y el Coeficiente de Determinación R2 

El MSE proporciona una penalización más grande a los errores más grandes, lo cual lo hace muy útil en situaciones donde los grandes desvíos son particularmente indeseables.

Coeficiente de Determinación mide la cantidad de variación en la variable dependiente que es predecible a partir de las variables independientes.

Aunque R2 es ampliamente utilizado por su interpretabilidad, es crucial recordar que un valor alto no necesariamente implica causalidad.

Elegir la métrica adecuada depende del contexto específico y los objetivos del análisis, y a menudo es útil considerar varias métricas para obtener una evaluación completa del rendimiento del modelo.


---


## <img width="40" height="40" src="https://img.icons8.com/pieces/40/experimental-machine-learning-pieces.png" alt="machine learning"/>  Métricas de Evaluación - Clasificación

Las métricas más comunes incluyen la precisión, que mide la proporción de predicciones correctas sobre el total de casos; la sensibilidad (tasa de verdaderos positivos) y la especificidad (tasa de verdaderos negativos) Otra métrica importante y robusta es el valor F1, que es el promedio armónico de la precisión y la sensibilidad. El valor F1 es especialmente útil cuando las clases están desbalanceadas, ya que no se ve tan influenciado por el número desproporcionado de verdaderos negativos, que es común en
datos con una gran clase mayoritaria. Este valor ofrece un balance entre la precisión y la sensibilidad.

La curva ROC (Receiver Operating Characteristic) y el área bajo la curva (AUC) son métricas esenciales para evaluar y comparar la performance de modelos de clasificación. La curva ROC muestra la relación entre la tasa de verdaderos positivos y la tasa de falsos positivos a varios umbrales de clasificación, mientras que el AUC proporciona una medida agregada de rendimiento en todos los umbrales posibles. Un AUC alto indica que el modelo tiene una buena medida de separabilidad entre las clases.


### Optimización de Hiperparámetros

Proceso clave en el aprendizaje automático que implica ajustar los parámetros que gobiernan el proceso de entrenamiento del modelo para mejorar su rendimiento y precisión.

A diferencia de los parámetros del modelo, que se aprenden durante el entrenamiento, los hiperparámetros deben ser establecidos antes del entrenamiento y tienen un impacto significativo en cómo el modelo aprende de los datos. Ejemplos comunes de hiperparámetros incluyen la tasa de aprendizaje, el número de capas en una red neuronal, o la profundidad
máxima de un árbol de decisión.

Para encontrar la combinación óptima de hiperparámetros, los científicos de datos utilizan técnicas exhaustivas como grid search y la búsqueda aleatoria, o bien técnicas más eficiente como la optimización bayesiana, que utiliza modelos probabilísticos para predecir la performance de los hiperparámetros y seleccionar nuevas combinaciones para probar basadas en los resultados anteriores.

---


## <img width="40" height="40" src="https://img.icons8.com/pieces/40/experimental-machine-learning-pieces.png" alt="machine learning"/>  Dataset Splitting Train, Validate, Test

Dividir el conjunto de datos en conjuntos de entrenamiento, validación y prueba es una práctica esencial para evaluar la efectividad y generalización de un modelo. Ayuda a prevenir el sobreajuste y asegura que el modelo pueda funcionar bien en datos no vistos, proporcionando una estimación honesta de su rendimiento en situaciones del mundo real.

El conjunto de entrenamiento se utiliza para ajustar los parámetros del modelo y representa la mayor parte del dataset. Durante el entrenamiento se aprende a reconocer patrones y a hacer predicciones, ajustando sus parámetros internos según el algoritmo específico que se esté utilizando.

El set de validación se utiliza para realizar una evaluación intermedia del modelo, permitiendo ajustar los hiperparámetros y tomar decisiones sobre las features sin contaminar la evaluación final con el set de prueba.

Finalmente, el conjunto de prueba se utiliza para evaluar la performance del modelo después de que se ha entrenado y validado. No debe utilizarse en ninguna fase del desarrollo del modelo, para que sirva como un indicador imparcial de cómo el modelo se comportará en datos no vistos.


### Cross Validation

Técnica de evaluación de modelos que busca mejorar la confiabilidad de las estimaciones de rendimiento del modelo, especialmente cuando los conjuntos de datos son limitados en tamaño.

El enfoque más común de validación cruzada es el k-fold cross-validation.

Este proceso implica dividir el conjunto de datos de manera aleatoria en 'k' subconjuntos (o folds). El modelo se entrena utilizando 'k-1' de estos subconjuntos, mientras que el subconjunto restante se utiliza como conjunto de prueba. Este proceso se repite 'k' veces, con cada uno de los 'k' subconjuntos utilizado exactamente una vez como conjunto de prueba.

Finalmente, el rendimiento del modelo se promedia sobre los 'k' ensayos para obtener una estimación más robusta de su rendimiento.

La principal ventaja de la validación cruzada es su capacidad para mitigar el problema de sobreajuste, proporcionando una visión más realista de cómo el modelo se desempeñará en un entorno operativo. Además, al utilizar todos los datos disponibles para entrenamiento y validación, maximiza la eficiencia del uso de los datos, lo cual es particularmente valioso en
escenarios donde los datos son escasos o costosos de obtener.

### Técnicas de Regularización

La regularización es una estrategia para prevenir el sobreajuste. Este método modifica la función de pérdida que el modelo optimiza al añadir un término de penalización a las magnitudes de los coeficientes del modelo.

Tipos comunes de regularización son L1 (Lasso) y L2 (Ridge). La regularización L1 penaliza la suma de los valores absolutos de los coeficientes, lo cual puede llevar a coeficientes con valor cero y por ende a modelos más simples y escasos. Por otro lado, la regularización L2 penaliza la suma de los cuadrados de los coeficientes, lo que reduce la magnitud de
los coeficientes pero sin hacerlos cero, proporcionando una solución más suave y menos sensible a los valores atípicos.

Utilizar correctamente la regularización puede significar la diferencia entre un modelo que es prácticamente útil y uno que no lo es bajo condiciones típicas de uso. Es especialmente útil en situaciones donde hay una gran cantidad de características o cuando las características son correlacionadas entre sí. 

### Overfitting y Underfitting

Overfitting ocurre cuando un modelo está demasiado ajustado a los datos de entrenamiento, capturando detalles y ruido que no generalizan a nuevos datos. Esto suele suceder cuando el modelo es demasiado complejo, con demasiados parámetros en relación con el número de observaciones. Como resultado, aunque el modelo puede funcionar excepcionalmente bien en el
conjunto de entrenamiento, su rendimiento en datos no vistos es malo. 

Underfitting, por otro lado, se da cuando un modelo es demasiado simple para capturar la estructura subyacente de los datos. Esto puede suceder si el modelo no tiene suficientes parámetros o si la técnica de aprendizaje no es adecuada para la complejidad de los datos. Los modelos que sufren de underfitting generalmente muestran un bajo rendimiento tanto en el conjunto de entrenamiento como en el de prueba, ya que no logran aprender las tendencias significativas de los datos.


### Aprendizaje NO Supervisado

El aprendizaje no supervisado es un tipo de aprendizaje donde los modelos se entrenan utilizando datos que no etiquetados. El objetivo aquí no es predecir una salida específica, sino explorar la estructura de los datos para identificar patrones o agrupaciones naturales descubriendo relaciones ocultas en los datos sin intervención sobre cómo deben agruparse.

Técnicas comunes incluyen el clustering y la reducción de dimensionalidad.

El clustering busca dividir los datos en grupos que compartan características similares, facilitando su análisis y comprensión. La reducción de dimensionalidad se utiliza para simplificar los datos sin perder información.

Especialmente valioso en campos como la detección de anomalías, segmentación de mercado y organización de grandes volúmenes de datos como documentos o imágenes, donde las etiquetas pueden no estar disponibles o ser difíciles de obtener. Al aplicar técnicas de aprendizaje no supervisado, se pueden obtener insights significativos de los datos, lo que facilita decisiones más informadas basadas en la estructura de los datos. 

### Agrupamiento Clustering

El clustering o agrupamiento es una técnica utilizada para dividir un conjunto de datos en grupos, de manera que los puntos de datos en el mismo grupo sean más similares entre sí que con los de otros grupos. Esta técnica es fundamental para identificar estructuras ocultas, patrones o categorías dentro de los datos sin la necesidad de etiquetas predefinidas.

Una aplicación común del clustering es en la segmentación de clientes para marketing, organización de documentos o en bioinformática para agrupar genes con funciones similares.

Existen varios algoritmos de clustering como K-means (que requiere determinar previamente el número de cluster), clustering jerárquico o DBSCAN (que no requieren una indicación directa del número de clusters)

---

## <img width="40" height="40" src="https://img.icons8.com/pieces/40/experimental-machine-learning-pieces.png" alt="machine learning"/> 

---
