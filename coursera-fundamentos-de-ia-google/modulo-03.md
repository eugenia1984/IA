# Módulo 3: Descubre el arte de la ingeniería de instrucciones

## Introducción al Módulo 3: Descubre el arte de la ingeniería de instrucciones

La ingeniería de instrucciones implica diseñar la mejor instrucción que puedas para obtener el resultado deseado

Piensa en cómo utilizas el lenguaje en tu vida diaria. El lenguaje se utiliza con muchos fines: para establecer conexiones, expresar opiniones o explicar ideas. Y, a veces, es posible que desees utilizar el lenguaje para pedir a otros que respondan de una manera determinada. Tal vez quieras que alguien te dé una recomendación o aclare algo. En esos casos, l**a forma en que expresas tus palabras puede afectar a la respuesta de los demás**. Lo mismo ocurre al dar instrucciones a una herramienta de IA conversacional con una pregunta o solicitud. 

Una instrucción (**PROMPT**) es **una entrada de texto que proporciona indicaciones al modelo de IA sobre cómo generar resultados**. 

Por ejemplo, alguien que posee una tienda de ropa podría querer que un modelo de IA le proporcione nuevas ideas sobre cómo comercializar sus prendas. Este empresario podría escribir la instrucción: “Tengo una tienda de ropa. Vendemos ropa de mujer de alta costura. Ayúdame con ideas de marketing". 

En esta sección del curso, te centrarás en cómo diseñar o desarrollar instrucciones eficaces para obtener resultados más útiles de una herramienta de IA conversacional. 

Me llamo Yufeng y soy ingeniero en Google. Primero, me interesé en la elaboración de instrucciones porque obtener respuestas de los modelos grandes requería mucho tiempo. A veces incluso nos resultaba más rápido hacer el trabajo sin recurrir a la IA. Eso me inspiré a ayudar a nuestras herramientas ser más eficientes, no menos eficientes. Estoy deseando ayudarte a aprender más sobre la **elaboración de instrucciones eficaces.** 

En primer lugar, descubrirás cómo generan resultados los LLM en respuesta a instrucciones. Y

luego, explorarás el papel de la ingeniería de instrucciones en la mejora de la calidad de los resultados. **La ingeniería de instrucciones es la práctica de desarrollar instrucciones eficaces que generen resultados útiles a partir de la IA generativa**. Aprenderás a crear instrucciones claras y específicas, una de las partes más importantes de la ingeniería de instrucciones. **Cuanto más clara y específica sea tu instrucción, más probabilidades tendrás de obtener resultados útiles**. 

Otra parte importante de la ingeniería de instrucciones es la **iteración**. Aprenderás a **evaluar los resultados y revisar tus instrucciones**. Esto también te ayudará a obtener los resultados que necesitas cuando utilizas herramientas conversacionales de IA en el lugar de trabajo. 

También exploraremos una técnica específica que utiliza **“algunos ejemplos de instrucciones”**. Redactar instrucciones eficaces implica pensamiento crítico y creatividad. También puede ser un proceso divertido, y es una habilidad muy importante que se debe practicar si quieres utilizar la IA eficazmente en el trabajo. 

¿Ansías empezar a trabajar en ingeniería de instrucciones? 

¡Vamos!

---

# Los modelos de lenguaje de grande y sus resultados

## Comprende los modelos de lenguaje grande

Es útil entender cómo funcionan los LLM y ser conscientes de sus limitaciones. 

**Un modelo de lenguaje grande**, o **LLM**, **es un modelo de IA entrenado con grandes cantidades de texto para identificar patrones entre palabras, conceptos y frases, de modo que pueda generar respuestas a las instrucciones**. 

¿Cómo los LLM aprenden a generar respuestas útiles a las instrucciones? Un LLM se entrena con millones de fuentes de texto, incluidos libros, artículos, sitios web y mucho más. Este entrenamiento ayuda al modelo a **aprender los patrones y las relaciones que existen en el lenguaje humano**. En general, **cuantos más datos de alta calidad reciba el modelo, mejor será su rendimiento**. Dado que los LLM pueden identificar muchos patrones en el lenguaje, **también pueden predecir qué palabra es más probable que venga a continuación en una secuencia de palabras**. Veamos un ejemplo sencillo para obtener una comprensión básica de cómo los LLM predicen la siguiente palabra de una secuencia. Toma la frase incompleta, “Después de llover, la calle estaba...”. Un LLM puede predecir qué palabra viene a continuación calculando las probabilidades para diferentes palabras posibles. Según los datos disponibles, la palabra mojado podría tener una alta probabilidad de ser la siguiente palabra. La palabra limpia sería una probabilidad menor. Y la palabra seca, una probabilidad extremadamente baja. En este caso, el LLM podría completar la frase insertando la palabra con mayor probabilidad de venir a continuación en la secuencia, mojado. O podría ser otra palabra altamente probable como humedad. Un LLM puede variar en su respuesta a la misma instrucción cada vez que lo utilizas.

**Los LLM utilizan la estadística para analizar las relaciones entre todas las palabras de una secuencia dada y calcular las probabilidades de miles de posibles palabras siguientes en esa secuencia**. Este **poder predictivo** permite a los LLM responder a las preguntas y peticiones, tanto si la instrucción es completar una frase sencilla o desarrollar una historia convincente para el lanzamiento de un nuevo producto o una campaña publicitaria. **Aunque los LLM son potentes, puede que no siempre obtengas el resultado deseado. A veces se debe a limitaciones en los datos de entrenamiento de un LLM**. Por ejemplo, el resultado de un LLM puede estar sesgado porque **los datos de entrenamiento contienen sesgos**. Estos datos pueden incluir artículos de prensa y sitios web que reflejen los prejuicios injustos presentes en la sociedad. Por ejemplo, debido a los datos con los que se ha entrenado, un LLM puede ser más probable que produzca resultados asociados una ocupación profesional con un papel específico de género. Los datos de entrenamiento de un LLM también pueden limitarse de otras formas. Por ejemplo, un LLM podría no generar contenido suficiente sobre un ámbito o tema específico porque los datos con los que se entrenó no contienen suficiente información sobre ese tema. Otro factor que puede afectar al resultado es la tendencia de los LLM a alucinar.

**Las alucinaciones son resultados que arroja la IA y que no son ciertos**. Aunque los LLM son buenos respondiendo a muchos tipos de preguntas e instrucciones, **pueden a veces generar texto que es objetivamente inexacto**. Digamos que estás investigando una empresa y utilizas un LLM para ayudarte a resumir la historia de la empresa. El LLM podría alucinar y proporcionar información incorrecta sobre determinados detalles como la fecha de fundación de la empresa o el número actual de empleados. Varios factores pueden contribuir a las alucinaciones, como la calidad de los datos de entrenamiento de un LLM, la formulación de la instrucción o el método que utiliza un LLM para analizar textos y predecir la siguiente palabra de una secuencia. Debido a las limitaciones de un LLM, es importante que evalúes de forma crítica todos los resultados del LLM para determinar si es objetivamente preciso, es imparcial, pertinente para tu solicitud concreta y proporciona información suficiente. Tanto si utilizas la IA para resumir un informe extenso, generar ideas para comercializar un producto o esbozar un plan de proyecto, **asegúrate de comprobar cuidadosamente la calidad del resultado**. 

