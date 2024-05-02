# <img width="40" height="40" src="https://img.icons8.com/external-flatart-icons-flat-flatarticons/40/external-note-pad-user-interface-flatart-icons-flat-flatarticons.png" alt="note pad" /> CLASES  - Anotaciones de las clases

- Cada clase va a tener una **actividad asincrónica** que se puede ir haciendo hasta la próxima clase.

- Nos dividimos en grupo de 8 para hacer el proyecto final que se mostrará. -> **proyecto**: resolver un problema con Inteligencia articifial, se preparan los datos, para que la Inteligencia Artificial sea entrenada y resuelva el problema, llevandolo a producción.

- 12 semanas: divididas en 4 bloques de 3 semanas cada uno
      
---

# <img width="30" height="30" src="https://img.icons8.com/office/30/artificial-intelligence.png" alt="artificial-intelligence"/> CLASE 1 - 4 ETAPAS

1. **PROBLEM SCOPING**: **especificar el problema de negocio**: definir el alcance del problema, para garantizar el éxito, debe saber qué se espera,que beneficio traeré, que restricciones tendremos, etc. Se deberá **contar con expertos en la materia**. **Planear el modelo y método de evaluación**. **Entender viabilidad e impascto**: a veces no es inmediato el impacto, pero deben ser tangibles apra que las personas qeu apuestan en el proyecto vayan veindo y confiando.

2. **RECOLECCIÓN DE DATOS**: **datos como materia prima**: los datos deben ser de calidad, tener buena cantidad, es con lo que vamosa  entrenar a la IA. **Claves para recolectar datos**, en fuentes relevantes, con almacenamiento seguro, de buena calidad en los datos.

### ¿Cómo obtenemos los datos?

- **Datos primarios**: los recolectamos nosotros mismos, con encuestas, observaciones, entrevistas, etc.

- **Datos secundarios**: alguien más los generó, como: informes públicos, investigaciones, bases de datos, imagenes, etc.

 - **Datos internos**: que la organización misma posee: datos de usuarios, clientes, datos de registro de servidores de logueo para detectar anomalía en la red.

- **Datos externos**: que provienen de fuentes externas a la organización, como agencias, otras empresas, redes sociales, un ejemplo es buscar en Twitter todos los # referentes a mi empresa para saber la percepción que hay de la misma.

3. **EVALUAR LA CALIDAD DE LOS DATOS**: unicidad (que no haya duplicaciones de datos), completitud (que no falten datos relevantes en el set de datos), consistencia (coherencia, que no tenga anomalías), oportunidad (que los datos estén disponibles en el momento en que los necesitamos), validez (a que dato consideramos como válidos) y presición (datos representativos a la realidad a resolver).

 4. **DATA AUGMENTATION**: son datos sintéticos, no son reales, son ficticios.
     
---

Del 100% de mis datos, voy a dividir: 70%/80% de los datos para entrenarlo y 30%/20% para evaluar el modelo, si nos da buenos resultados, podremos ponerlo en marcha.

---
---

# <img width="30" height="30" src="https://img.icons8.com/office/30/artificial-intelligence.png" alt="artificial-intelligence"/> CLASE 2

**INTELIGENCIA ARTIFICIAL** rama d ela informática, crear sistema capaces de **Realizar tareas que normalmente requieren inteligencia humana** (x ej: reconocimiento de voz, reconocimiento de patrones, toma de decisiones, etc).

- **IA DÉBIL**: sistemas para tareas específicas / limitadas.

- **IA FUERTE**: 

---

## Aprendizaje vs Memorización

APRENDIZAJE -> Para comprender y generalizar la estructura de los datos. Hay distintos tipos...

... SUPERVIZADO: aprendizaje automático con datos etiquetados (un par entrada / salida)

