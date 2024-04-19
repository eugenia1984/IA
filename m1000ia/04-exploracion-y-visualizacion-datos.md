# 💾  Exploración y Visualización de datos

## Exploración y visualización

- 01 **¿Qué es la exploración de datos?**

- 02 **Estadística descriptiva**

- 03 **Visualización de datos**

- 04 **Recomendaciones para EDA**


"La exploración y análisis de datos es el proceso a través del los transformamos en conocimientos profundos y accionables, lo que constituye la base
para tomar decisiones fundamentadas y estratégicas. Esta disciplina es crucial porque permite descubrir patrones ocultos, predecir tendencias futuras y
optimizar procesos, convirtiéndose así en una pieza clave para el éxito de un proyecto de IA." 

---

## 💾  1 - Exploración y visualización de datos

### Ciencia de Datos

La ciencia de datos es una disciplina que combina estadísticas, análisis de datos, aprendizaje automático y técnicas de visualización para extraer
conocimientos y tomar decisiones basadas en datos.

En la era actual, donde se generan enormes cantidades de datos, la ciencia de datos se ha vuelto esencial para comprender y resolver problemas
complejos en diversos campos, como la medicina, las finanzas y la tecnología.

La exploración, análisis y visualización de datos son pasos clave en el proceso de la ciencia de datos, permitiendo a los científicos de datos y
analistas descubrir patrones, tendencias y relaciones ocultas en los datos.

### Análisis de Datos

El proceso de análisis de datos en la ciencia de datos sigue un flujo de trabajo estructurado que comienza con la recolección de datos de diversas
fuentes.

Una vez recopilados, los datos deben limpiarse y preprocesarse para eliminar errores, valores faltantes y datos irrelevantes.

La exploración de datos implica examinar los datos de manera visual y estadística para comprender su estructura y características.

El análisis de datos utiliza técnicas estadísticas y algoritmos de aprendizaje automático para extraer conocimientos y patrones.

Finalmente, la visualización de datos convierte los resultados del análisis en gráficos y tablas comprensibles, facilitando la interpretación y comunicación
de los hallazgos.

### Beneficios del Análisis de Datos

- **Descubrimiento de patrones**: La exploración de datos ayuda a identificar patrones, tendencias y relaciones ocultas en los datos.

- **Detección de anomalías**: Permite detectar valores atípicos y errores en los datos que podrían afectar el análisis posterior.

- **Selección de características**: Facilita la identificación de las variables más relevantes para el modelado.

- **Toma de decisiones informada**: Proporciona una base sólida para la toma de decisiones basada en datos y la formulación de hipótesis.

- **Comunicación efectiva**: Los gráficos y visualizaciones generados durante la exploración ayudan a comunicar los hallazgos de manera clara y
comprensible.

### Poner en contexto a los datos para el análisis

- **Entender el Origen**: Es crucial conocer la fuente de los datos, el proceso de recopilación y cualquier factor que pueda influir en los resultados. Esto
incluye comprender las limitaciones y suposiciones inherentes a los datos.

- **Definir el Objetivo**: El contexto ayuda a definir el objetivo del análisis y a formular preguntas de investigación relevantes. Esto guía la selección de
métodos y técnicas adecuadas para el análisis de datos.

- **Interpretación Adecuada**: El contexto proporciona el marco necesario para interpretar correctamente los resultados del análisis. Sin este entendimiento,
existe el riesgo de sacar conclusiones erróneas o irrelevantes.

- **Comunicación Efectiva**: Al presentar los hallazgos, es importante contextualizar los resultados para que sean comprensibles y significativos
para la audiencia.

### Exploración de Datos

La exploración de datos es un paso fundamental en la ciencia de datos que permite a los analistas comprender la naturaleza y las características de los
datos con los que trabajan.

A través de la exploración de datos, se pueden identificar patrones iniciales, detectar valores atípicos, y formular hipótesis para investigaciones más
profundas.

Esta fase preliminar proporciona una visión crucial que guía el análisis y modelado de datos subsiguiente, asegurando que las decisiones basadas en
datos sean informadas y confiables.

Herramientas como gráficos de dispersión, histogramas y estadísticas descriptivas son comúnmente utilizadas en esta etapa para visualizar y
resumir los datos.

### Estadística Descriptiva

Las estadísticas descriptivas proporcionan un resumen cuantitativo de las características principales de un conjunto de datos.

Medidas de tendencia central, como la media, mediana y moda, ofrecen una idea del valor típico o central en los datos.

Las medidas de dispersión, como la varianza, desviación estándar y rango intercuartílico, indican la variabilidad o dispersión de los datos alrededor de
la medida central.

