# 💾 Fundamentos IA

"Los fundamentos de la inteligencia artificial son los pilares sobre los cuales se construyen todas las demás áreas de esta disciplina, proporcionando las bases teóricas y prácticas necesarias para desarrollar sistemas capaces de aprender, razonar y adaptarse, lo que está transformando radicalmente nuestra interacción con la tecnología y sentando las bases para innovaciones futuras en una amplia gama de aplicaciones y sectores."

---

## 💾 01 - Inteligencia Artificial: Aprendizaje y datos

### ¿Qué es la inteligencia artificial?

La Inteligencia Artificial (IA) es una rama de la informática que busca crear sistemas capaces de realizar tareas que normalmente requieren inteligencia humana, como el reconocimiento de voz, la toma de decisiones y la traducción entre idiomas.

Desde sus inicios en la década de 1950, la IA ha evolucionado significativamente, impulsada por avances en algoritmos, poder de cómputo y disponibilidad de datos.

La IA se clasifica generalmente en dos categorías: débil y fuerte. La IA débil se enfoca en sistemas diseñados para realizar tareas específicas, como los asistentes virtuales, mientras que la IA fuerte se refiere a sistemas con capacidades cognitivas generales similares a las humanas, aunque esta última sigue siendo en gran parte teórica.

- ¿A qué nos referimos cuando hablamos de que las máquinas aprenden?

- ¿A qué denominamos aprendizaje supervisado?

### Aprendizaje Supervisado

El aprendizaje supervisado es una técnica de aprendizaje automático donde se entrena a un modelo utilizando datos etiquetados.

Cada ejemplo de entrenamiento consiste en un par de entrada y salida, y el objetivo es aprender una función que mapee las entradas a las salidas correctas.

Este enfoque se utiliza comúnmente en tareas de clasificación y regresión, como la clasificación de correos electrónicos en spam o no spam.

El modelo hace predicciones sobre los datos de entrada y se ajusta en función de su precisión, mejorando su rendimiento a medida que se expone a más datos etiquetados.

- ¿A qué denominamos aprendizaje NO supervisado?

### Aprendizaje NO Supervisado

El aprendizaje no supervisado es un enfoque de aprendizaje que se utiliza para encontrar patrones ocultos o estructuras intrínsecas en datos no etiquetados.

A diferencia del aprendizaje supervisado, no hay respuestas correctas predefinidas, y el algoritmo debe hacer sentido de los datos por sí mismo.

Las técnicas comunes incluyen la agrupación de datos similares en grupos (clustering), detección de anomalías y la reducción de dimensionalidad para simplificar los datos sin perder información importante.

Un ejemplo clásico es la segmentación de clientes en grupos con características similares para estrategias de marketing dirigidas.

- ¿Conocen algún otro tipo de aprendizaje?

### Aprendizaje Por Refuerzo

El aprendizaje por refuerzo es un tipo de aprendizaje donde un agente aprende a tomar decisiones mediante la interacción con un entorno.

El agente realiza acciones y recibe recompensas o penalizaciones en función de los resultados de sus acciones.

El objetivo es aprender una política de comportamiento que maximice la recompensa total a lo largo del tiempo del agente.

Esta técnica se utiliza en diversos campos, como los juegos, la robótica y la optimización de procesos. Un ejemplo notable es el desarrollo de algoritmos de navegación autónoma que permiten a los vehículos aprender a maniobrar de manera óptima.

- ¿Qué necesitamos para entrenar una IA?

---

## 💾 02 - Datos Entrenamiento

### Conjuntos de Datos Dataset

Los datos son el fundamento de cualquier sistema de IA.

La calidad, diversidad y representatividad de los datos son cruciales para el entrenamiento de modelos precisos y justos.

Los datos deben ser recolectados y preprocesados cuidadosamente para asegurar que sean libres de sesgos y errores.

Además, es importante considerar aspectos éticos y de privacidad en la recolección y manejo de datos, especialmente cuando se trata de información sensible o personal.

### Exploración de Datos

La exploración de datos es una fase fundamental en el análisis de datos que implica investigar minuciosamente el conjunto de datos para descubrir patrones, tendencias, y anomalías.

Este proceso permite a los analistas de datos y científicos de datos obtener una comprensión profunda de la naturaleza y las características de los datos, lo que es crucial para formular hipótesis adecuadas y seleccionar las técnicas de modelado más apropiadas.