![image](https://github.com/eugenia1984/IA/assets/72580574/a8f22561-fa92-42b3-aeb7-c6cb6d1bab2d)

Los más comunes: clasificación y regresión (predice un valor numérico basado en un conjunto de características pre definidas, un ejemplo: determinar el valor del alquiler).

![image](https://github.com/eugenia1984/IA/assets/72580574/d01c35e1-ff08-42a3-bca5-c3191a4f9763)

... NO SUPERVISADO: para encontrar patrones ocultos o estructuras intrinsecas en datos no etiquetados.

![image](https://github.com/eugenia1984/IA/assets/72580574/78413c6f-0858-444c-b476-68a5d41fbf85)

Puede ser...

... CLUSTERIZACION: encontrar datos similares procesándolos a todos, x ej: las recomendaciones de Netflix.

... ASOCIACION

... REDUCCION DE DIMENSION

![image](https://github.com/eugenia1984/IA/assets/72580574/3a5052ed-c576-47e6-a054-8eee02cee7dd)

... POR REFUERZO: hay una acción que tomar, que va a ser recompensada o penalizada. Interviene un agente que debe aprender una política de comportamiento, x ej: la aspiradora robot que mapea el lugar y luego esquiva los muebles.


![image](https://github.com/eugenia1984/IA/assets/72580574/fa5b504d-11ba-427a-878a-c5eb9ce8c1c2)

MEMORIZACION -> adquieren conocimiento mediante información en la memoria, producen un resultado esperado, no parten desde una experiencia como el humano; si le damos un dato distinto al de su memoria no sabrá como responder (se lo llama sobre ajuste).

---

## DATOS Y ENTRENAMIENTO

- Hay 2 tipos de datos:

- **ESTRUCTURADOS**
 
- **NO ESTRUCTURADOS**: como audio, imagen, textos. Se usan en computer vision, x ej.

Los DATOS son la MATERIA PRIMA, hay que pasar por ciertos pasos, para que los datos sea ASCERTIVOS, tengan CIERTA CALIDAD. Los pasos:

- RECOLECTAR: datos representativos

- EXPLORAR: entender la naturaleza, estructura de los datos. Estadística descriptiva (que info contienen los datos? mediana, desviación estandar, media, etc). Relaciones entre variables.

- VISUALIZAR: representar los datos, para comprender mejor los datos, con histogramas, gráficos de calor, etc.

- CARACTERIZAR: valores atípicos, valores faltantes, normalización.

- SESGOS
  
---

## ENTRENAMIENTO DEL MODELO & EVALUACIÓN

70-80% datos y 20-30% evaluación

---

## REDES NEURONALES

En base al comportamiento y el funcionamiento del cerebro humano, ver la eestructura, se modela en un sistema, y se trata de obtener le mismo resultado que se obtendría de una red neuronal.

![image](https://github.com/eugenia1984/IA/assets/72580574/830e986d-7e65-4a71-9f7f-129189d8ee69)

Neuronas artificiales -> por donde entra, están todas conectadas y combinadas.

![image](https://github.com/eugenia1984/IA/assets/72580574/66a996ec-3022-4bcb-b489-3cd3779b53fc)

## DEEP LEARNING

Redes neuronales con multiples capaz

![image](https://github.com/eugenia1984/IA/assets/72580574/646eba63-8a4a-47d3-9d7e-3f882cf8fe7f)

## COMPUTER VISION

![image](https://github.com/eugenia1984/IA/assets/72580574/f3313367-ee3f-4aec-88d6-14281adb7213)

## PROCESAMIENTO DEL LENGUAJE NATURAL

Es la interfaz entre la computadora y la gente

---

## SISTEMAS DE RECOMENDACION

![image](https://github.com/eugenia1984/IA/assets/72580574/ccb71ff8-3c5a-4ca5-a39d-df375099732f)


---

## ÉTICA

- Equidad y sesgo

- Privacidad y seguridad de datos
 
- Transparencia y explicabilidad

- Impacto en empleo

- Autonomía y responsabilidad

- Seguridad y riesgo   

---

## DESARROLLO SUSTENTABLE

- Eficiencia energética

- Aplicaciones para la sostenibilidad ambiental

- Ciudades inteligentes

- Salud y Bienestar  

---

## PROGRAMANDO IA

![image](https://github.com/eugenia1984/IA/assets/72580574/873083af-753c-4939-a0d9-8d4e4dbf3ca1)

---

[Google Colab](https://colab.research.google.com/drive/1S4yY8x5joLhv9maaTuf7icLnbos0p9YE?usp=sharing)

---
---

# <img width="30" height="30" src="https://img.icons8.com/office/30/artificial-intelligence.png" alt="artificial-intelligence"/> CLASE 3

## ESTADÍSTICA DESCRIPTIVA


![image](https://github.com/eugenia1984/IA/assets/72580574/e42ddccd-1126-42f0-8335-b30f61c13f16)

- MEDIA: es el promedio

- MEDIANA: es el valor que se encuentra en el medio, teniendo los datos ordenaods

- MODA: los valores ue aparecen con mayor frecuencia

### Varianza, desvío estándar y rango intercuartílico
 
![image](https://github.com/eugenia1984/IA/assets/72580574/c73b3f7a-e816-44ed-93ad-d8cbae8b7ac2)

- **rango intercuartílico**: se ordenen los datos de menor a mayor, se divide en 4 partes, va a ser el segmento que ocupe el 50% de los datos, dejando un 25% por delante y por detrás

## VISUALIZACIÓN DE DATOS 

- **gráfico hitograma**
  
![image](https://github.com/eugenia1984/IA/assets/72580574/f1feda17-5e8b-45b3-9bfa-84b05b54bb3b)

- **gráficos de barra**: cada barra es una categoría, y la altura la cantidad

  ![image](https://github.com/eugenia1984/IA/assets/72580574/57ed8e66-132c-4de5-82d8-74742533cc64)

- **diagramas de caja / boxplot**: para comparar distribuciones entre difernetes grupos

 ![image](https://github.com/eugenia1984/IA/assets/72580574/9d6709a0-75f5-40f5-946e-5d2814d6b85b)

## EDA: Analisis exploratorio de datos

1. conocer los datos

2. limpiar los datos
  
3. gráficos adecuados a usar

4. análisis iterativo: para garantizar la calidad de los datos 

5. documentar: lo que vamos encontrando, las decisiones tomadas, etc.
    
---
---

# <img width="30" height="30" src="https://img.icons8.com/office/30/artificial-intelligence.png" alt="artificial-intelligence"/>  CLASE 4

### Aprendizaje Supervisado Clasificaicón

Para asignar categorías discretas a las observaciones basánose en sus caracterísitcas

![image](https://github.com/eugenia1984/IA/assets/72580574/f521bd4d-b2e6-4a84-9ed8-0a3bc211fc5e)

### Métricas de evaluación - clasificación

![image](https://github.com/eugenia1984/IA/assets/72580574/6128319a-f2db-4e1c-874a-849a2f8d115f)


**ROC**: Receiver Operating Characteristic -> es la curva

**AUC** -> el área debajo de la curva

![image](https://github.com/eugenia1984/IA/assets/72580574/541a7a00-c900-43fb-96a2-4eab1c30db22)

### Cross Validation


![image](https://github.com/eugenia1984/IA/assets/72580574/c3cacad3-6515-479f-8e4c-352aef050a5e)

---
---

# <img width="30" height="30" src="https://img.icons8.com/office/30/artificial-intelligence.png" alt="artificial-intelligence"/>  CLASE 5
