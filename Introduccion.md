# Introduccion

Este libro es una guía de cómo desarrollamos productos en Basecamp. También es una caja de herramientas llena de técnicas que puede aplicar a su manera a su propio proceso.

Si usted es fundador, CTO, gerente de producto, diseñador o desarrollador, probablemente esté aquí debido a algunos desafíos comunes que todas las compañías de software tienen que enfrentar.

## Dolores de crecimiento


A medida que los equipos de software van creciendo, aparecen algunas dificultades comunes:

- Los miembros del equipo sienten que los proyectos siguen y siguen, sin un final a la vista.

- Los gerentes de producto no pueden encontrar tiempo para pensar estratégicamente sobre el producto.

- Los fundadores se preguntan: "¿Por qué no podemos sacar por la puerta las funciones como solíamos hacer en los primeros días?"

Vimos estos desafíos de primera mano en Basecamp a medida que pasamos de cuatro personas a más de cincuenta.

Basecamp comenzó en 2003 como una herramienta que construimos para nosotros mismos. En ese momento éramos una consultora que diseñaba sitios web para clientes. La información se perdía en llamadas teléfonicas entre el cliente, el diseñador y la persona que gestionaba el proyecto. Queríamos que Basecamp fuera un lugar centralizado donde todas las partes pudieran ver el trabajo, discutirlo y saber qué hacer a continuación. Resultó que muchas empresas tenían este problema de "información que se escapaba por las grietas". Hoy en día, millones de personas de todo tipo de industrias confían en Basecamp como su fuente compartida de información.

Tres de nosotros construimos la primera versión. Jason Fried, fundador de Basecamp, dirigió el diseño. Su cofundador, David Heinemeier Hansson, lo programó (y creó el conocido framework web Ruby on Rails como subproducto). En ese momento, yo era diseñador web con un enfoque en usabilidad e interfaces de usuario. Ejecuté la dirección de diseño de Jason para las funciones clave de la aplicación y colaboré con él para completar los detalles del concepto.

Desde los primeros prototipos en julio de 2003 hasta su lanzamiento en febrero de 2004, David solo trabajó diez horas a la semana. Sabíamos que no llegaríamos a ningún lado con esas diez horas de programación a menos que las usáramos de manera muy deliberada. Nuestro intenso enfoque en "martillar" el alcance para que se ajuste a un presupuesto de tiempo dado nació bajo estas limitaciones.

A medida que el negocio crecía, comencé a ampliar mis habilidades. Trabajar con David y Ruby on Rails hizo que el mundo de la programación fuera accesible para mí. Aprendí las técnicas que usan los programadores para dominar la complejidad: cosas como factorización, niveles de abstracción y separación de responsabilidades. Con un pie en el mundo del diseño y un pie en el mundo de la programación, me preguntaba si podríamos aplicar estos principios de desarrollo de software a la forma en que diseñamos y gestionamos el producto.

La primera prueba de esta idea se produjo en 2009. Para entonces, habíamos contratado algunos programadores más y ofrecimos cuatro productos de software como servicio independientes. Queríamos agrupar los productos en una suite perfecta con inicio de sesión único y facturación unificada. Fue una mision técnica masiva con flujos traicioneros de cara al usuario. Además de corregir la arquitectura subyacente, tuvimos que interrumpir a los clientes en su camino hacia el producto y hacer que cambiaran su nombre de usuario y contraseña por motivos que no eran fáciles de explicar. En el proyecto usé los sombreros de diseñador y gerente de producto y realicé un prototipo de las técnicas de mapeo de alcance y tablero de pruebas descritas en este libro para gestionar la complejidad.

Tuvimos tan buenos resultados que decidimos aplicar las mismas técnicas nuevamente en 2012, cuando rediseñamos Basecamp desde cero para la versión 2.0. Una vez más, hubo mucha superficie para gestionar y, de nuevo, el proceso fue sorprendentemente fluido.

Para 2015, teníamos un equipo central que había vivido estas experiencias y había logrado un avance impresionante. Pero nos resultó difícil articular lo que estábamos haciendo con los nuevos empleados. Nuestro equipo de productos se había cuadriplicado y todos trabajaban de forma remota. Eso hizo que fuera difícil transmitir nuestras intuiciones. Necesitábamos lenguaje para describir lo que estábamos haciendo y más estructura para seguir haciéndolo a nuestra nueva escala.

Para gestionar esta nueva capacidad, pasamos de proyectos de duración ad-hoc a ciclos repetidos. (Se necesitó algo de experimentación para encontrar la duración correcta del ciclo: seis semanas. Más sobre eso más adelante). Formalizamos nuestros procesos de lanzamiento y apuestas. Mi función cambió nuevamente, del diseño y la gestión de productos a la estrategia de productos. Necesitaba un nuevo lenguaje, como la palabra "dar forma"(shape up), para describir el trabajo de diseño inicial que hicimos para establecer límites y reducir los riesgos en los proyectos antes de que los comprometiéramos con los equipos.

Justo cuando estábamos mejorando en articular la forma en que trabajamos con nosotros mismos, más y más amigos y compañeros comenzaron a acudir a nosotros para preguntarnos cómo lo hacemos. Finalmente Jason me llevó a un lado un día y me dijo: Creo que deberías escribir un libro sobre esto.

Este es el resultado. Puedes pensar en esto como dos libros en uno. Primero, es un libro de verdades básicas. Quiero que le brinde al lector un mejor lenguaje para describir y lidiar con los riesgos, las incertidumbres y los desafíos que surgen cada vez que desarrolla un producto. En segundo lugar, el libro describe los procesos específicos que utilizamos para lograr un progreso significativo en nuestros productos en nuestra escala actual.

A continuación, se ofrece una breve descripción general de las ideas principales del libro.