Estas estadísticas son esenciales para entender la distribución y la forma general de los datos, y son un primer paso crucial en el análisis de datos para
identificar posibles áreas de interés o preocupación.

### Media, Mediana y Moda

La media es el valor promedio de un conjunto de datos. Se calcula sumando todos los valores y dividiendo por el número total de valores. La media es útil
para obtener una idea general del valor típico en un conjunto de datos. Es apropiada cuando los datos son simétricos y no hay valores atípicos
extremos.

La mediana es el valor que se encuentra en el medio de un conjunto de datos ordenados. Si hay un número par de datos, la mediana es el promedio
de los dos valores centrales. La mediana es útil cuando los datos tienen una distribución asimétrica o cuando hay valores atípicos, ya que no se ve
afectada tanto por estos como la media.

La moda es el valor o valores que aparecen con mayor frecuencia en un conjunto de datos.La moda es útil para identificar el valor más común en un
conjunto de datos. Es especialmente relevante en datos categóricos o cuando se desea resaltar el valor más frecuente.

**Diferencias a tener presente:**

- La media se ve afectada por valores atípicos, mientras que la mediana y la moda son más resistentes.

- La mediana proporciona un mejor resumen de la tendencia central en distribuciones asimétricas.

- La moda puede no ser única, especialmente en distribuciones con múltiples picos.

**Cuándo usar cada una:**

- Usa la media para datos simétricos sin valores atípicos.

- Usa la mediana para datos asimétricos o con valores atípicos.

- Usa la moda para datos categóricos o para resaltar el valor más común.

### Desvío, Varianza

El desvío estándar es una medida de dispersión que indica cuánto se alejan los valores en un conjunto de datos de la media.

Un desvío estándar bajo indica que los valores tienden a estar cerca de la media, mientras que un desvío estándar alto indica que los valores están
más dispersos. El desvío estándar es útil para entender la variabilidad en un conjunto de datos.

Es especialmente relevante en contextos donde la distribución de los datos es importante, como en análisis estadísticos y control de calidad.

La varianza es una medida de dispersión que indica cuán dispersos están los valores en un conjunto de datos respecto a la media. Es el cuadrado del
desvío estándar.

### Rango Intercuartílico

El rango intercuartílico es una medida de dispersión que indica la variabilidad en un conjunto de datos eliminando los valores extremos. Se
calcula como la diferencia entre el tercer cuartil (Q3) y el primer cuartil (Q1).

IQR = Q3−Q1, donde Q3 es el valor que separa los primeros tres cuartos de los datos del último cuarto, y Q1 es el valor que separa el primer cuarto de
los datos del resto. 

El IQR es útil para identificar la dispersión de los datos centrales, minimizando el efecto de valores atípicos. Es especialmente relevante en
análisis de datos donde los valores extremos pueden distorsionar la interpretación.


### EDA: Análisis - Exploratorio de Datos

El Análisis Exploratorio de Datos (EDA) es una técnica utilizada para resumir las características principales de los datos y detectar patrones o anomalías.

Se basa en la visualización de datos y estadísticas descriptivas para explorar la estructura y las relaciones entre las variables.

El EDA es una fase interactiva y flexible en el proceso de análisis de datos, donde se pueden generar hipótesis y preguntas que guiarán el análisis
posterior. Herramientas como gráficos de dispersión, histogramas, diagramas de caja y mapas de calor son comúnmente utilizadas en el EDA para visualizar la distribución y las relaciones entre las variables.


### Tipos de Datos

Los datos en la ciencia de datos se clasifican en diferentes tipos según su naturaleza y características.

Los datos cualitativos, o categóricos, representan atributos o categorías, como género o color.

Los datos cuantitativos, o numéricos, representan cantidades medibles, como edad o ingresos. Dentro de los datos cuantitativos, se distinguen los
datos discretos, que toman valores enteros, como el número de hijos, y los datos continuos, que pueden tomar cualquier valor dentro de un rango,
como la altura.

La comprensión de los tipos de datos es crucial para elegir las técnicas de análisis y visualización adecuadas.

### Tratamiento Datos Categóricos

- **Visualización de Frecuencias**: Los gráficos de barras y los diagramas de sectores son útiles para visualizar la distribución de frecuencias de las
variables categóricas y comparar proporciones entre categorías.

- **Análisis de Asociación**: Las tablas de contingencia y las pruebas de chi-cuadrado se utilizan para examinar la relación entre dos variables
categóricas y determinar si existe una asociación significativa entre ellas.

- **Codificación de Variables**: Para incluir variables categóricas en modelos de machine learning, es necesario convertirlas en formatos numéricos mediante
técnicas de codificación, como la codificación one-hot o la codificación de etiquetas.

