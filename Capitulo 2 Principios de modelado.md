Cuando damos forma al trabajo, debemos hacerlo en el nivel correcto de abstracción: ni demasiado vago ni demasiado concreto. Los gerentes de producto a menudo se equivocan en uno de estos dos extremos.

## Los wireframes son demasiado concretos

Cuando los líderes de diseño van directamente a los wireframes o maquetas de alta fidelidad, definen demasiados detalles demasiado pronto. Esto no deja a los diseñadores espacio para la creatividad. Un amigo lo expresó de esta manera:

> Le daré una estructura alámbrica a mi diseñadora y luego le digo: "Sé que estás viendo esto, pero eso no es lo que quiero que diseñes. ¡Quiero que lo reconsideres! " Es difícil hacer eso cuando les estás dando algo concreto.

La sobreespecificación del diseño también conduce a errores de estimación. Por contradictorio que parezca, cuanto más específico sea el trabajo, más difícil será estimarlo. Esto se debe a que hacer que la interfaz sea así puede requerir resolver complejidades ocultas y detalles de implementación que no estaban visibles en la maqueta. Cuando el alcance no es variable, el equipo no puede reconsiderar una decisión de diseño que está resultando costar más de lo que vale.

## Las palabras son demasiado abstractas

En el otro extremo del espectro, los proyectos que son demasiado vagos tampoco funcionan. Cuando un proyecto se define en pocas palabras, nadie sabe lo que significa. “Crear una vista de calendario” o “agregar notificaciones grupales” suena sensato, pero ¿qué implican exactamente? Los miembros del equipo no tienen suficiente información para hacer concesiones. No saben qué incluir u omitir. Un programador que trabajó en esa situación dijo:

> Estás resolviendo un problema sin contexto. Tienes que ser un lector de mentes. Es como: "lo sabremos cuando lo veamos".

Con respecto a la estimación, los proyectos subespecificados naturalmente crecen fuera de control porque no hay límites para definir lo que está fuera de alcance.

## Estudio de caso: el calendario de cuadrícula de puntos

Veamos un ejemplo de cómo dar forma a un proyecto con el nivel de detalle adecuado.

Lanzamos la versión tres de Basecamp sin una función de calendario. Tenía una función de "programación" que solo enumeraba los eventos uno tras otro sin ningún tipo de cuadrícula mensual, semanal o diaria.

Poco después del lanzamiento, los clientes comenzaron a pedirnos que "agreguemos un calendario" a Basecamp. Ya habíamos construido calendarios antes y sabíamos lo complejos que son. Puede llevar fácilmente seis meses o más crear un calendario adecuado.

Estos son los tipos de cosas que complican un calendario:

- Arrastrar y soltar eventos entre celdas para moverlos
- Envolviendo eventos de varios días alrededor del borde de la pantalla
- Diferentes vistas para escalas de tiempo mensuales, semanales o diarias
- Arrastrar el borde de un evento para cambiar su duración
- Eventos de codificación de colores para diferentes categorías
- Manejo de diferentes expectativas para interacciones de escritorio y móviles

Las versiones anteriores de Basecamp tenían calendarios, y solo alrededor del 10% de los clientes los usaban. Por eso no teníamos ganas de pasar seis meses en un calendario. Por otro lado, si pudiéramos hacer algo para satisfacer a los clientes que nos escribían en un ciclo de seis semanas, estaríamos dispuestos a hacerlo.

Con solo seis semanas para trabajar, solo pudimos construir alrededor de una décima parte de lo que la gente piensa cuando dice "calendario". La pregunta fue: ¿cuál décimo?

Investigamos un poco (discutido en el próximo capítulo) y redujimos un caso de uso que queríamos resolver. Finalmente llegamos a un concepto prometedor inspirado en los calendarios de los teléfonos. Podríamos crear una vista de cuadrícula de solo lectura de dos meses. Cualquier día con un evento tendría un punto para cada evento. Aparecería una lista de eventos debajo del calendario, y al hacer clic en un día con un punto, los eventos de ese día se desplazarían a la vista. Lo llamamos Dot Grid.

Dot Grid no era un calendario con todas las funciones. No íbamos a permitir arrastrar eventos entre días. No íbamos a abarcar eventos de varios días en toda la red; simplemente repetiríamos los puntos. No habría códigos de colores ni categorías para los eventos. Nos sentíamos cómodos con todas estas compensaciones debido a nuestra comprensión del caso de uso.

Este es el nivel de fidelidad que usamos para definir la solución:

Observe cuán tosco es el boceto y cuántos detalles quedan fuera. El diseñador tuvo mucho espacio para interpretar cómo debería verse y sentirse esto.

Al mismo tiempo, observe cuán específica es la idea. Está muy claro cómo funciona, qué se necesita construir, qué está dentro y qué está fuera.

Al final del proyecto, el trabajo terminado que crearon los diseñadores y programadores se veía así:

Este pequeño ejemplo destaca algunas propiedades del trabajo con forma.

## Propiedad 1: Es duro