## Ciclos de seis semanas

Primero, trabajamos en ciclos de seis semanas. Seis semanas es suficiente para construir algo significativo de principio a fin y lo suficientemente corto como para que todos puedan sentir que la fecha límite se avecina desde el principio, por lo que usan el tiempo sabiamente. La mayoría de nuestras nuevas funciones se crean y lanzan en un ciclo de seis semanas.

Nuestras decisiones se basan en hacer avanzar el producto en las próximas seis semanas, no en la microgestión del tiempo. No contamos las horas ni nos preguntamos cómo se gastan los días individuales. No tenemos reuniones diarias. No repensamos nuestra hoja de ruta cada dos semanas. Nuestro enfoque está en un nivel superior. Nos decimos a nosotros mismos: "Si este proyecto se lanza después de seis semanas, estaremos muy felices. Sentiremos que nuestro tiempo estuvo bien invertido". Luego comprometemos las seis semanas y dejamos al equipo solo para que lo haga.

## Dando forma al trabajo

En segundo lugar, damos forma al trabajo antes de dárselo a un equipo. Un pequeño grupo senior trabaja en paralelo a los equipos de ciclo. Definen los elementos clave de una solución antes de que consideremos un proyecto listo para apostar. Los proyectos se definen en el nivel correcto de abstracción: lo suficientemente concretos para que los equipos sepan qué hacer, pero lo suficientemente abstractos como para que tengan espacio para resolver los detalles interesantes por sí mismos.

Al dar forma, nos centramos menos en las estimaciones y más en nuestro apetito. En lugar de preguntar cuánto tiempo tomará hacer algo de trabajo, preguntamos: ¿Cuánto tiempo queremos dedicar? ¿Cuánto vale esta idea? Ésta es la tarea de dar forma: delimitar el problema y diseñar el esquema de una solución que se ajuste a las limitaciones de nuestro apetito.

## Responsabilizar a los equipos

En tercer lugar, damos toda la responsabilidad a un pequeño equipo integrado de diseñadores y programadores. Ellos definen sus propias tareas, hacen ajustes en el alcance y trabajan juntos para construir cortes verticales del producto uno a la vez. Esto es completamente diferente de otras metodologías, donde los gerentes dividen el trabajo y los programadores actúan como tomadores de boletos.

Juntos, estos conceptos forman un círculo virtuoso. Cuando los equipos son más autónomos, los gerentes pueden dedicar menos tiempo a administrarlos. Con menos tiempo dedicado a la gestión, los altos cargos pueden diseñar mejores proyectos. Cuando los proyectos están mejor configurados, los equipos tienen límites más claros y, por lo tanto, pueden trabajar de manera más autónoma.

## Apuntando al riesgo

En cada paso del proceso apuntamos a un riesgo específico: el riesgo de no entregar a tiempo. Este libro no trata sobre el riesgo de construir algo incorrecto. Otros libros pueden ayudarte con eso (recomendamos [Competing Against Luck][1]). La mejora de su proceso de descubrimiento debería llegar después de recuperar su capacidad de entrega. Puede tener la mejor estrategia del mundo, pero si no puede actuar en consecuencia, ¿de qué sirve?

Este libro trata sobre el riesgo de atascarse, el riesgo de empantanarse con el trabajo del último trimestre, perder el tiempo en problemas inesperados y no tener la libertad de hacer lo que quiere hacer mañana.

Reducimos el riesgo en el proceso de modelado resolviendo preguntas abiertas antes de comprometer el proyecto en una caja de tiempo. No le damos a un equipo un proyecto que todavía tiene agujeros de conejo o interdependencias enredadas.

Reducimos el riesgo en el proceso de planificación al limitar nuestras apuestas a seis semanas. Si un proyecto se ejecuta, de forma predeterminada no recibe una extensión. Este "cortacircuitos" asegura que no invirtamos múltiplos del apetito original en un concepto que primero necesita repensarse.

Y, por último, reducimos el riesgo en el proceso de construcción al integrar el diseño y la programación desde el principio. En lugar de construir muchas piezas desconectadas y esperar que encajen juntas en la undécima hora, construimos una pieza significativa del trabajo de principio a fin y luego la repetimos. El equipo secuencia el trabajo desde las piezas más desconocidas hasta las menos preocupantes y aprende qué funciona y qué no mediante la integración lo antes posible.

## Cómo está organizado este libro

La primera parte se trata de dar forma, el trabajo previo que hacemos en los proyectos antes de considerarlos listos para programar. Cada capítulo explica un paso específico del proceso, desde poner el apetito en una idea en bruto, esbozar una solución y escribir un discurso que presente el proyecto potencial. A lo largo del camino, aprenderá técnicas específicas, como las tablas de pruebas y bocetos de marcadores gruesos, para mantener el diseño en el nivel correcto de abstracción.

La segunda parte trata sobre las apuestas: cómo elegimos entre los proyectos presentados y decidimos qué hacer seis semanas a la vez.

La tercera parte trata sobre la construcción: las expectativas que ponemos en los equipos y las prácticas especiales que utilizan para descubrir qué hacer. Veremos cómo los equipos descubren qué hacer, cómo integran el diseño y la programación, cómo rastrean lo conocido frente a lo desconocido y, finalmente, cómo toman las decisiones difíciles para terminar el proyecto a tiempo.

Por último, el Apéndice le brinda ayuda para cuando sea el momento de realizar cambios en su empresa. Hay algunos consejos sobre cómo probar su primer experimento de seis semanas, consejos sobre cómo ajustar los métodos al tamaño de su empresa y orientación específica sobre cómo implementar Shape Up con Basecamp.

[1]: https://www.amazon.com/Competing-Against-Luck-Innovation-Customer/dp/0062435612