La exploración de datos incluye el examen de estadísticas descriptivas, como la media, la mediana, la desviación estándar y los cuartiles, así como la identificación de relaciones entre variables mediante la correlación y la covarianza.

Además, la exploración de datos ayuda a detectar problemas potenciales como valores faltantes, valores atípicos y sesgos en los datos, los cuales deben abordarse antes de proceder con el análisis o el modelado de datos.

### Visualización de Datos

La visualización de datos es una técnica poderosa que transforma datos numéricos y categóricos en representaciones gráficas, facilitando su comprensión e interpretación.

Las visualizaciones de datos pueden variar desde gráficos simples como histogramas, gráficos de barras y gráficos de líneas hasta representaciones más complejas como mapas de calor, gráficos de dispersión y diagramas de caja.

Estas herramientas visuales permiten a los analistas de datos y a los tomadores de decisiones identificar rápidamente patrones, tendencias y anomalías en los datos, lo que es esencial para el análisis exploratorio de datos, la comunicación de resultados y la toma de decisiones basada en datos.

La visualización de datos también juega un papel crucial en la presentación de resultados de manera clara y convincente a audiencias no técnicas, facilitando la comprensión y el intercambio de información compleja.

### Caracterización de Valores

La caracterización de datos implica un análisis detallado de las propiedades y atributos de un conjunto de datos, incluyendo la identificación de valores atípicos, el manejo de valores faltantes y la normalización de los datos.

Los valores atípicos son observaciones que se desvían significativamente de la mayoría de los datos y pueden ser indicativos de errores de medición, variabilidad natural o fenómenos inusuales. Es importante detectar y tratar adecuadamente estos valores para evitar distorsiones en el análisis.

Los valores faltantes son otra preocupación común en los conjuntos de datos, y su tratamiento puede incluir técnicas de imputación para estimar y reemplazar los datos ausentes.

La normalización es un proceso que ajusta la escala de los datos para que diferentes variables puedan compararse y combinarse de manera efectiva, lo cual es especialmente importante en algoritmos de aprendizaje automático que son sensibles a la escala de los datos.

Una cuidadosa caracterización de los datos es esencial para garantizar la calidad y la confiabilidad del análisis posterior.

### Datos Sesgados

El sesgo en los datos es una distorsión sistemática que puede afectar negativamente la precisión y la justicia de los modelos de inteligencia artificial.

Los sesgos pueden originarse en diversas fuentes, como la recopilación de datos, el preprocesamiento, o incluso las suposiciones subyacentes del modelo.

Un sesgo no detectado y no corregido puede llevar a decisiones injustas o discriminatorias, especialmente en aplicaciones sensibles como la contratación de personal, la concesión de créditos o la justicia penal.

Es crucial identificar y mitigar los sesgos en los datos para desarrollar modelos de IA que sean equitativos y representativos de la población objetivo.

### Tipos de datos en Inteligencia Artificial

Los datos en inteligencia artificial se pueden clasificar en dos categorías principales: estructurados y no estructurados.

Los datos estructurados son aquellos que se organizan en un formato definido, como tablas con números enteros, flotantes y categóricos. Estos datos son fáciles de analizar y procesar.

Por otro lado, los datos no estructurados carecen de una estructura predefinida y pueden incluir texto, imágenes, videos y audio. Estos datos son más complejos de manejar, pero contienen una riqueza de información que puede ser aprovechada por modelos de IA avanzados para tareas como el análisis de sentimientos, la visión por computadora y el procesamiento del lenguaje natural.

---

## 💾 03 - Machine Learning Deep Learning

### Machine Learning Tradicional

El término "Machine Learning Tradicional" generalmente se refiere a los métodos y algoritmos de aprendizaje automático que precedieron a la era del aprendizaje profundo (deep learning) basado redes neuronales.

Estos métodos incluyen algoritmos de aprendizaje supervisado como regresión lineal, regresión logística, máquinas de vectores de soporte (SVM), árboles de decisión y bosques aleatorios, así como técnicas de aprendizaje no supervisado como el análisis de componentes principales (PCA) y la agrupación k-means.