El trabajo en la etapa de modelado es duro. Todo el mundo puede decir al mirarlo que está inacabado. Pueden ver los espacios abiertos donde irán sus contribuciones. Trabajar demasiado bien, demasiado pronto compromete a todos con los detalles incorrectos. Los diseñadores y programadores necesitan espacio para aplicar su propio juicio y experiencia cuando se arremangan y descubren todas las compensaciones reales que surgen.

## Propiedad 2: está resuelto

A pesar de ser tosco e inacabado, el trabajo moldeado ha sido pensado. Todos los elementos principales de la solución están en el nivel macro y se conectan entre sí. El trabajo no se especifica en tareas individuales, sino que se detalla la solución general. Si bien aún pueden ocurrir sorpresas y aún pueden surgir icebergs, hay una dirección clara que muestra qué hacer. Cualquier pregunta abierta o agujeros de conejo que pudiéramos ver desde el principio se han eliminado para reducir el riesgo del proyecto.

## Propiedad 3: está acotado

Por último, el trabajo con forma indica lo que no se debe hacer. Le dice al equipo dónde detenerse. Hay un apetito específico: la cantidad de tiempo que el equipo puede dedicar al proyecto. Completar el proyecto dentro de esa cantidad de tiempo fija requiere limitar el alcance y dejar cosas específicas.

En conjunto, la aspereza deja espacio para que el equipo resuelva todos los detalles, mientras que la solución y los límites actúan como barandillas. Reducen el riesgo y canalizan los esfuerzos del equipo, asegurándose de que no construyan demasiado, deambulen o se atasquen.

## Quien da forma

Dar forma es creativa e integradora. Requiere combinar ideas de interfaz con posibilidades técnicas con prioridades comerciales. Para hacer eso, deberá incorporar estas habilidades como generalista o colaborar con una o dos personas más.

Dar forma es principalmente trabajo de diseño. El concepto de forma es un diseño de interacción visto desde la perspectiva del usuario. Define qué hace la característica, cómo funciona y dónde encaja en los flujos existentes.

No es necesario ser un programador para dar forma, pero debe tener conocimientos técnicos. Debería poder juzgar qué es posible, qué es fácil y qué es difícil. El conocimiento sobre cómo funciona el sistema lo ayudará a ver oportunidades u obstáculos para implementar su idea.

También es un trabajo estratégico. Establecer el apetito y encontrar una solución requiere que usted sea crítico con el problema. ¿Qué estamos tratando de resolver? ¿Por qué eso importa? ¿Qué cuenta como éxito? ¿Qué clientes se ven afectados? ¿Cuál es el costo de hacer esto en lugar de otra cosa?

Dar forma es un proceso creativo a puertas cerradas. Puede estar solo dibujando en papel o frente a una pizarra con un colaborador cercano. Habrá diagramas aproximados frente a usted que nadie fuera de la habitación podría interpretar. Cuando trabaja con un colaborador, se mueve rápido, habla con franqueza y salta de una posición prometedora a otra. Es ese tipo de trabajo privado, duro y temprano.

## Dos pistas

Realmente no se puede programar el trabajo de modelado porque, por su propia naturaleza, el trabajo sin modelar es riesgoso y desconocido. Por esa razón tenemos dos pistas separadas: una para dar forma y otra para construir. Durante cualquier ciclo de seis semanas, los equipos están construyendo el trabajo que se ha formado previamente y los modeladores están trabajando en lo que los equipos podrían construir potencialmente en un ciclo futuro. El trabajo en la pista de modelado se mantiene en privado y no se comparte con el equipo en general hasta que se haya hecho el compromiso de apostar por él. Eso les da a los modeladores la opción de poner el trabajo en progreso en el estante o dejarlo cuando no está funcionando.

## Pasos para dar forma

Dar forma tiene cuatro pasos principales que cubriremos en los próximos cuatro capítulos.

1. Establecer límites. Primero, averiguamos cuánto tiempo vale la idea en bruto y cómo definir el problema. Esto nos da los límites básicos para moldearnos.
2. Analice los elementos. Luego viene el trabajo creativo de esbozar una solución. Hacemos esto a un nivel de abstracción más alto que los wireframes para movernos rápido y explorar una amplia gama de posibilidades. El resultado de este paso es una idea que resuelve el problema dentro del apetito pero sin todos los detalles finos resueltos.
3. Aborde los riesgos y las madrigueras. Una vez que pensamos que tenemos una solución, la examinamos detenidamente para encontrar huecos o preguntas sin respuesta que puedan hacer tropezar al equipo. Modificamos la solución, eliminamos cosas de ella o especificamos detalles en ciertos puntos difíciles para evitar que el equipo se atasque o pierda el tiempo.
4. Escribe el discurso. Una vez que pensamos que lo hemos moldeado lo suficiente como para apostar potencialmente, lo empaquetamos con un artículo formal llamado discurso. El lanzamiento resume el problema, las limitaciones, la solución, los agujeros del conejo y las limitaciones. El lanzamiento va a la mesa de apuestas para su consideración. Si se elige el proyecto, el terreno de juego se puede reutilizar en el inicio para explicar el proyecto al equipo.