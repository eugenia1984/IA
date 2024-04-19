# 💾  Exploración y Visualización de datos

## Exploración y visualización

- 01 **¿Qué es la exploración de datos?**

- 02 **Estadística descriptiva**

- 03 **Visualización de datos**

- 04 **Recomendaciones para EDA**


"La exploración y análisis de datos es el proceso a través del los transformamos en conocimientos profundos y accionables, lo que constituye la base para tomar decisiones fundamentadas y estratégicas. Esta disciplina es crucial porque permite descubrir patrones ocultos, predecir tendencias futuras y optimizar procesos, convirtiéndose así en una pieza clave para el éxito de un proyecto de IA." 

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


---

## 💾 2 -  Estadística Descriptiva

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

**Desventajas de los Datos de Imágenes:**

- **Complejidad**: El procesamiento y análisis de imágenes pueden ser más complejos y computacionalmente intensivos en comparación con los
datos estructurados.

- **Variabilidad**: Las imágenes pueden variar en calidad, iluminación, ángulo y otros factores que pueden afectar el análisis.

- **Requerimientos de Almacenamiento**: Las imágenes, especialmente en alta resolución, pueden requerir una cantidad significativa de
almacenamiento, lo que puede ser un desafío para sistemas con recursos limitados.

### Consideraciones para los datos faltantes
 
Identificación de Patrones: Es importante analizar los patrones de datos faltantes para determinar si la ausencia de datos es aleatoria o si existe un sesgo. Esto puede afectar la validez de los resultados del análisis.

Impacto en el Análisis: Los datos faltantes pueden afectar significativamente el análisis estadístico y los modelos predictivos. Es importante evaluar el impacto de la imputación en los resultados y considerar la incertidumbre asociada.

Documentación y Transparencia: Es esencial documentar cómo se han manejado los datos faltantes y ser transparente sobre las decisiones
tomadas, ya que esto puede influir en la interpretación de los resultados.

### Remoción de valores atípicos (outliers)

La remoción de valores atípicos es una técnica importante en la limpieza de datos, ya que estos valores pueden distorsionar el análisis y los resultados de los modelos de machine learning.

Los valores atípicos son observaciones que se desvían significativamente del resto de los datos y pueden ser el resultado de errores de medición, variabilidad natural o anomalías genuinas.

Para identificarlos, se pueden utilizar métodos como el rango intercuartílico (IQR), la desviación estándar o la visualización mediante diagramas de caja.

Una vez identificados, los valores atípicos pueden ser eliminados o ajustados para minimizar su impacto en el análisis.

Es importante tener en cuenta que la remoción de valores atípicos debe hacerse con cautela, ya que en algunos casos pueden contener información
valiosa.

### Transformación de Datos

La transformación de datos es el proceso de modificar los datos para facilitar su análisis y modelado.

Incluye técnicas como la normalización, que ajusta los datos a una escala común, y la estandarización, que centra los datos en torno a la media con una desviación estándar de uno.

La transformación también puede involucrar la codificación de variables categóricas en numéricas y la creación de variables derivadas.

Estas transformaciones son esenciales para preparar los datos para algoritmos de aprendizaje automático y para mejorar la interpretación de los
resultados.

### Correlación y Causalidad

La correlación y la causalidad son conceptos clave en el análisis de datos.

La correlación mide la relación lineal entre dos variables, indicando cómo cambia una variable en relación con otra.

Sin embargo, una correlación no implica causalidad; es decir, no indica que una variable sea la causa de los cambios en la otra.

La causalidad requiere evidencia adicional, como experimentos controlados o análisis estadísticos más sofisticados. Es importante no confundir
correlación con causalidad al interpretar los resultados del análisis de datos.

### Gráfico Histograma

Los histogramas son una herramienta fundamental en la visualización de datos, especialmente útil para entender la distribución de una variable
cuantitativa.