Por último, es importante no hacer suposiciones sobre las capacidades de un LLM. Por ejemplo, solo porque producía resultados de alta calidad para una carta persuasiva a un cliente, no des por sentado que obtendrás la misma calidad del resultado si utilizas la misma instrucción de nuevo en el futuro. **Los modelos de lenguaje grandes son herramientas poderosas que requieren orientación humana para un uso eficaz. Ser consciente de las limitaciones de una LLM puede ayudarte a conseguir los mejores resultados posibles.**


## Yufeng: Experimenta con la ingeniería de instrucciones

Hola, soy Yufeng y soy **ingeniero de Relaciones con Desarrolladores en Google Cloud.** Soy solo una pequeña parte de un equipo mucho más grande que se centra en **crear instrucciones útiles para la evaluación y, hasta cierto punto, el entrenamiento de los modelos**. Crecí en el centro de Pensilvania, en Hershey, la ciudad del chocolate. Y disfruté de las matemáticas y ciencias en la secundaria. Luego, fui a la universidad en Johns Hopkins y estudié ingeniería biomédica. Cuando me gradué, la empresa para la que trabajaba tenía un programa de entrenamiento muy amplio y estaban buscando específicamente contratar a estudiantes no informáticos. Y no era como los programas de formación normales en el lugar de trabajo que pensamos hoy. Fue como un curso intensivo y supercomprimido. Hoy en día, lo llamaríamos bootcamp o algo así, pero eso no existía entonces. 

**La ingeniería de instrucciones no es algo que necesariamente se producirá a través del uso intuitivo**. Hacer las instrucciones como se debe realmente va a ayudar a desbloquear las capacidades de estos sistemas de IA conversacionales para ti. 

Cualquiera puede escribir una instrucción simple y obtener una respuesta sencilla. Pero eso no es lo verdaderamente interesante, ¿verdad? **Cuando puedes hablar con un sistema y obtener una respuesta adaptada y personalizada basada exactamente en tu caso de uso, ahí las cosas se vuelven realmente emocionantes**. Mi consejo para la gente que está experimentando con estas herramientas de IA por primera vez sería no desanimarse si no produce los resultados deseados inicialmente. Estas herramientas no son mágicas y no pueden leer tu mente. Todo lo que pueden hacer es tomar exactamente lo que les dices e intentar hacerlo lo mejor que pueden. Hay una especie de lo que yo llamo contexto secundario o contexto implícito que necesitas practicar sacándolo de tu cabeza. Quieres que sea largo, quieres que sea corto. Quieres que use palabras simples, palabras elegantes, como este tipo de cosas que ya sabes, pero quizá no sepas que que tienes que escribirlas. Te animo a que pruebes diferentes cosas. Puedes enloquecerte con la experimentación. Prueba cosas. Puedes escribir mucha información o simplemente escribir poco, luego escribe un poco luego escribe un poco, y nota cómo se comporta de manera diferente. Se convierte simplemente en este sistema experimental, y este proceso es divertido. A medida que experimentes y pruebes cosas nuevas, descubrirás que tu fluidez y soltura con estas herramientas de IA conversacional estarán por las nubes y querrás seguir probando diferentes instrucciones. 

¿Y quién sabe? Quizá tenga un gran impacto en tu vida. Solo el tiempo lo dirá.

---
---

# Principios clave para escribir instrucciones eficaces

## Escribe instrucciones claras y específicas

¿Cómo puedes escribir instrucciones que arrojen resultados útiles? En general, es cierto que la calidad de lo que se empieza afecta en gran medida a la calidad de lo que produce. Pensemos, por ejemplo, en la cocina. Digamos que estás preparando la cena. Si tienes ingredientes frescos de alta calidad, bueno, es más probable que prepares una gran comida. Por el contrario, si falta un ingrediente o los ingredientes no son de alta calidad, la comida resultante puede no ser tan buena. Del mismo modo, **la calidad de la instrucción que se pone en una herramienta de IA conversacional puede afectar la calidad de los resultados de la herramienta**.

Aquí es donde entra en juego la **ingeniería de instrucciones**. La ingeniería de instrucciones **implica diseñar la mejor instrucción que puedas para obtener el resultado deseado de un LLM.** Esto incluye **escribir instrucciones claras y específicas que proporcionen un contexto relevante**.

Para comprender mejor del contexto que necesitan los LLM, comparemos cómo una persona y un LLM podrían responder a la misma pregunta. Supongamos que un vegetariano pregunta a su amigo a qué restaurante ir en San Francisco. El amigo probablemente sugeriría restaurantes con buenas opciones vegetarianas. Sin embargo, si se le pide eso mismo a un LLM, podría recomendar restaurantes que no son adecuados para un vegetariano. Una persona instintivamente consideraría el hecho de que su amigo es vegetariano al responder a la pregunta, pero un LLM no tiene este conocimiento previo. Entonces, **para obtener la información necesaria de un LLM, la instrucción debe ser más específica**. En este caso, la instrucción debe mencionar que el restaurante debería tener buenas opciones vegetarianas. Veamos un ejemplo que demuestra cómo utilizar la ingeniería de instrucciones para mejorar la calidad del resultado de un LLM. Encarguémonos de la tarea de planificar un evento de empresa. Necesitas encontrar un tema para una próxima conferencia. Escribamos una instrucción en Gemini para generar una lista de cinco posibles temas para un evento. Puedes utilizar instrucciones similares en ChatGPT, Microsoft Copilot o cualquier otra herramienta de IA conversacional.

Ahora repasemos la respuesta. Bueno, esto no es lo que queríamos. Hemos conseguido una lista que parece estar más relacionada con temas de fiestas que con temas para una conferencia profesional. Nuestra instrucción no proporcionaba suficiente contexto para producir el resultado que necesitábamos. No era lo suficientemente clara ni específica. 

Intentémoslo de nuevo. Esta vez escribiremos la instrucción, **generar una lista de cinco temas potenciales para una conferencia profesional sobre la experiencia del cliente en el sector de la hostelería**. Esta instrucción es mucho más específica y deja claro que es una conferencia profesional sobre la experiencia del cliente en el sector de la hostelería. Examinemos la respuesta. ¡Esto es mucho mejor! **Hemos diseñado nuestra instrucción para incluir contexto específico y pertinente, por lo que Gemini puede generar resultados útiles**. 

-> **Cuando proporcionas instrucciones claras y específicas que incluyen el contexto, permites que los LLM generar resultados útiles**. 

Ten en cuenta que debido a las limitaciones del LLM, puede haber algunos casos en los que no se pueda obtener un resultado de calidad independientemente de la calidad de tu instrucción. Por ejemplo, si le pides al LLM que busque información sobre un acontecimiento de actualidad, pero el LLM no tiene acceso a esa información, no será capaz de proporcionar el resultado que necesitas. 

Y como en otras áreas del diseño, **la ingeniería de instrucciones suele ser un proceso iterativo**. A veces, incluso cuando se proporcionan instrucciones claras y específicas, puede que no obtengas el resultado en el primer intento. Cuando nuestra primera instrucción no produjo la respuesta que queríamos, revisamos la instrucción para mejorar el resultado. La segunda iteración proporcionó instrucciones lo suficientemente claras y específicas para producir un resultado más útil.

## Aprovecha el potencial de un LLM en el trabajo

