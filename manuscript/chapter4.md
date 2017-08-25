# Habilidades IT Ops en un entorno de DevOps
Digamos que ha decidido, al menos en teoría, ayudar a llevar a su organización a una posición de DevOps. Ha leído acerca de algunas de las capacidades de alto nivel que usted, como Operador, debe proporcionar a la organización.

¿Cómo lo hace?

En una palabra, "pegamento".

Lo diré de nuevo: _DevOps es una filosofía_. La contabilidad sigue siendo un buen ejemplo. La industria de la contabilidad está de acuerdo, más o menos, en lo que constituye una buena contabilidad, y de ahí es de donde provienen los PCGA. Del mismo modo, la industria de DevOps está definiendo lentamente de que se trata un “DevOps bueno”

Pero cada organización lo hace a su manera. Observe cómo cada organización maneja su contabilidad, en detalle, y encontrará un montón de diferencias con otras organizaciones. Tal vez los auditores trabajen de formas diferentes, o tal vez un rol de trabajo diferente es responsable de diferentes funciones de contabilidad. Algunas empresas necesitan una contabilidad bastante simple, mientras que otros necesitan una contabilidad increíblemente compleja que exige cientos de personas que trabajan las veinticuatro horas del día. Aunque todos ellos operan con _los mismos principios_, sus implementaciones varían ampliamente.

Así es con DevOps.

En una organización pequeña, la contabilidad puede ser lo suficientemente simple como para que las herramientas disponibles en el mercado, como Quickbooks, sean suficientes. En ese tamaño de una organización, DevOps ni siquiera podría existir, porque una empresa de ese tamaño simplemente podría no hacer ningún "dev" para empezar. En una empresa masiva y multidepartamental, la contabilidad podría incluir herramientas "disponibles" que requieren meses y meses de personalización y ajustes. Del mismo modo, DevOps en esa misma organización podría implicar herramientas personalizadas que utilizan bloques genéricos de construcción ... y un montón de pegamento personalizado.

Proporcionar la infraestructura operacional para una organización de DevOps puede ser hacking en su mejor momento. Sí, usted encontrará un montón de productos y tecnologías disponibles en el mercado ... pero muchos de ellos sólo le llevarán hasta cierto punto en las metas de su organización. Después de eso, tendrá que hacer mucho de personalización, y poco de "pegado" de herramientas diferentes clases, además de algo de “hacking” alrededor para juntar las piezas. Probablemente siempre será así, así como todavía es el caso de nuevos despliegues de herramientas de contabilidad que por lo general toman meses y meses. Nada fuera de una plataforma podrá cubrir todas las necesidades de cada organización, por lo que simplemente tendrá que estar preparado para hacer algo de personalización, algo de hacking y un poco de pegado.

Con eso en mente, ¿cuáles son las habilidades adecuadas que se deben tener?

* Capacidad de aprender rápidamente. Tendrá que dominar nuevos productos y tecnologías sobre la marcha.

* Creatividad. Tendrá que pensar en soluciones inteligentes para evitar obstáculos. No espere que todo "funcione" - no lo hará.

* Conocimiento profundo de su plataforma(s). Ya sea que esté trabajando en Microsoft Windows, una distribución de Linux o alguna otra plataforma, necesita conocer profundamente cómo funciona, porque va a interactuar con ella a muy bajo nivel.

* Scripting. Va a necesitar ser fluido en lenguajes de programación de sistemas ("scripting") usados en su plataforma, porque ese es el “pegamento” que usará para adherir diferentes tecnologías en una solución coherente y personalizada.

Este material de DevOps no es para principiantes, ni para débiles de corazón. Es por esto que, en mi propia creencia personal, las empresas crean títulos de trabajo como "DevOps Engineer". La mayoría de la comunidad de DevOps con bastante razón se asusta por títulos de trabajo como ese, porque a menudo son una demostración de que _alguien en la organización no lo entiende_. DevOps no es un rol de trabajo. Sin embargo, en una organización que practica DevOps, hay ciertamente algunas habilidades que será muy práctico contar con ellas, especialmente en el lado de Operaciones. Alguien que posea esas habilidades podría ser llamado "Ingeniero de DevOps", que es quizás menos engorroso que "Una persona de TI que sabe lo suficiente para pegar todos esos bits de tal manera que podamos obtener las capacidades de DevOps que necesitamos". Eso sería una gran tarjeta de presentación. "DevOps Engineer" es probablemente también un título menos vergonzoso para los compañeros de trabajo que "El Chico listo de IT que necesitamos", que al final suele ser el caso.