Al agrupar los datos en intervalos o "bins", los histogramas muestran la frecuencia o cantidad de datos que caen dentro de cada intervalo,
proporcionando una visión clara de la forma de la distribución, ya sea simétrica, sesgada, bimodal o uniforme.

Este tipo de gráfico es esencial para identificar patrones como la centralidad de los datos y la presencia de valores atípicos, lo que a su vez informa decisiones posteriores en el análisis de datos.

### Gráfico de barras

Los gráficos de barras son una herramienta de visualización versátil y ampliamente utilizada para comparar cantidades de diferentes categorías.

Cada barra representa una categoría, y su longitud o altura es proporcional a la cantidad que representa.

Los gráficos de barras se pueden presentar de manera vertical u horizontal y son particularmente efectivos para mostrar diferencias entre grupos, tendencias en datos categóricos y comparaciones de frecuencia.

Al proporcionar una representación visual clara y directa, facilitan la interpretación y el análisis de datos categóricos.


### Diagramas de Caja Boxplot

Los diagramas de caja, o boxplots, son una herramienta estadística visual que proporciona una representación concisa de la distribución de una
variable cuantitativa.

Muestran la mediana, los cuartiles y los valores atípicos, ofreciendo una visión rápida de la variabilidad y simetría de los datos.

Los diagramas de caja son especialmente útiles para comparar distribuciones entre diferentes grupos o categorías y para identificar posibles
valores atípicos que podrían influir en el análisis posterior.

Su capacidad para resumir información clave sobre la distribución de los datos los hace indispensables en la exploración y análisis de datos.

### Diagramas de Violín

Los gráficos de violín combinan características de los diagramas de caja y los gráficos de densidad de kernel para proporcionar una representación más rica de la distribución de los datos.

Muestran la densidad de los datos en diferentes valores, con un ancho más amplio donde los datos son más densos.

Los gráficos de violín son particularmente útiles para comparar la distribución de los datos entre diferentes grupos o categorías.

### Gráfico de líneas

Los gráficos de líneas son una herramienta esencial en la visualización de datos para mostrar tendencias y cambios a lo largo del tiempo.

Cada punto en el gráfico representa una observación en un momento específico, y la línea conecta estos puntos para mostrar la evolución de la
variable.

Los gráficos de líneas son particularmente efectivos para visualizar datos temporales, destacando tendencias ascendentes, descendentes o
estacionarias. 

Además, permiten comparar múltiples series temporales en el mismo gráfico, facilitando la identificación de patrones y relaciones entre variables a lo largo del tiempo.

### Gráfico de áreas

Los gráficos de área son similares a los gráficos de líneas, pero con el área bajo la línea rellena con color o patrones.

Son útiles para visualizar la evolución de una cantidad a lo largo del tiempo y para comparar diferentes series de datos.

Los gráficos de área pueden ser apilados para mostrar la contribución de cada serie al total o apilados al 100% para resaltar la proporción de cada serie en el total.

### Mapas de Calor

Los mapas de calor son una técnica de visualización que utiliza colores para representar la magnitud de los valores en una matriz bidimensional.

Son particularmente útiles para visualizar correlaciones, patrones y tendencias en grandes conjuntos de datos, como matrices de correlación o
tablas de contingencia.

Los cambios graduales en el color permiten identificar áreas de interés, como relaciones fuertes o débiles entre variables. Al proporcionar una
representación visual intuitiva de la información, los mapas de calor facilitan la identificación de patrones y la toma de decisiones basada en datos.


### Recomendaciones para realizar un buen EDA

Conocer los datos: Antes de comenzar la exploración, es importante entender la naturaleza y el contexto de los datos.

Limpieza de datos: Asegurarse de que los datos estén limpios y libres de errores antes de proceder al análisis.

Uso de gráficos adecuados: Elegir el tipo de gráfico o visualización que mejor represente la información que se desea transmitir.