Existen varias formas de aprovechar las capacidades de un LLM que funcionan para impulsar la productividad y la creatividad. Una de las más comunes es la **creación de contenido.** Puedes utilizar un LLM para crear correos electrónicos, planes, ideas y mucho más. Por ejemplo, podrías pedir a un LLM que te ayude a redactar un artículo sobre un tema relacionado con el trabajo. Vamos a pedirle a Gemini que cree un esquema para un artículo sobre las prácticas recomendadas de visualización de datos. El artículo está dirigido a analistas empresariales principiantes. Fíjate que la instrucción comienza con el verbo crear. A menudo es útil incluir un verbo en la instrucción que guíe al LLM para que produzca resultados útiles para la tarea prevista.

El resultado ofrece un esquema útil para un primer borrador del artículo.

También puedes utilizar un LLM para resumir. Un LLM puede resumir los puntos principales de un documento extenso. Por ejemplo, puedes pedir a Gemini que resuma un párrafo detallado sobre estrategias de gestión de proyectos. Comenzaremos la instrucción con el verbo resumir y especificaremos que queremos que el resultado sea una sola oración.

Luego incluiremos el párrafo que queremos que Gemini resuma.

El resultado proporciona un resumen práctico de una oración del párrafo. Aunque este ejemplo muestra cómo se puede resumir un solo párrafo, puedes pedirle a un LLM que resuma también textos y documentos más largos. La clasificación es otro uso posible. Por ejemplo, puedes pedirle al LLM que clasifique el sentimiento o la sensación de reseñas de clientes como positivas, negativas o neutras. Pidamos a Gemini que clasifique las reseñas de los clientes sobre el nuevo diseño de un sitio web como positivas, negativas o neutras. La instrucción incluye el verbo clasificar para guiar el resultado. La instrucción también contiene las reseñas. En este ejemplo, hay cuatro reseñas. El resultado clasifica correctamente las dos primeras reseñas como negativas, la tercera como positiva y la cuarta como neutral. Considera cómo podrías aprovechar un LLM para completar con eficacia grandes tareas de clasificación.

O puedes utilizar un LLM para la extracción, que consiste en extraer datos de texto y transformarlos en un formato estructurado más fácil de entender. Digamos que tienes un informe que proporciona información sobre una organización mundial. Puedes pedir a Gemini que extraiga todas las menciones de ciudades e ingresos en el informe y los coloque en una tabla. Luego incluiremos el informe en nuestra instrucción. Ten en cuenta que no debes introducir información confidencial en los LLM. Pero en este ejemplo, el informe no es confidencial. El resultado muestra una tabla con columnas para la ciudad y los ingresos. Esto presenta la información en un formato bien organizado que es fácil de revisar. Otro uso es la traducción. Puedes aprovechar un LLM para traducir textos de un idioma a otro. Por ejemplo, puedes pedir a Gemini que traduzca el título de una sesión de entrenamiento del inglés al español. El resultado incluye una variedad de traducciones al español para elegir y explica el razonamiento de cada traducción. Esta información puede ayudarte a elegir la opción más útil para tu audiencia. También puedes hacer ediciones con un LLM, por ejemplo para cambiar el tono de una sección de texto de formal a informal y comprobar si el texto es gramaticalmente correcto. Por ejemplo, Gemini puede ayudarle a a editar un análisis técnico sobre vehículos eléctricos haciendo que el lenguaje sea más accesible para un público no especializado. Empezaremos la instrucción con el verbo editar y especificaremos que el lenguaje debe ser fácil para que lo entienda un público no especializado. Después de esto, incluiremos el análisis técnico.

El resultado proporciona una versión del análisis que un público menos familiarizado con los detalles técnicos puede entender. Éste es sólo un ejemplo de cómo un LLM puede ayudarte a editar documentos. Los LLM pueden personalizar rápidamente el tono, la longitud, y el formato de los documentos para adaptarlos a tus necesidades.

Otro de los usos del LLM que abordaremos es la resolución de problemas. Puedes utilizar un LLM para generar soluciones para diversos retos en el lugar de trabajo. Al planificar un evento empresarial, por ejemplo, podrías pedirle al LLM que encuentre soluciones de menú que se adapten a las restricciones alimentarias de varios invitados siguiendo un menú de temática festiva. Y he aquí otro ejemplo. Supongamos que eres empresario y que acabas de lanzar un nuevo servicio de corrección de textos. Pidamos a Gemini que resuelva un problema relacionado con el servicio de corrección de textos. Pediremos sugerencias para aumentar la base de clientes. El resultado ofrece sugerencias concretas para llegar a nuevos clientes, optimizar los servicios y hacer crecer el negocio. Me encantan estas ideas. Pidamos a Gemini que redacte un correo electrónico para que podamos compartir fácilmente estas ideas con los demás.

Los LLM pueden ayudarte a encontrar soluciones para muchos tipos diferentes de problemas. Estoy entusiasmado por la variedad de formas en que podemos aprovechar los LLM para realizar tareas laborales. Es una habilidad muy importante para practicar si quieres utilizar la IA eficazmente en el trabajo. Próximamente, nos centraremos más en evaluar los resultados y hacer iteraciones de tu instrucción.


## :book: Instrucciones para diferentes propósitos

Recordemos que un **modelo de lenguaje grande** o **LLM **es u**n modelo de IA que se entrena a partir de grandes cantidades de texto para identificar patrones en palabras, conceptos y frases con el fin de poder generar respuestas a las instrucciones**. Como estuviste aprendiendo, una buena ingeniería de instrucciones sirve para guiar a un LLM para que genere resultados útiles para las tareas de trabajo. En esta lectura, analizarás cómo escribir instrucciones claras y específicas en mayor profundidad para diversos casos de uso en el trabajo. 

### Casos de uso
Como has explorado anteriormente, puedes utilizar un LLM en el trabajo para ayudar a aumentar tu productividad y creatividad y completar cualquiera de estas útiles tareas: 

```
-Crear contenido
-Resumir 
-Clasificar
-Extraer
-Traducir 
-Editar 
-Resolver problemas
```

**Nota:** Los siguientes ejemplos ilustran mejores prácticas. No son plantillas exactas que deban copiarse en cada situación. Tus resultados variarán en función de una serie de factores, incluido el LLM específico que utilices. No olvides hacer una evaluación crítica de todos los resultados del LLM y hacer iteraciones de tu instrucción inicial para obtener el mejor resultado. 


En general, las siguientes pautas sirven para que tus instrucciones sean más eficaces: 

- **Piensa en lo que quieres que genere el LLM.** El LLM arrojará mejores resultados si incluyes una indicación específica en la instrucción, como crea, resume, clasifica, extrae, traduce, edita o resuelve.

- **Proporciona el contexto necesario**. El LLM generará mejores resultados si incluyes indicaciones detalladas, con pautas específicas sobre el estilo o formato del resultado que deseas. 

A continuación, examinaremos cada uno de los casos de uso descritos anteriormente mediante un ejemplo adicional de cada uno. 