Se caracteriza por su enfoque en la extracción manual de características y la selección de modelos basados en la comprensión del dominio y la interpretación de los datos. Aunque estos métodos pueden ser menos potentes que las técnicas de aprendizaje profundo para ciertas tareas complejas, como el procesamiento del lenguaje natural y la visión por computadora, siguen siendo herramientas valiosas y ampliamente utilizadas para una variedad de problemas de aprendizaje automático debido a su simplicidad, eficiencia y facilidad de interpretación.

### Entrenamiento del modelo

El entrenamiento de un modelo de IA implica ajustar sus parámetros para que pueda realizar predicciones o decisiones precisas basadas en los datos de entrada.

Este proceso requiere un conjunto de datos de entrenamiento y un algoritmo de aprendizaje que optimice el rendimiento del modelo.

El entrenamiento puede ser supervisado, no supervisado o por refuerzo, dependiendo del tipo de tarea y los datos disponibles.

Es esencial dividir los datos en conjuntos de entrenamiento, validación y prueba para evaluar la generalización del modelo.


### Métricas de evaluación

Las métricas de evaluación son esenciales para medir el rendimiento de los modelos de IA. Estas métricas varían según la tarea y los objetivos del modelo.

En tareas de clasificación, se utilizan métricas como la precisión, la sensibilidad y la especificidad. Para problemas de regresión, el error cuadrático medio y el coeficiente de determinación son comunes.
 
Es importante elegir las métricas adecuadas para obtener una evaluación significativa del modelo y garantizar que se ajuste a las necesidades de la aplicación.

### Aprendizaje vs Memorización

El aprendizaje, en el contexto de la IA, se refiere a la capacidad de un modelo para generalizar a partir de datos de entrenamiento y hacer predicciones o tomar decisiones sobre datos no vistos anteriormente. Este proceso implica la identificación de patrones y relaciones subyacentes en los datos.

El objetivo del aprendizaje es desarrollar modelos que sean capaces de abstraer y aplicar el conocimiento adquirido a situaciones nuevas y desconocidas.

Por otro lado, la memorización en la IA se produce cuando un modelo aprende los datos de entrenamiento de memoria, sin captar la esencia o los patrones subyacentes. Esto puede llevar a un fenómeno conocido como sobreajuste (overfitting), donde el modelo se desempeña excepcionalmente bien en los datos de entrenamiento pero falla al generalizar a datos nuevos.

La memorización puede ser problemática porque el modelo se vuelve incapaz de adaptarse a situaciones que difieren ligeramente de lo que ha visto durante el entrenamiento.

### Redes Neuronales

Las redes neuronales son modelos computacionales inspirados en la estructura y el funcionamiento del cerebro humano, diseñados para simular la forma en que los seres humanos aprenden y procesan la información.

Están compuestas por unidades básicas llamadas neuronas artificiales o nodos, que están interconectadas en capas para formar una red. Cada neurona recibe señales de entrada, las combina de manera ponderada y aplica una función de activación para generar una señal de salida.

La información fluye a través de la red desde la capa de entrada hasta la capa de salida, y el aprendizaje se logra ajustando los pesos de las conexiones entre las neuronas durante un proceso de entrenamiento.

Las redes neuronales son capaces de aprender patrones complejos y no lineales, lo que las hace adecuadas para una amplia gama de aplicaciones en inteligencia artificial, incluyendo el reconocimiento de patrones, la clasificación, la regresión y el procesamiento del lenguaje natural.

### Deep Learning

El aprendizaje profundo es una rama avanzada del aprendizaje automático que utiliza redes neuronales profundas con muchas capas ocultas para modelar relaciones complejas en los datos.

Esta técnica ha demostrado ser muy efectiva en una amplia gama de aplicaciones, como el reconocimiento de imágenes, el procesamiento del lenguaje natural y la generación de contenido.

Un ejemplo notable es el reconocimiento facial en smartphones, donde el aprendizaje profundo permite identificar rostros con alta precisión incluso en condiciones variables de iluminación y orientación.

### Computer Vision

El aprendizaje profundo es una rama avanzada del aprendizaje automático que utiliza redes neuronales profundas con muchas capas ocultas para modelar relaciones complejas en los datos.

Esta técnica ha demostrado ser muy efectiva en una amplia gama de aplicaciones, como el reconocimiento de imágenes, el procesamiento del lenguaje natural y la generación de contenido.

Un ejemplo notable es el reconocimiento facial en smartphones, donde el aprendizaje profundo permite identificar rostros con alta precisión incluso en condiciones variables de iluminación y orientación.

