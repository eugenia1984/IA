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

Por ejemplo, si estás desarrollando una propuesta, un informe u otro documento para compartir con tus compañeros de trabajo, es posible que elabores varios borradores y realices mejoras en cada borrador hasta que te satisfaga el resultado. Adoptar un enfoque iterativo suele ser la forma más eficaz para resolver un problema o desarrollar un producto. Un proceso iterativo también es eficaz en la ingeniería de instrucciones. La ingeniería de instrucciones a menudo requiere múltiples intentos antes de obtener el resultado óptimo. La mayoría de las veces, no obtendrás el mejor resultado en el primer intento. Si intentas algo y no funciona, no te desanimes. En su lugar, evalúa cuidadosamente el resultado para determinar por qué no obtuviste la respuesta deseada. A continuación, revisa tu instrucción para intentar obtener un mejor resultado. Consideremos las posibles razones por las que puede que no obtengas resultados útiles después de crear una instrucción clara y específica. En primer lugar, las diferencias en modelos de lenguaje grande pueden afectar el resultado. Cada LLM se desarrolla con datos de entrenamiento únicos y técnicas de programación, y tiene diferentes conocimientos previos sobre ámbitos específicos. Por esta razón, diferentes modelos pueden responder a instrucciones similares de diferentes maneras. Y podría fracasar en dar una respuesta adecuada a algunas instrucciones. Adoptar un enfoque iterativo con el LLM que estás utilizando producirá los mejores resultados. En segundo lugar, las limitaciones del LLM. Anteriormente, aprendiste que los resultados del LLM a veces pueden ser inexactos, sesgados, insuficientes, irrelevantes o incoherentes. Deberás evaluar de forma crítica todos los resultados del LLM planteándote las siguientes preguntas. ¿El resultado es preciso? ¿El resultado es imparcial? ¿El resultado incluye suficiente información? ¿El resultado es relevante para mi proyecto o tarea? Y por último, ¿el resultado es coherente si utilizo la misma instrucción varias veces? Si detectas algún problema al evaluar el resultado, iterar sobre tu instrucción inicial a menudo puede ayudarte a resolver estos problemas y obtener mejores resultados. Para empezar, si notas que falta algún contexto en tu instrucción, añádelo. Tu elección de palabras también puede repercutir significativamente en los resultados de un LLM. Utilizar palabras o frases diferentes en tus instrucciones a menudo produce diferentes respuestas del modelo. Experimentar con diferentes frases puede ayudarte a obtener el resultado más útil. Ahora que sabes más sobre las instrucciones iterativas, veamos un ejemplo. Supón que trabajas como coordinador de recursos humanos para una productora de video. La empresa quiere desarrollar un programa de prácticas para estudiantes que exploran las carreras relacionadas con la animación y el diseño de gráficos en movimiento. La empresa tiene su sede en Estados Unidos, en el estado de Pensilvania, mi estado natal. Tu equipo quiere asociarse con las universidades locales para ofrecer oportunidades de prácticas para los estudiantes de Pensilvania. Como primer paso, debes crear una lista de universidades en Pensilvania que tengan programas de animación. La lista debe incluir los detalles necesarios sobre las universidades y tener un formato bien organizado que tu equipo pueda revisar rápidamente. Repasemos un ejemplo utilizando Gemini. Ayúdame a encontrar universidades con programas de animación en Pensilvania.

A continuación, examinaremos nuestro resultado. El resultado enumera las universidades de Pensilvania que tienen programas de animación, junto con más información relacionada con estos programas. Es información útil, pero no está estructurada de forma que tu equipo pueda consultar rápidamente al ponerse en contacto con las universidades. Organizar la información en una tabla facilitaría la lectura y comprensión, especialmente para las partes interesadas, como tu gerente, que pueden disponer de poco tiempo. Podemos iterar sobre la instrucción añadiendo contexto para especificar el formato deseado de salida. Escribiremos estas opciones en forma de tabla. El resultado muestra una tabla que proporciona información útil sobre la ubicación de cada universidad y el tipo específico de titulación que ofrece. Ahora, la lista está en un formato organizado que es más fácil de seguir para tu equipo. Aunque la tabla contiene la mayoría de la información que tu equipo necesita, no incluye un detalle clave, si la escuela es pública o privada. Tu empresa quiere ofrecer prácticas a estudiantes de universidades públicas y universidades privadas. Añadiremos una nueva solicitud para que Gemini incluya la información relevante en la tabla. ¿Puedes añadir una columna que muestre si son públicas o privadas? Ahora, la tabla incluye una columna que indica si una universidad es privada o pública. Para compartir esta información con tu equipo en un formato que sea fácil de revisar y comprender, puedes utilizar la función Exportar a Sheets. Esto permitirá a tu equipo a acceder y analizar fácilmente los datos y tomar decisiones informadas basadas en los resultados. Debes aplicar el mismo enfoque iterativo a otras tareas. Cuando desarrolles instrucciones para tareas adicionales, ten en cuenta que las instrucciones anteriores realizadas en la misma conversación pueden influir en el resultado de tu instrucción más reciente. Si observas que esto ocurre, es posible que desees iniciar una nueva conversación. La iteración es una parte clave de la ingeniería de instrucciones. Al adoptar un enfoque iterativo para elaborar instrucciones, puedes aprovechar un LLM para proporcionar los resultados más útiles para tus necesidades.

---
---

# Técnicas para dar instrucciones a un LLM

---
---

#  Revisión: Descubre el arte de la ingeniería de instrucciones

---
