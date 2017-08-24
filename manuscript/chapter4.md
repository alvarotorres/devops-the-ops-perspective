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


This DevOps stuff is not for beginners, nor is it for the faint of heart. This is, in my own personal belief, why companies create job titles like "DevOps Engineer." Most of the DevOps community quite justifiably freaks out about job titles like that, because they're often a demonstration that _someone in the organization doesn't get it_. DevOps isn't a job role. However, in an organization practicing DevOps, there certainly are some skills that will come in handy, especially on the Operations side. Someone possessing those skills might justifiably be called a "DevOps Engineer," which is perhaps less cumbersome than "IT person who knows enough to make all these bits stick together so we can get the DevOps-enabling capabilities we need." That'd be a big business card. "DevOps Engineer" is probably also a title less demeaning to one's co-workers than "Cleverest IT Person We've Got," which is also usually the case.

IT Ops folks working to provide DevOps-compatible capabilities are often the more experienced, cleverer folks on the team. They often have the broadest experience and knowledge, and they're often the ones most eager to tackle a challenge. 

By the way, notice how I phrased that. "...working to provide DevOps-compatible capabilities..." was a very deliberate phrase. A DevOps-practicing organization does need specific capabilities, and the Operations side provides some of them, in close collaboration with the Dev side. That doesn't mean you have a "DevOps Department," because that misses the point. "DevOps Engineer" as a job title is only legit if it means "Engineer Who Helps Provide Our DevOps-Related Capabilities." DevOps isn't something you _do_; it's something you _believe_, which in turn drives you to do things. If you believe in DevOps, your organization needs to behave in a certain way, and it needs certain tools to support those behaviors. 

There are new Development skills that need to be brought into a DevOps environment, too. Developers have to focus more on building code that _can_ be deployed, monitored, and managed in a DevOps-centric way. For example, in most Windows-centric environments, developers would often use the tools bundled into Visual Studio to create Windows Installer packages for applications. Those packages weren't always easy to deploy in an automated fashion, may have required (or thought they required) Administrator privileges, and other elements that simply made deploying the code difficult and even dangerous. To "do" DevOps, that has to change. Operations needs to give Development the ability to seamlessly slide code into production - but Development needs to write code that supports that model. The burden is on both groups, as a combined team, not just on Operations to make things simpler.

## Plan for Failure

> "Wait a damn minute," I can hear you saying, "sliding new code into production is what causes all the problems!" 

Agreed. _Any kind of change_ has the potential to create problems. The point of DevOps - and most particularly the Operations role in DevOps - is to _create an environment where you can fail quickly, and fix just as quickly_ (thanks to Chris Hunt for that). If DevOps means constantly pushing out small bits of code, then you have to be prepared to - in Facebook's language - "move fast and break things." Eventually some release is going to be problematic, and so the role of Operations is _not to slow things down to avoid the problem_ but rather to _hit the problem hard and fast_. Virtualization, as one example, gives us the ability to rapidly "roll back" entire operating environments to a "known good state," making the prospect of failure a little less frightening. _Plan for failure_, rather than trying to avoid failure entirely.

Ask yourself if you're the type of person who routinely plans for failure. For example, on every airline flight I take, I have a set of spare clothes in my carry-on, even if that's just my computer bag. I have a small stick of deodorant, because that's an item not included in airlines' amenity packs. I _assume_ there will be a failure in the trip, and I have simple plans in place to mitigate that failure. _Few_ people take these simple steps, though, and so when failure eventually does happen, they become angry, stressed, and uncomfortable - even when the causes of failure are completely outside human control, like weather. I plan longer layovers than most people - usually 2 hours domestically - and am often able to avoid a trip failure because of that extra margin.

In a DevOps environment, you have to accept that failure will occur. Your effort should go less into preventing that failure - especially through time-consuming "gates" that put a wall between coders and users - and instead put effort into being able to iterate and recovery quickly. In a true DevOps team, a buggy release doesn't mean you roll back to the last one - it means you release another one really quickly. That's moving forward, not rolling back, and having the capability to do that is the main hallmark of a DevOps-ready organization.



