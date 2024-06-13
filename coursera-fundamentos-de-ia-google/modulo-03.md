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

---
---

# Técnicas para dar instrucciones a un LLM

---
---

#  Revisión: Descubre el arte de la ingeniería de instrucciones

---