### Procesamiento Del Lenguaje Natural

El procesamiento del lenguaje natural (NLP) es una rama de la IA que se centra en la interacción entre las computadoras y el lenguaje humano. NLP permite a las máquinas leer, entender y generar texto de manera similar a como lo hacen los humanos.

Esto incluye tareas como la traducción automática, la generación de resúmenes y la extracción de información. Los avances en NLP han llevado al desarrollo de chatbots y asistentes virtuales capaces de comprender y responder a consultas en lenguaje natural, mejorando la interacción entre humanos y máquinas.

### Sistemas de Recomendación

Los sistemas de recomendación son herramientas de IA que sugieren productos, servicios o contenidos a los usuarios en función de sus preferencias y comportamientos anteriores.

Estos sistemas utilizan algoritmos para analizar los patrones de consumo y predecir qué elementos podrían interesar al usuario. Un ejemplo común son las recomendaciones personalizadas en plataformas de streaming como Netflix, que sugieren películas y series basadas en el historial de visualización del usuario.

### Despliegue de Modelos

El despliegue es el proceso de integrar un modelo de IA entrenado en un entorno de producción para que pueda ser utilizado en aplicaciones reales.

Esto implica convertir el modelo en un servicio accesible, asegurando su escalabilidad y rendimiento.

Es crucial monitorear el modelo desplegado para detectar posibles problemas y actualizarlo regularmente para mantener su relevancia y precisión. El despliegue exitoso de un modelo de IA requiere una colaboración estrecha entre científicos de datos, ingenieros de software y otros profesionales.

----

## 💾 04 -  Ética Desarrollo Sustentable

### Desafíos Ética en IA

A medida que la IA se integra cada vez más en nuestra vida cotidiana, surgen preocupaciones éticas y desafíos relacionados con la privacidad, la seguridad y la justicia.

Los sesgos en los datos de entrenamiento pueden llevar a decisiones injustas o discriminatorias, y la transparencia de los algoritmos es crucial para mantener la confianza del público.

Además, la automatización impulsada por la IA plantea preguntas sobre el futuro del trabajo y la distribución equitativa de los beneficios tecnológicos.

### Desarrollo Sustentable

El desarrollo sustentable en inteligencia artificial (IA) implica la creación y aplicación de tecnologías de IA de manera que promuevan la sostenibilidad ambiental, social y económica.

Este enfoque busca equilibrar el avance tecnológico con la responsabilidad ética y la conservación de los recursos naturales. En la práctica, esto significa diseñar sistemas de IA que optimicen el uso de la energía, reduzcan la huella de carbono y minimicen el desperdicio.

Además, el desarrollo sustentable en IA implica asegurar que las tecnologías sean accesibles y beneficiosas para todos los sectores de la sociedad, evitando la exacerbación de desigualdades y promoviendo la inclusión.

Al integrar principios de sostenibilidad en el desarrollo de la IA, podemos garantizar que estas tecnologías contribuyan positivamente a los objetivos globales de desarrollo sostenible y al bienestar de las generaciones futuras.

### Programando IA con Python

Python se ha establecido como el lenguaje de programación predominante en el campo de la inteligencia artificial y el aprendizaje automático. Su sintaxis clara y concisa, junto con su amplio ecosistema de bibliotecas y herramientas especializadas como NumPy, Pandas, TensorFlow y scikit-learn, lo hacen ideal para el desarrollo y la experimentación de modelos de IA.

Python facilita la manipulación de datos, la implementación de algoritmos de aprendizaje automático y la visualización de resultados, lo que permite a los científicos de datos y desarrolladores construir soluciones de IA de manera eficiente y efectiva.

### Python con Google Colab

Google Colab es una plataforma de computación en la nube que permite a los usuarios escribir y ejecutar código Python en un entorno de navegador.

Es especialmente popular en el campo de la inteligencia artificial por su facilidad de uso, acceso gratuito a recursos computacionales como GPUs y TPUs, y su integración con Google Drive para el almacenamiento de datos y modelos. Colab proporciona un entorno colaborativo donde los científicos de datos y los investigadores pueden compartir y trabajar en cuadernos de Jupyter, facilitando el desarrollo y la experimentación de modelos de IA sin la necesidad de una configuración de hardware compleja.

---