- **Consideraciones Especiales**: Al analizar datos categóricos, es importante considerar el orden de las categorías (si es aplicable) y la posible presencia
de categorías con frecuencias muy bajas, que pueden requerir un tratamiento especial.

### Limpieza de Datos

La limpieza de datos es un paso crucial en el proceso de análisis de datos para garantizar la calidad y precisión de los resultados. Implica identificar y
tratar problemas como valores faltantes, valores atípicos, errores de entrada y datos duplicados.

Los valores faltantes pueden ser imputados o eliminados según el contexto.

Los valores atípicos deben ser examinados para determinar si son errores o variaciones naturales.

La limpieza de datos asegura que el conjunto de datos esté listo para el análisis y reduce el riesgo de conclusiones erróneas.

### Imputación de valores faltantes

La imputación de valores faltantes es un paso crítico en la preparación de datos para garantizar la calidad y completitud del conjunto de datos.

Los valores faltantes pueden ocurrir por diversas razones, como errores en la recopilación de datos o la ausencia de información. La imputación consiste
en reemplazar estos valores faltantes con estimaciones basadas en el resto de los datos disponibles.

Existen diferentes métodos de imputación, como la imputación por la media, mediana o moda para variables numéricas, y la imputación por la moda o técnicas más sofisticadas como la imputación múltiple o el uso de modelos predictivos para variables categóricas.

La elección del método de imputación depende de la naturaleza de los datos y del patrón de los valores faltantes.

### Datos no estructurados: Texto

La exploración de datos de texto implica el análisis y procesamiento de información en forma de texto natural para extraer patrones, tendencias y conocimientos útiles.

**Comparativa con datos estructurados:**

- **Estructura**: Los datos tabulares están organizados en filas y columnas, con cada columna representando una variable y cada fila representando un registro. En cambio, los datos de texto no tienen una estructura predefinida y pueden variar en formato, longitud y contenido.
  
- **Análisis**: El análisis de datos tabulares suele ser más directo, utilizando técnicas estadísticas y de modelado convencionales. El análisis de datos de texto requiere técnicas de específicas de NLP.
  
- **Almacenamiento**: Los datos tabulares se almacenan típicamente en bases de datos relacionales o en hojas de cálculo. Los datos de texto pueden almacenarse en archivos de texto, bases de datos no relacionales o sistemas de gestión de contenido.

**Ventajas de los Datos de Texto:**

- **Riqueza de Información**: Los datos de texto pueden contener una gran cantidad de información cualitativa y matices que no siempre están
presentes en los datos tabulares.

- **Flexibilidad**: Los datos de texto pueden adaptarse a una amplia variedad de formatos y estructuras, lo que los hace útiles para una
amplia gama de aplicaciones.

- **Insights Profundos**: El análisis de texto puede revelar insights profundos sobre comportamientos, opiniones y tendencias que
pueden ser difíciles de obtener a partir de datos tabulares.

**Desventajas de los Datos de Texto:**

- **Complejidad**: El procesamiento y análisis de datos de texto pueden ser más complejos y requieren habilidades especializadas en NLP y
técnicas avanzadas de análisis.

- **Inconsistencia**: Los datos de texto pueden ser inconsistentes debido a errores de ortografía, variaciones en la gramática o el uso de jerga, lo que puede dificultar su análisis.
  
- **Requerimientos de Almacenamiento**: Los datos de texto pueden ocupar más espacio de almacenamiento en comparación con los datos
tabulares, especialmente si se trata de grandes volúmenes de texto.

### Datos no estructurados: Imágenes

La exploración de datos de imágenes implica el análisis y procesamiento de información visual para extraer patrones, características y conocimientos útiles. Las imágenes son un tipo de dato no estructurado que requiere técnicas específicas de visión por computadora y aprendizaje automático.

Las imágenes son datos no estructurados que no tienen una estructura predefinida y consisten en píxeles que representan información visual.

Las imágenes se almacenan en formatos de archivo específicos (como JPEG, PNG) y pueden requerir sistemas de almacenamiento especializados para
grandes volúmenes de datos visuales.

**Ventajas de los Datos de Imágenes:**

- **Riqueza de Información**: Las imágenes pueden contener una gran cantidad de información visual que puede ser utilizada para diversas
aplicaciones, desde el reconocimiento de objetos hasta el diagnóstico médico.

- **Aplicabilidad**: Los datos de imágenes tienen aplicaciones en una amplia variedad de campos, incluyendo la medicina, la seguridad, la
agricultura, y la industria manufacturera.

- **Automatización**: El análisis de imágenes permite la automatización de tareas que requieren reconocimiento visual, como la inspección de
productos o el monitoreo de áreas.

---