![image](https://github.com/eugenia1984/IA/assets/72580574/8e05cc2c-2a62-4392-b99c-59dd160ac685)


- **Crear contenido**: Sea cual sea tu sector, un LLM puede ayudarte a crear contenido para diversos fines, como publicaciones de blog, informes, descripciones de productos y lemas. Por ejemplo, supongamos que trabajas en una campaña publicitaria para una nueva línea de electrodomésticos. Puedes pedir a un LLM que te ayude a crear un eslogan atractivo para uno de los productos: 

Haz de cuenta que eres un profesional creativo del ámbito publicitario que aplica razonamiento innovador para elaborar eslóganes originales que proyecten las cualidades positivas de un producto. Crea un eslogan conciso para una lavadora que deja la ropa impecable, tiene 25 configuraciones y cabe en un espacio pequeño.

La instrucción empieza describiendo el papel del LLM como creativo publicitario. Luego, señala claramente que la tarea consiste en crear un eslogan conciso para una lavadora. Por último, especifica las características del producto que se deben incluir en el eslogan.

Sugerencia profesional: Asigna un papel, un trabajo o una función al LLM para reforzar el propósito de la instrucción y guiar al LLM para que arroje resultados útiles. 


- **Resumir**: Un LLM puede ayudarte a resumir muchos tipos de textos: informes, encuestas a clientes, notas de reuniones, correos electrónicos, etc. Por ejemplo, la siguiente instrucción solicita a un LLM que resuma un correo electrónico extenso: 

El siguiente texto es un correo electrónico de un proveedor de software. Resume los puntos principales en una lista con viñetas:

“Espero que todo esté bien. Fue un placer que hayamos tenido la oportunidad de conversar en la conferencia de la semana pasada.

Estoy enviando más detalles sobre los precios de nuestros planes. Nuestra suscripción de nivel bronce brinda acceso a tres de nuestros productos de software más populares, así como a tutoriales en video de esos productos. En caso de requerir asistencia para necesidades de software adicionales, nuestro nivel plata puede ser una opción. Ese nivel permite elegir dos productos de software adicionales, con tutoriales en videos, y recibir asistencia las 24 horas del día para resolver cualquier dificultad que ocurra al utilizar los productos. Por último, la membresía de oro brinda acceso a nuestros diez productos de software. Recibirás capacitaciones para utilizar los diez productos, así como asistencia las 24 horas del día, y también serás la primera persona en disfrutar de cualquier incorporación beta a nuestros productos.

Ponte en contacto conmigo para conocer el precio del nivel que te interese. Ofrecemos suscripciones mensuales y una tarifa reducida para una suscripción anual”.

La instrucción comienza con contexto útil sobre el correo electrónico en cuestión. Luego, señala claramente que la tarea consiste en resumir los puntos principales del correo electrónico. Por último, especifica que el resultado debe tener el formato de una lista con viñetas. 

Nota: Ten en cuenta que, en ciertas ocasiones, los LLM generan alucinaciones, es decir, arrojan resultados de IA que no son ciertos. En este caso, el LLM podría añadir detalles al resumen que no están incluidos en el correo electrónico de partida. Siempre evalúa la precisión de los resultados de los LLM antes de utilizarlos. 

- **Clasificar**: La clasificación de textos es otra aplicación de trabajo frecuente de los LLM. Un LLM puede ayudarte a clasificar los correos electrónicos de atención al cliente en categorías según el contenido del correo electrónico, catalogar el contenido de publicaciones de redes sociales y analizar el tono de los comentarios de clientes. La siguiente instrucción pide a un LLM que analice el tono de reseñas de clientes: 

Lee estas reseñas de clientes y dime si el tono es positivo, negativo o neutral.

Reseña del cliente: No sé por dónde empezar. Teníamos una reserva para las 7:00, pero nos ubicaron a las 7:45. Luego, nadie vino a nuestra mesa por al menos 30 minutos. El aperitivo y plato principal fueron mediocres. Me encantó el postre, pero eso no alcanzó para cambiar nuestra experiencia.

Reseña del cliente: Me encanta este restaurante. La comida es deliciosa y el servicio es excelente.

La instrucción comienza señalando claramente que la tarea consiste en analizar el tono de reseñas de clientes y, luego, especifica las opciones: positivo, negativo o neutral. Por último, la instrucción incluye las reseñas pertinentes con la etiqueta “Reseña del cliente”.

- **Extraer**: También puedes utilizar un LLM para extraer información de un texto y aplicarle un formato estructurado más fácil de entender, lo que se conoce como extracción. Por ejemplo, esta instrucción pide a un LLM que revise una publicación de blog y extraiga información sobre los productos mencionados en la publicación en cuestión. 

Lee la siguiente publicación de blog y extrae todas las referencias a prendas de ropa que puedo comprar y el precio de cada una. Elabora una lista con viñetas solo con esos datos. 

Publicación de blog: Hola a todos, quiero compartir lo que estoy usando en el campus este otoño. Si voy a salir por la noche, prefiero el jean de orillo crudo (USD 150) combinado con el jersey de cuello redondo de cachemira (USD 250). Para un look más informal, me gusta la sudadera de polar con capucha (USD 99) y los pantalones deportivos de polar (USD 129). También me encantan todos los colores de los calcetines de rayas (USD 15). Combinan bien tanto con el jean como con la ropa deportiva. 

La instrucción comienza señalando claramente que la tarea consiste en extraer todas las prendas de ropa mencionadas en el blog con sus respectivos precios. Luego, especifica que el formato del resultado debe ser una lista con viñetas de los elementos. Por último, la instrucción incluye la publicación de blog correspondiente. 

- **Traducir**: Puedes aprovechar un LLM para traducir textos de uno a otro idioma con gran rapidez. Por ejemplo, la siguiente instrucciones le pide a un LLM que ayude a traducir la descripción de un producto del inglés al español: 

Traduce las descripciones de nuestros productos del inglés al español. Conserva en la traducción al español la misma estructura y el mismo tono informal de la versión en inglés.

Bicicleta: Tanto si recorres las calles de la ciudad como los senderos del bosque, nuestra elegante y duradera bicicleta lo tiene todo. 

Patines: Deslízate hacia el verano con estilo gracias a nuestros bacanes y elegantes patines.

La instrucción comienza señalando claramente que la tarea consiste en traducir descripciones de productos del inglés al español. También especifica que las traducciones al español deben mantener una estructura y un tono similares a los del original en inglés. Por último, cada ejemplo contiene una etiqueta que introduce la descripción del producto: “Bicicleta” y “Patines”. Ese formato indica que el LLM debe presentar el resultado de forma similar. 

Nota: Como práctica recomendada, verifica que las traducciones de un LLM sean precisas comparándolas con otra herramienta de traducción. 

- **Editar**: También puedes utilizar un LLM para editar y reescribir texto. El LLM es capaz de modificar el tono del texto de formal a informal, o realizar una revisión gramatical. Por ejemplo, en la siguiente instrucción, se le pide a un LLM que edite un informe técnico para que tenga menos jerga y sea más fácil de entender para las partes interesadas: 

Edita el vocabulario del siguiente párrafo para que sea fácil de entender para un público general. Usa un lenguaje y estructuras sintácticas más simples, pero conserva las mismas ideas.

La elección de emplazamientos para la ampliación es un proceso complejo y polifacético. El emplazamiento del lado oeste ofrece varias ventajas, como la zonificación para uso industrial y acceso directo a una autopista principal y el ferrocarril. Sin embargo, el emplazamiento también está situado en una jurisdicción donde el proceso de obtención de permisos es complejo y lento, y como es remoto con respecto a las zonas residenciales, quizás se requieran salarios más altos para atraer trabajadores.

La instrucción comienza señalando claramente que la tarea consiste en editar el texto para facilitar su comprensión para un público general. Luego, especifica que el vocabulario y la sintaxis del texto deben simplificarse, mientras que su contenido principal debe seguir siendo el mismo. Por último, incluye el párrafo en cuestión. 

- **Resolver problemas**: Otro caso de uso es la resolución de problemas. Puedes utilizar un LLM para elaborar soluciones a diversos retos laborales, desde analizar datos de ventas hasta planificar un evento. Por ejemplo, en la siguiente instrucción, se le pide a un LLM que ayude a organizar un programa para una organización sin fines de lucro: 

Vamos a ofrecer un programa para la comunidad donde se enseñan destrezas de jardinería a los niños. El programa dura del 1 de junio al 15 de agosto. Queremos que los niños sean capaces de cultivar plantas que estén listas para la cosecha cuando termine el programa. En primer lugar, elabora una lista de 10 plantas que puedan plantarse y cultivarse en ese periodo de tiempo. Incluye fuentes que confirmen el momento de cosechar cada planta.

Queremos que los niños cultiven tres plantas. Esas plantas deben ser tan diferentes entre sí como sea posible. Luego, selecciona tres plantas de la lista que proporcionen a los niños esa variedad.

La instrucción comienza brindando un contexto útil sobre el programa, como su objetivo principal y su cronograma. Luego, desglosa el problema en dos pasos principales: en primer lugar, elaborar una lista de 10 plantas que se ajusten al cronograma y, en segundo lugar, elegir tres plantas de la lista que sean diferentes entre sí. La instrucción también pide al LLM que incluya las fuentes de la lista de 10 plantas. Pedir al LLM que cite sus fuentes en el resultado te ayuda a verificar la precisión de la información utilizada para resolver el problema. 

Sugerencia profesional: divide un problema en varios pasos para ayudar al LLM a procesar la solicitud y mejorar la precisión general del resultado.

## :tv: Mejora los resultados de la IA mediante la iteración


¿Alguna vez creaste una presentación para un cliente o diseñaste un sitio web para tu nueva empresa? Si es así, es posible que hayas utilizado un **proceso iterativo para lograr tu objetivo**. En un proceso iterativo, **creas una primera versión, la evalúas y la mejoras para la próxima versión**. Luego, **repites estos pasos hasta obtener el resultado deseado.** 

Por ejemplo, si estás desarrollando una propuesta, un informe u otro documento para compartir con tus compañeros de trabajo, es posible que elabores varios borradores y realices mejoras en cada borrador hasta que te satisfaga el resultado. Adoptar un enfoque iterativo suele ser la forma más eficaz para resolver un problema o desarrollar un producto. Un proceso iterativo también es eficaz en la ingeniería de instrucciones. La ingeniería de instrucciones a menudo requiere múltiples intentos antes de obtener el resultado óptimo. La mayoría de las veces, no obtendrás el mejor resultado en el primer intento. Si intentas algo y no funciona, no te desanimes. En su lugar, evalúa cuidadosamente el resultado para determinar por qué no obtuviste la respuesta deseada. A continuación, revisa tu instrucción para intentar obtener un mejor resultado. Consideremos las posibles razones por las que puede que no obtengas resultados útiles después de crear una instrucción clara y específica. En primer lugar, las diferencias en modelos de lenguaje grande pueden afectar el resultado. Cada LLM se desarrolla con datos de entrenamiento únicos y técnicas de programación, y tiene diferentes conocimientos previos sobre ámbitos específicos. Por esta razón, diferentes modelos pueden responder a instrucciones similares de diferentes maneras. Y podría fracasar en dar una respuesta adecuada a algunas instrucciones. Adoptar un enfoque iterativo con el LLM que estás utilizando producirá los mejores resultados. En segundo lugar, las limitaciones del LLM. Anteriormente, aprendiste que los resultados del LLM a veces pueden ser inexactos, sesgados, insuficientes, irrelevantes o incoherentes. Deberás evaluar de forma crítica todos los resultados del LLM planteándote las siguientes preguntas. 

- ¿El resultado es preciso? 

- ¿El resultado es imparcial? 

- ¿El resultado incluye suficiente información? 

- ¿El resultado es relevante para mi proyecto o tarea? 

- Y por último, ¿el resultado es coherente si utilizo la misma instrucción varias veces? 

Si detectas algún problema al evaluar el resultado, iterar sobre tu instrucción inicial a menudo puede ayudarte a resolver estos problemas y obtener mejores resultados. Para empezar, si notas que falta algún contexto en tu instrucción, añádelo. Tu elección de palabras también puede repercutir significativamente en los resultados de un LLM. Utilizar palabras o frases diferentes en tus instrucciones a menudo produce diferentes respuestas del modelo. Experimentar con diferentes frases puede ayudarte a obtener el resultado más útil. Ahora que sabes más sobre las instrucciones iterativas, veamos un ejemplo. Supón que trabajas como coordinador de recursos humanos para una productora de video. La empresa quiere desarrollar un programa de prácticas para estudiantes que exploran las carreras relacionadas con la animación y el diseño de gráficos en movimiento. La empresa tiene su sede en Estados Unidos, en el estado de Pensilvania, mi estado natal. Tu equipo quiere asociarse con las universidades locales para ofrecer oportunidades de prácticas para los estudiantes de Pensilvania. Como primer paso, debes crear una lista de universidades en Pensilvania que tengan programas de animación. La lista debe incluir los detalles necesarios sobre las universidades y tener un formato bien organizado que tu equipo pueda revisar rápidamente. Repasemos un ejemplo utilizando Gemini. Ayúdame a encontrar universidades con programas de animación en Pensilvania.

A continuación, examinaremos nuestro resultado. El resultado enumera las universidades de Pensilvania que tienen programas de animación, junto con más información relacionada con estos programas. Es información útil, pero no está estructurada de forma que tu equipo pueda consultar rápidamente al ponerse en contacto con las universidades. Organizar la información en una tabla facilitaría la lectura y comprensión, especialmente para las partes interesadas, como tu gerente, que pueden disponer de poco tiempo. Podemos iterar sobre la instrucción añadiendo contexto para especificar el formato deseado de salida. Escribiremos estas opciones en forma de tabla. El resultado muestra una tabla que proporciona información útil sobre la ubicación de cada universidad y el tipo específico de titulación que ofrece. Ahora, la lista está en un formato organizado que es más fácil de seguir para tu equipo. Aunque la tabla contiene la mayoría de la información que tu equipo necesita, no incluye un detalle clave, si la escuela es pública o privada. Tu empresa quiere ofrecer prácticas a estudiantes de universidades públicas y universidades privadas. Añadiremos una nueva solicitud para que Gemini incluya la información relevante en la tabla. ¿Puedes añadir una columna que muestre si son públicas o privadas? Ahora, la tabla incluye una columna que indica si una universidad es privada o pública. Para compartir esta información con tu equipo en un formato que sea fácil de revisar y comprender, puedes utilizar la función Exportar a Sheets. Esto permitirá a tu equipo a acceder y analizar fácilmente los datos y tomar decisiones informadas basadas en los resultados. Debes aplicar el mismo enfoque iterativo a otras tareas. Cuando desarrolles instrucciones para tareas adicionales, ten en cuenta que las instrucciones anteriores realizadas en la misma conversación pueden influir en el resultado de tu instrucción más reciente. Si observas que esto ocurre, es posible que desees iniciar una nueva conversación. La iteración es una parte clave de la ingeniería de instrucciones. Al adoptar un enfoque iterativo para elaborar instrucciones, puedes aprovechar un LLM para proporcionar los resultados más útiles para tus necesidades.

---
---

# Técnicas para dar instrucciones a un LLM

## Descubre la técnica de algunos ejemplos de instrucciones

¿Has creado alguna vez algo nuevo basándote en ejemplos anteriores? Tal vez utilizaste un informe bien recibido como referencia al redactar un informe similar, o tal vez utilizaste un sitio web relevante y atractivo como modelo a la hora de diseñar tu propio sitio web. Los ejemplos también son útiles para los LLM. **Incluir ejemplos en tu instrucción puede ayudar a un LLM a responder mejor a tu solicitud, y puede ser una estrategia especialmente eficaz para obtener el resultado deseado**. 

Exploraremos cómo utilizar ejemplos en las instrucciones, pero primero, vamos a discutir brevemente el término técnico “intento”. En ingeniería de instrucciones, la palabra “intento” se utiliza a menudo como sinónimo de la palabra “ejemplo”. Existen diferentes nombres para las técnicas de **dar instrucciones en función del número de ejemplos dados al LLM**. Las instrucciones de **intento cero son una técnica que no proporciona ejemplos en una instrucción**, mientras que el ejemplo de instrucción ofrece un solo ejemplo, y “algunos ejemplos de instrucciones” son una técnica que proporciona dos o más ejemplos en una instrucción. 

Como los ejemplos no se incluyen en las instrucciones de intento cero, se espera que el modelo realice la tarea basándose únicamente en sus datos de entrenamiento, y la descripción de la tarea incluida en la instrucción. 

- **Las instrucciones de intento cero pueden ser más eficaces cuando buscas respuestas simples y directas.** Las instrucciones de intento cero pueden no ser eficaces para tareas que requieren que el LLM responda de forma más específica y matizada.

Algunos ejemplos de instrucciones pueden mejorar el rendimiento de los LLM proporcionando contexto adicional y ejemplos adicionales en tu instrucción. Estos ejemplos adicionales pueden ayudar a aclarar el formato deseado, fraseo o patrón general. Algunos ejemplos de instrucciones pueden ser útiles para diversas tareas. Por ejemplo, puedes utilizar algunos ejemplos de instrucciones para generar contenidos con un estilo determinado. Supongamos que trabajas para un minorista en línea. Debes escribir una descripción del producto por un monopatín nuevo. Ya dispones de descripciones de los productos existentes, como una bicicleta y patines. Quieres que la descripción del monopatín siga un estilo y un formato similares. Empezaremos con una instrucción que comienza con unas indicaciones generales. “Escribe una descripción de una oración de un producto. Debe contener dos adjetivos que describan el producto”. También especificamos que queremos que Gemini revise los ejemplos que ofrecemos y escriba la descripción del monopatín en el mismo estilo. Como estos son algunos ejemplos de instrucciones, necesitamos proporcionar ejemplos que modelen el estilo que queremos. Nuestro ejemplo contiene una etiqueta, indicando el producto descrito, una bicicleta y patines. Y cada descripción consta de una oración y contiene dos adjetivos, “elegante” y “duradero” para la bicicleta, y “suave” y “elegante” para los patines.

A continuación, escribimos la etiqueta ”monopatín”. Cuando añadimos esta etiqueta y dejamos en blanco la descripción del producto, indicamos a Gemini que queremos que complete la descripción del monopatín como lo hizo con las otras dos descripciones de productos.

Repasemos nuestros resultados.

El resultado ofrece una descripción del monopatín que cumple los criterios que solicitamos, y tiene el mismo estilo y formato de redacción que los ejemplos que incluimos en nuestra instrucción. En este caso, bastaban dos ejemplos para obtener resultados útiles, pero no existe una regla definitiva para determinar el número óptimo de ejemplos que debemos incluir en una instrucción. Algunos LLM pueden reproducir patrones precisos utilizando solo algunos ejemplos, mientras que otros LLM necesitan más. Al mismo tiempo, si incluyes demasiados ejemplos, las respuestas de un LLM pueden volverse menos flexibles y creativas y pueden reproducir los ejemplos con demasiada fidelidad. Experimenta con el número de ejemplos a incluir para obtener los mejores resultados para tu tarea específica. Ahora ya conoces una técnica para dar instrucciones que te ayudará a obtener resultados de mejor calidad. La estrategia de “algunos ejemplos de instrucciones” es eficaz y puede ayudarte a orientar a un LLM para generar respuestas más útiles.


---

## :book: Explora las instrucciones de cadena de pensamiento

Como ya ha aprendido, existen técnicas de aviso que pueden guiar a un Modelo de lenguaje grande (LLM) en la realización de tareas. La guía de pocos ejemplos es una técnica que proporciona dos o más ejemplos en una guía. Y las instrucciones de un solo paso son técnicas que proporcionan un solo ejemplo en una instrucción.

En esta lectura, aprenderá una tercera técnica que puede utilizar: Indicaciones de cadena de pensamiento. En primer lugar, conocerá las principales aplicaciones laborales de las indicaciones de cadena de pensamiento y cómo pueden mejorar la calidad general de los resultados del LLM. A continuación, revisará un ejemplo detallado de cómo escribir un aviso utilizando esta técnica.

### Resumen

Indicaciones de cadena de pensamiento es una técnica que consiste en solicitar a un Modelo de lenguaje grande que explique sus procesos de razonamiento. Las Indicaciones de cadena de pensamiento son útiles para resolver problemas que implican razonamiento paso a paso. Esta técnica mejora la calidad de las respuestas de un LLM en ciertos casos.


### Ventajas

Las Indicaciones de cadena de pensamiento tienen dos ventajas principales:

1. Puede mejorar la precisión general de los resultados de un LLM. Cuando se divide una tarea en pasos más manejables, se ayuda al LLM a producir resultados precisos y consistentes.

2. Puede mejorar el proceso de resolución de problemas. Al instruir a un LLM para que descomponga el problema, usted puede comprender mejor los pasos que utiliza el LLM para llegar a la solución.


### Aplicaciones

Las Indicaciones de cadena de pensamiento son útiles para resolver problemas que implican razonamiento matemático o lógico. Por ejemplo, puede utilizar el guiado por la cadena de pensamiento cuando tome decisiones de compra, analice datos de ventas o recomiende productos basándose en los requisitos del cliente.

### Diseño del estímulo

![image](https://github.com/eugenia1984/IA/assets/72580574/ede114a5-7074-473f-a038-fe5e2fb757a7)

Las instrucciones de cadena de pensamiento suelen incluir uno o más ejemplos que demuestran cómo resolver un problema en pasos discretos. La instrucción debe proporcionar el contexto del problema o tarea, incluir un ejemplo y formular una petición con instrucciones.

### Ejemplo: Crear un código de compra
He aquí un ejemplo de cómo diseñar un estímulo de cadena de pensamiento para una tarea en el trabajo. Considere una organización con miles de empleados. A cada empleado se le asigna un código de compra único que puede utilizar para comprar suministros o equipos. En primer lugar, un especialista en soporte técnico crea un código de compra único para cada empleado. Para ello, el especialista utiliza una solución de IA personalizada, aprobada para su uso con información de la empresa y de los empleados, que le ayuda a crear el código de compra con la siguiente instrucción de cadena de pensamiento:

Nuestra empresa asigna códigos de compra combinando el departamento y el número de identificación del empleado. Todos los caracteres alfabéticos están en minúsculas en el código de compra. Repase los ejemplos y responda a la pregunta siguiente de la misma manera. Explique los pasos necesarios para determinar el código de compra de cada empleado.

Pregunta: Tiana B trabaja en el departamento de Marketing y tiene el número de identificación 9283. ¿Cuál es el código de compras de Tiana B?

Respuesta: El código de compras de Tiana B es marketing9283. Para determinarlo, combine primero el departamento (Marketing) con el número de identificación (9283). El resultado es Marketing9283. A continuación, cambie todos los caracteres alfabéticos a minúsculas. Esto crea el código de compra marketing9283.

Pregunta: Sylvie E trabaja en el departamento de Ventas y tiene el número de identificación 2379. ¿Cuál es el código de compra de Sylvie E?

Respuesta:

Esta pregunta contiene tres partes principales. En primer lugar, proporciona el contexto. A continuación, incluye un ejemplo. En tercer lugar, se pide al LLM que responda. Analicemos más detenidamente cada parte.

#### Proporciona contexto
En primer lugar, la instrucción proporciona un contexto útil para resolver un problema específico:

Nuestra organización asigna códigos de compras combinando el departamento y el número de identificación del empleado. Todos los caracteres alfabéticos están en minúsculas en el código de compra. Repase el ejemplo y responda a la pregunta siguiente de la misma manera. Explique los pasos necesarios para determinar el código de compra de cada empleado.

La pregunta describe el método de la organización para crear un código de compras. Debido a que ésta es una instrucción de cadena de pensamiento, la instrucción le pide al LLM que siga el ejemplo y explique los pasos que determinan el código de compras.

#### ncluye un ejemplo
La siguiente parte de la pregunta incluye un ejemplo de los pasos utilizados para crear un código de compra, presentado como un par de pregunta y respuesta:

Pregunta: Tiana B trabaja en el departamento de Marketing y tiene el número de identificación 9283. ¿Cuál es el código de compra de Tiana B?

Respuesta: El código de compras de Tiana B es marketing9283. Para determinarlo, combine primero el departamento (Marketing) con el número de identificación (9283). El resultado es Marketing9283. A continuación, cambie todos los caracteres alfabéticos a minúsculas. Esto crea el código de compra marketing9283.

Presentar el ejemplo en formato de pregunta y respuesta facilita su seguimiento por parte del LLM.

La parte de la pregunta del ejemplo incluye información relevante sobre el departamento y el número de identificación del empleado, y solicita el código de compra de Tiana B basándose en esta información.

La parte de la respuesta del ejemplo muestra el razonamiento paso a paso que el especialista quiere que el LLM utilice para determinar el código de compra.

Nota: Es posible que no siempre pueda proporcionar un ejemplo útil en su pregunta. En ese caso, simplemente indique que desea que el LLM explique su razonamiento. La calidad de sus resultados dependerá de su pregunta y del LLM específico que esté utilizando. Intenta incluir el siguiente texto en tu pregunta para obtener los mejores resultados:

"Resuelva el problema paso a paso"

"Explica cada paso utilizado para determinar la respuesta"


#### Enuncia una petición
Finalmente, el prompt incluye la pregunta específica que el LLM debe responder:

Pregunta: Sylvie E trabaja en el departamento de Ventas y tiene el número de identificación 2379. ¿Cuál es el código de compras de Sylvie E?

Respuesta:

La pregunta sigue el patrón del ejemplo anterior para facilitar que el LLM proporcione una respuesta similar. El campo después de la etiqueta "Respuesta:" está en blanco para indicar que el LLM debe completar la respuesta.



---

## :tv: Rachna: Mejora las instrucciones mediante la exploración

Hola, soy Rachna. Soy ingeniero de software en Google. Trabajo en un equipo llamado **Gestión central del conocimiento,** y somos responsables de **asegurarnos de que los desarrolladores tengan acceso a toda la información que necesitan**. 

Una de las cosas más importantes para aprender sobre IA son las **instrucciones**, que es simplemente **descubrir qué texto introducir para obtener la respuesta deseada.**.

Una forma de encontrar las instrucciones más eficaces para los LLM, o modelos de lenguaje grande, es **hacer iteraciones rápidamente con ellos y probar una gran variedad de instrucciones diferentes**. Así que, si no fue lo suficientemente divertido, la próxima vez podrías intentar pedirle al LLM que lo haga más divertido. O si es demasiado vago, puedes utilizar una instrucción para pedir específicamente que la IA no sea imprecisa. 

**Probar un montón de cosas diferentes de esta manera generalmente te dará buenos resultados.** 

Una forma de cambiar cómo estás utilizando los LLM para permitirles ser más creativos o más específicos se basa en **cuánto contexto ingreses**. Así que **si quieres que el LLM te dé una respuesta bastante creativa, puedes probar con una instrucción muy corta. Si quieres que sea muy específico, puedes poner muchos ejemplos, y entonces se ajustará más a tus ejemplos**. 

Otra técnica que es muy interesante son las **instrucciones de cadena de pensamiento**, donde se pide al modelo que que razone su propia respuesta. Así que si le estás pidiendo al modelo que siga algún cálculo matemático, una ecuación matemática, puedes pedirle que primero lo descomponga en pasos, luego haga el primer paso y luego el segundo paso, y así sucesivamente. Y conseguir que el LLM realice múltiples pasos a veces puede hacerlo mucho más preciso. 

Una técnica que utilizamos que es un poco más imprevista es pedir al modelo que reaccione a sus propias respuestas. Así que a veces pido al modelo una respuesta. Y luego digo: ¿es vaga esta respuesta? Y si la respuesta es afirmativa, entonces a veces descarto esa respuesta. Entonces, lo dejo hacer parte de mi trabajo por mí. Cuanto más experimentes y más creativo seas, mejor. Mantenerse al día con la IA puede sentirse un poco como correr en una cinta a veces, y cada vez va más rápido, y hay tantas cosas cosas nuevas que están cambiando, pero creo que eso es también lo que lo hace realmente divertido.

---

## :book: Mejores prácticas para la ingeniería de instrucciones


Los modelos de lenguaje grande (LLM) reaccionan a lo que les pedimos: cuanto mejor sea la indicación, mejor será el resultado. Utiliza esta guía para crear instrucciones eficaces que ayuden a los LLM a desempeñarse al máximo para que puedas obtener las respuestas más provechosas.

### Especifica la tarea

Los LLM se entrenan con cantidades masivas de datos.  Tienes que ser específico sobre el resultado que deseas, para que el Modelo pueda ofrecer un resultado bien enfocado. Sé claro con respecto a lo que quieres que hagan los LLM proporcionándoles suficientes parámetros. Usa un lenguaje sencillo y haz que las consultas tengan una estructura lógica para que el modelo interprete mejor tu solicitud. No es mejor una configuración específica; escribe de forma intuitiva y céntrate en la claridad.

Ejemplo: Redacta un correo electrónico informal dirigido a mi jefe para solicitar una licencia.

### roporciona el contexto necesario

El contexto determina la forma en que los LLM responden a una instrucción porque proporcionan información importante sobre tus expectativas. Si se incluye un contexto relevante, es más probable que los LLM generen resultados útiles.

Incluye detalles clave sobre lo que pides para dar a los LLM la información que necesitan para generar resultados útiles. A continuación, hay algunas preguntas que se deben considerar a la hora de redactar una instrucción eficaz:

- ¿Cuál es el público objetivo? Especifica las cualidades pertinentes de los destinatarios, como la edad, la profesión o el nivel de comprensión de un tema.

- ¿Qué tono debe utilizar el modelo? Aclara el aire y el estilo que deben utilizar los LLM para transmitir tu mensaje de la manera más eficaz. Quizás quieras un resultado informal y amistoso si lo vas utilizar para comunicarte con un colega, o algo más profesional y persuasivo para los clientes. 

- ¿Cómo deben estructurar los resultados los LLM? Especifica el formato que deben utilizar los LLM para ordenar la información que proporcionan. Puedes incluir pautas sobre la longitud o especificar un tipo de presentación, como una lista con viñetas o una tabla.

- ¿Cuál es la finalidad del resultado? Identifica lo que quieres que logren los LLM con una determinada instrucción. Por ejemplo, si en la instrucción se le pide al modelo que explique un concepto, la finalidad puede ser que los principiantes en ese campo específico adquieran una comprensión práctica del tema. Asignar una finalidad al LLM te ayudará a adaptar los resultados a tus necesidades específicas.

Ejemplo: Escribe un correo electrónico amistoso a mi colega de RR. HH. para agradecerle por su colaboración en un proyecto reciente y que sepa que su aporte fue inestimable.

### Proporciona referencias

Proporcionar a los LLM material de referencia que cumpla tus objetivos o se parezca a lo que quieres crear puede ayudar a generar mejores resultados. Ya sea que incluyas tu propio trabajo, fuentes más generales o ambos, también deberías explicar claramente en qué sentido ese material de referencia se relaciona con tu instrucción para obtener los mejores resultados posibles.

Ejemplo: Redacta una lista de posibles eslóganes de campaña para una empresa de anteojos de sol siguiendo el estilo escrito de los anuncios publicitarios de los años sesenta.

### Evalúa tus resultados

Cada modelo tiene un conjunto de entrenamiento único, se basa en técnicas de programación diferentes y se crea en un momento determinado. Como resultado, algunos LLM pueden saber más que otros sobre ciertos temas o tener un límite de conocimientos. Además, a veces las modelos generan alucinaciones. 

Antes de utilizar un resultado generado con IA, haz una evaluación crítica del resultado para asegurarte de que sea aceptable y provechoso para ti. Eso puede implicar llevar a cabo algo de investigación después de que los LLM generen sus resultados. Al evaluar un resultado, pregúntate: 

- ¿Es precisa esta respuesta? Confirma que la información está actualizada y sea cierta. 

- ¿Es imparcial esta respuesta? Evalúa si la respuesta es justa e imparcial, representa con exactitud a las poblaciones y evita el trato preferencial con determinadas personas o grupos.

- ¿Incluye información suficiente esta respuesta? Asegúrate de que el resultado arroje una respuesta completa y satisfactoria a tu consulta. 

- ¿Es pertinente esta respuesta para lo que necesito? Comprueba que el resultado esté relacionado con la instrucción y se ajuste al contexto, el tema y la tarea que definiste. 

- ¿Es congruente esta respuesta? Comprueba que la respuesta no sea un caso aislado. Si no lo sabes con seguridad, ingresa instrucciones varias veces en el LLM e ingrésalas con diferentes formulaciones para asegurarte de que los resultados te proporcionan información similar. 


Si determinas que un resultado no es aceptable, agrega más contexto a la instrucción inicial para generar una respuesta más acotada: 

Ejemplo: El resultado ante una instrucción como ¿Qué es una condicional? puede ser muy amplio, variado o irrelevante para tus necesidades porque ese término tiene significados diferentes en diversos contextos.

Iteración: En cambio, una instrucción como Explica las “condicionales” a un programador principiante como en un libro de texto  probablemente obtenga un resultado más específico y útil al especificar el destinatario, el tono y la disciplina.

###  Adopta un enfoque iterativo

Por el motivo que sea, es posible que un LLM no genere lo que necesitas la primera vez que se lo pides. Pero igualmente puedes obtener el resultado deseado con iteraciones, perfeccionando la instrucción inicial, enviando solicitudes de seguimiento o enviando comentarios a los LLM.

Para corregir adecuadamente una instrucción, conserva lo que sirvió y haz modificaciones a partir de eso. Podrías modificar la formulación (por ejemplo, la instrucción podría ser una orden o una pregunta), reordenar los componentes de la instrucción (por ejemplo, podría empezar o terminar con un ejemplo) o proporcionar contexto adicional para ayudar a limitar las respuestas de los LLM.

Ejemplo: Resume las siguientes notas de la reunión.

Iteración: Resume las siguientes notas de la reunión e identifica los puntos clave.

Iteraciones adicionales: Resume las siguientes notas de la reunión, identifica los puntos clave y enumera los elementos de acción más urgentes y sus respectivos plazos.

Para realizar solicitudes de seguimiento de forma eficaz, pide al modelo que realice ajustes sin repetir la instrucción inicial, como si fuera un diálogo, un ida y vuelta. Los LLM son capaces de basarse en interacciones previas dentro de una conversación, lo cual significa que puedes concentrarte en hacer ajustes específicos e individuales hasta que tengas todo lo que necesitas.

Ejemplo: Resume las siguientes notas de la reunión.

Seguimiento: ¿Cuáles fueron los puntos clave de esa reunión?

Segunda solicitud: ¿Cuáles son los puntos de acción más urgentes y sus plazos?



---
---

#  Revisión: Descubre el arte de la ingeniería de instrucciones

## :tv: Actividad de cierre


Has aprendido mucho sobre cómo escribir instrucciones que puedes aplicar a las tareas en el lugar de trabajo. En esta sección, abordamos el modelo de lenguaje grande o resultado LLM. Examinamos cómo los LLM producen sus resultados y los posibles problemas que puedes encontrar en los resultados. Después, nos centramos en un principio clave de ingeniería de instrucciones, creando instrucciones claras y específicas. Aprenderás lo importante que es especificar lo que deseas que haga el LLM e incluir un contexto de apoyo para ayudarle a proporcionar un mejor resultado. A continuación pasamos a descubrir cómo mejorar la calidad del resultado de la IA a través de la iteración. Es esencial que evalúes tus resultados y, a continuación, revises tu instrucción según sea necesario. Por último, aprendimos sobre algunos ejemplos de instrucciones, que consiste en ofrecer ejemplos para guiar al LLM. Quiero dar un último consejo antes de irme. Nos centramos en dar instrucciones a modelos de lenguaje grande. Puedes utilizar los mismos principios generales cuando envíes instrucciones a otros tipos de modelos de IA. Por ejemplo, la próxima vez que quieras utilizar la IA para generar una imagen, intenta ser lo más claro y específico posible, y luego itera para acercarte al resultado deseado. Ha sido genial guiarte a través del proceso de la ingeniería de instrucciones, espero que sigas aplicando y desarrollando estas habilidades a medida que aprovechas las herramientas conversacionales de la IA en el lugar de trabajo. Para seguir aprendiendo, te animo a explorar el tema del uso responsable de la IA como parte de los Fundamentos de IA de Google.

---
---