La gente de IT Ops que trabaja para proporcionar las capacidades compatibles con DevOps es a menudo la gente más experimentada y más inteligente del equipo. Tienen más experiencia y conocimiento, y son a menudo los más ansiosos de hacer frente a este desafío.

Por cierto, fíjese cómo lo expresé. "... trabajar para proporcionar las capacidades compatibles con DevOps ..." fue una frase deliberada. Una organización que practica DevOps necesita capacidades específicas, y la parte de Operaciones proporciona algunas de ellas, en estrecha colaboración con el lado Dev. Pero esto no significa que usted vaya a tener un "Departamento de DevOps", eso no tiene sentido. "DevOps Engineer" como un título de trabajo es sólo legítimo si significa "Ingeniero que ayuda a proporcionar nuestras capacidades relacionadas con DevOps". DevOps _no es algo que  simplemente se haga_. Es algo _en lo que usted cree_ y que a su vez le impulsa a hacer las cosas. Si usted cree en DevOps, su organización necesitara comportarse de cierta manera, y necesitara ciertas herramientas para apoyar esos comportamientos.

También hay un conjunto de nuevas habilidades de desarrollo que necesitan ser introducidas en un entorno DevOps. Los desarrolladores tienen que centrarse más en que el código se pueda ser desplegado, supervisado y administrado de una manera centrada en DevOps. Por ejemplo, en la mayoría de los entornos basados en Windows, los desarrolladores suelen utilizar herramientas incluidas en Visual Studio para crear paquetes de Windows Installer. Esos paquetes no siempre han sido fáciles de desplegar de forma automatizada, porque pueden haber requerido (o se creían necesarios) privilegios de administrador u otros elementos que simplemente hicieron que el despliegue del código fuera difícil e incluso peligroso. Para "hacer" DevOps eso tiene que cambiar. Operaciones debe proporcionar a desarrollo la capacidad de desplegar el código de forma transparente en ambientes de producción, pero desarrollo necesita escribir código que admita ese modelo. La carga recae en ambos grupos, como un equipo combinado, no sólo en Operaciones.

## Plan for Failure

> "Wait a damn minute," I can hear you saying, "sliding new code into production is what causes all the problems!" 

Agreed. _Any kind of change_ has the potential to create problems. The point of DevOps - and most particularly the Operations role in DevOps - is to _create an environment where you can fail quickly, and fix just as quickly_ (thanks to Chris Hunt for that). If DevOps means constantly pushing out small bits of code, then you have to be prepared to - in Facebook's language - "move fast and break things." Eventually some release is going to be problematic, and so the role of Operations is _not to slow things down to avoid the problem_ but rather to _hit the problem hard and fast_. Virtualization, as one example, gives us the ability to rapidly "roll back" entire operating environments to a "known good state," making the prospect of failure a little less frightening. _Plan for failure_, rather than trying to avoid failure entirely.

Ask yourself if you're the type of person who routinely plans for failure. For example, on every airline flight I take, I have a set of spare clothes in my carry-on, even if that's just my computer bag. I have a small stick of deodorant, because that's an item not included in airlines' amenity packs. I _assume_ there will be a failure in the trip, and I have simple plans in place to mitigate that failure. _Few_ people take these simple steps, though, and so when failure eventually does happen, they become angry, stressed, and uncomfortable - even when the causes of failure are completely outside human control, like weather. I plan longer layovers than most people - usually 2 hours domestically - and am often able to avoid a trip failure because of that extra margin.

In a DevOps environment, you have to accept that failure will occur. Your effort should go less into preventing that failure - especially through time-consuming "gates" that put a wall between coders and users - and instead put effort into being able to iterate and recovery quickly. In a true DevOps team, a buggy release doesn't mean you roll back to the last one - it means you release another one really quickly. That's moving forward, not rolling back, and having the capability to do that is the main hallmark of a DevOps-ready organization.