Análisis iterativo: La exploración de datos es un proceso iterativo; no dude en volver atrás y ajustar su análisis a medida que descubre nueva información.

Documentación: Mantener un registro de los hallazgos y las decisiones tomadas durante la exploración para facilitar la reproducibilidad y la
revisión.


### Recomendaciones Exploración de datos
 
- **Explorar relaciones entre variables**: Utilice gráficos de dispersión, mapas de calor y otras técnicas de visualización para investigar las relaciones entre las variables. Esto puede ayudar a identificar patrones y correlaciones que podrían ser importantes para el análisis posterior.

- **Considerar la dimensión temporal**: Si sus datos tienen una componente temporal, asegúrese de explorar cómo las variables cambian con el tiempo.
  
Los gráficos de líneas y las series temporales pueden ser útiles para visualizar tendencias y patrones estacionales.

Usar subconjuntos de datos: Si está trabajando con un conjunto de datos grande, considere usar muestras o subconjuntos de datos para explorar y
visualizar. Esto puede hacer que el proceso sea más manejable y rápido, especialmente en las etapas iniciales de la exploración.
 
Estar atento a los sesgos: Reconozca que la forma en que se recopilan y procesan los datos puede introducir sesgos. Sea crítico con los datos y
considere cómo podrían afectar sus conclusiones.

### Recomendaciones Visualización de datos

- **Mantener la simplicidad**: Una visualización efectiva es aquella que transmite la información de manera clara y concisa. Evite agregar elementos innecesarios que puedan distraer o confundir al espectador.
  
- **Elegir colores cuidadosamente**: Utilice colores de manera estratégica para resaltar información importante y para distinguir entre diferentes categorías.
  
- **Etiquetar adecuadamente**: Asegúrese de que los ejes, leyendas y títulos estén claramente etiquetados para facilitar la interpretación de los gráficos. 
Las etiquetas deben ser precisas y descriptivas.

- **Considerar la audiencia**: Adapte su visualización al público objetivo. Asegúrese de que el nivel de complejidad y el tipo de visualización sean apropiados para las personas a las que se dirige.

- **Verificar la precisión**: Antes de presentar o publicar sus visualizaciones, verifique que sean precisas y que reflejen correctamente los datos subyacentes. Los errores en las visualizaciones pueden llevar a interpretaciones erróneas.

### Qué hacer y qué no hacer durante el análisis de datos

**Qué Hacer:**

- Ser curioso: Haga preguntas sobre los datos y busque respuestas a través de la exploración.

- Ser crítico: Evalúe críticamente los resultados y verifique si tienen sentido en el contexto de los datos.

- Ser creativo: Experimente con diferentes técnicas de visualización y análisis para obtener nuevos conocimientos.

**Qué No Hacer:**

- Ignorar los valores atípicos: No descarte los valores atípicos sin investigar su origen, ya que pueden contener información valiosa.

- Sobrecargar los gráficos: Evite agregar demasiada información en un solo gráfico, lo que puede dificultar su interpretación.

- Saltarse la limpieza de datos: No pase por alto la importancia de limpiar y preparar los datos antes de la exploración.


---

### Librerías de Python para el análisis de datos

- **Pandas**: Librería de Python para manipulación y análisis de datos, que proporciona estructuras de datos flexibles y herramientas para trabajar con datos tabulares.
  
- **NumPy**: Librería de Python para cálculos numéricos, que ofrece soporte para operaciones con arrays de gran tamaño y alta dimensionalidad.

- **Matplotlib**: Librería de Python para la creación de gráficos estáticos, animados e interactivos en 2D.

- **Seaborn**: Librería de Python basada en Matplotlib que proporciona una interfaz de alto nivel para la creación de gráficos estadísticos atractivos y informativos.

- **Plotly**: Librería de Python para la creación de gráficos interactivos que pueden ser utilizados en cuadernos Jupyter o aplicaciones web.

--- 
