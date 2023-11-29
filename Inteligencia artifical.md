# Práctica 1. Introducción a la Inteligencia Artificial Actividad 1
## Ensayo 1.1 - capitulo 1, 2, 26, 27 y apartado A del libro "inteligencia artificial un enfoque moderno"
## Introducción
La inteligencia artificial es un tema que si bien se ha popularizado mucho en los últimos años su concepto y concepción del termino se remonta a varios años atrás. Desde que turing llego y formalizo el termino y dio unas reglas básicas de como funcionaria una inteligencia artificial que piensa por si misma a lo que comprendemos ahora nosotros por inteligencia artificial y las mas modernas redes neuronales que se usan hoy en día.
Este presente documento trata de dar una opinión y representación de aquello leído en los capítulos 1, 2, 26 y 27 del libro “inteligencia artificial un enfoque moderno” dado que si bien existe una gran cantidad de documentación al respecto la gran mayoría de los mismos esta algo desactualizado o presenta un enfoque algo desactualizado por lo que es importante profundizar en el tema desde un enfoque un poco mas actual.
El capitulo 1 presenta una introducción al tema en el cual se abarcara los conceptos generales acerca de la inteligencia artificial, los fundamentos en los que se basa y la historia del origen propio del mismo. El análisis de ese apartado se limitara a los puntos mas importantes a considerar sobre el tema.
El capitulo 2 del libro abarca al concepto de agentes inteligentes que ya es una consideración mas especifica acerca de agentes automatizados que trabajan sobre su propio entorno siendo de las bases mas sencillas para comprender a las inteligencias artificiales.
El capitulo 26 abarca los fundamentos filosóficos comprendidos por como es que consideramos que piensa el ser humano, si una inteligencia artificial seria capaz de replicar este tipo de pensamiento y diversos experimentos que dieron tanto argumentos a favor como en contra para la definir si era posible crear una inteligencia artificial que actuara con libre albedrío.
El capitulo 27 del libro trata sobre el estado presente de las IA y cual puede ser su posible futuro con una mejor potencia tecnológica, pero sin dejar de lado el aspecto psicológico que podría repercutir en la vida del hombre crear una maquina capaz de pensar por si misma y si debería ser esto algo que nos debería de preocupar o no.
Finalmente el apartado A del libro que es la ultima parte que se analiza trata mas sobre los fundamentos matemáticos siendo estos vectores, problemas NP, matrices, entre otras características que se abarcaran a su debido tiempo.

## Desarrollo
Como se menciono en la introducción la IA es una ciencia relativamente reciente, el inicio de los trabajos propios de aquello que conocemos como una inteligencia artificial inicio poco después de la segunda guerra mundial siendo el termino acuñado en el año de 1956. La IA hoy en dia sintetiza y automatiza tareas intelectuales y es, por lo tanto, potencialmente relevante para cualquier ámbito de la actividad intelectual humana considerándose casi “universal”.
Si nos ponemos a pensar acerca de que fue lo que en sus inicios mas marco a lo que hoy conocemos como inteligencia artificial sin duda lo primero que nos viene a la mente es el famoso test de Turing creado por Alan Turing en 1950, este se diseño para proporcionar una definición operacional y satisfactoria para el concepto de inteligencia aplicado a las maquinas. Este test se basaba en que dadas una serie de preguntas pudiera identificarse si aquel con el que estábamos manteniendo la conversación era una persona o una computadora, en caso de no identificar a la maquina esta pasaría el test de Turing.
Hoy en día consideramos que para aprobar el test de Turing un computador debería de poseer las siguientes capacidades:
-Procesamiento de lenguaje natural.
-Representación del conocimiento.
-Razonamiento automático.
-Aprendizaje automático.
Y aun con la información y datos anteriores existen distintas variantes acerca de lo que consideramos una IA, empezaremos hablando del enfoque del modelo cognitivo que podría equivaler a “pensar como un humano”, podemos decir que un programa piensa como un ser humano cuando primero somos capaces de determinar como piensa realmente un humano. Para esto es que se creo un campo interdisciplinario que se conoce como ciencia cognitiva en el cual convergen los modelos computacionales de IA y técnicas experimentales de psicología intentando elaborar teorías precisas y verificables sobre el funcionamiento de la mente humana.
Por otro lado tenemos el enfoque racional o aquello que se le conoce como “leyes del pensamiento”, esto viene a tratar de construir sistemas inteligentes a partir de programas “lógicos” por medio de notación lógica. Este enfoque si bien mas desarrollado presenta el inconveniente de que no siempre se puede transformar el conocimiento informal para expresarlo en los términos formales que ocupa la notación lógica.
Un enfoque mas aceptado y que presento un mayor grado de desarrollo es el enfoque racional o de agentes racionales, en principio un agente racional es aquel que actua con la intención de alcanzar el mejor resultado o, cuando hay incertidumbre, el mejor resultado esperado. En el caso de la IA todo el énfasis de este enfoque se basa en hacer las inferencias correctas dependiendo de la situación que se le presente y es este enfoque el que mas desarrollo ha tenido en los últimos años.
Dado la información anterior es importante definir lo que se entiende por agente siendo este cualquier cosa capaz de percibir su medioambiente con al ayuda de sensores y actuar en ese medio utilizando actuadores. En general, un agente tomara una decisión en un momento dado dependiendo de la secuencia completa de percepciones hasta ese instante esto en base a lo que matemáticamente se conoce como la función del agente.
Si profundizamos un poco mas en este concepto de agente racional caemos que es aquel que hace lo correcto, cada elemento de la tabla de situaciones que define la función del agente se tendría que rellenar correctamente, pero para ello tenemos que definir que es eso que se considera “correcto”. Para ello es que se hace la inclusión de un nuevo concepto siendo este las medidas de rendimiento que incluyen los criterios que determinan el éxito en el comportamiento del agente y podemos decir que como regla general es mejor diseñar medidas de utilidad de acuerdo con lo que se quiere para el entorno, mas que de acuerdo con como se cree que el agente debería de comportarse.
Todo lo anterior suena muy bien y parece que el sentido de racionalidad solo nos ayuda a entender mejor a las inteligencias artificiales pero hay que tener cuidado dado que la racionalidad a veces se llega a confundir con la omnisciencia. Un agente omnisciente conoce el resultado de su acción y actuá de acuerdo con el; sin embargo la omnisciencia no es posible dado que nunca se puede alcanzar la perfección en los resultados. Por su lado la racionalidad busca maximizar el rendimiento esperado a diferencia de la perfección que busca maximizar el resultado real.
Ahora que se tiene una definición de la racionalidad hay que centrarnos en la naturaleza del entorno que son esencialmente los “problemas” para los que los agentes racionales son las “soluciones”. En este caso se tiene lo que se llama el entorno de trabajo, para cuya denominación se utiliza el acrónimo REAS (Rendimiento, Entorno, Actuadores, Sensores). En el diseño de un agente, el primer paso debe ser siempre especificar el entorno de trabajo de la forma mas completa posible. El rango de los entornos de trabajo en los que se utilizan técnicas de IA es obviamente muy grande. Sin embargo, se puede identificar un pequeño número de dimensiones en las que categorizar estos entornos. Estas dimensiones determinan, hasta cierto punto, el diseño más adecuado para el agente y la utilización de cada una de las familias principales de técnicas en la implementación del agente.
Ya con las bases bien fundamentadas considero conveniente empezar a trabajar un poco mas en las definiciones de las propias IA que en sus partes dado el contexto que nos atañe, si recordamos las consideraciones iniciales establecidas al inicio de este ensayo se recordara que entre los primeros problemas que presentaba la propia definición es cual era los limites de la IA en cuanto a su capacidad. Bueno es para esto que se crearon dos conceptos que iniciaron un conflicto entre aquellos que trabajaban en el área siendo estos la IA débil y la IA fuerte. La mayoría de los investigadores dan por sentado la hipótesis de la IA débil como la afirmación de que es posible que las maquinas actúen con inteligencia (simulándola) mientras un grupo mas reducido aun les interesa el concepto de IA fuerte como la afirmación de que las maquinas si son capaces de pensar realmente por su cuenta.
Este tipo de problemas depende del nivel de profundidad y estilo que le damos al problema, si nos enfocamos por el lado matemático nos encontramos con problemas como el argumento de la informalidad (siendo este la incapacidad de capturar toda la información en un conjunto de reglas lógicas como un problema de cualificación) mientras si nos enfocamos un poco mas en el lado psicológico del problema nos encontramos con cosas como el experimento de la habitación china que defiende que si bien una maquina se le pueden programar los estados posibles para reaccionar ante todas las situaciones que pueda encontrar esta solo estará actuando en base al conjunto de instrucciones y no estará siendo “inteligente” de verdad al no tomar “decisiones”.
Estas consideraciones acerca de si las IA en realidad son capaces o no de pensar con libertad paso de ser una idea alentadora a algo que le provoco pesadillas a mas de uno, esto principalmente porque muchas de las nuevas tecnologías han tenido efectos negativos no intencionados y la gente suele preocuparse principalmente por los siguientes problemas al trabajar o tratar sobre la IA:
-Las personas podrían perder sus trabajos por la automatización.
-Las personas podrían cuestionarse su existencia al crear algo capaz de pensar como un ser humano.
-La utilización de los sistemas de IA podría llevar a la perdida de responsabilidad ya que dejaríamos a las maquinas hacer “todo”.
-Y la que es la favorita de muchos, el éxito de la IA podría significar el “fin de la raza humana”.
Algunas consideraciones que se hacen respecto a la IA tienen sentido la preocupación pero otras claramente son simples exageraciones de las personas que no conocen a profundidad acerca del tema. Lo que tiene que ver con el trabajo y la responsabilidad no es algo que dependa de la IA es una cuestión que depende del hombre mismo si este decide hacerlo o no es parte de su naturaleza no culpa directa de la aparición de la IA.
Por otro lado las ideas acercas del fin de la raza humana tiene un problema fundamental, dado que la forma en que se programan las IA son para que piensen como humanos no como maquinas por lo que al adquirir conciencia seria como una persona mas y no buscaría el fin de la humanidad si ella misma se considera a si misma parte de la misma.
Conociendo toda la información anterior podemos empezar a hablar sobre el presente de la Ia y su futuro, hoy en día la IA ha hecho posibles aplicaciones nuevas tales como sistemas de reconocimiento de voz, sistemas de control de inventarios, sistemas de vigilancia, robots y motores de búsqueda. Con lo anterior parece probable que un éxito en IA a gran escala cambiaría las vidas a una mayoria de la humanidad. La verdadera naturaleza del trabajo y el papel de los investigadores de IA cambiaría así como nuestro punto de vista sobre la inteligencia, la consciencia y el propio destino futuro de la raza humana.

## Conclusiones
Con todo lo anterior creo que tenemos un vistazo general al impacto y la importancia que tienen hoy en día las IA desde su concepción a lo que podrían llegar a ser en un futuro. Es evidente como estas son cada vez mas relevantes en la industria y la sociedad en si conforme mas avanza el tiempo y es por ello que se considera importante el analizar este tipo de cuestiones para tener una idea mas amplia acerca de lo que las IA representan para la humanidad.
Siempre es curioso como un campo tan tecnológico de la industria humana llega a estar tan entrelazado con los aspectos psicológicos del ser humano, siendo que las mejores IA son las que mejor replican lo que la psicología demuestra que se considera pensamiento a la hora de tomar decisiones. Las consideraciones acerca de lo que fue, lo que es y aquello que puede llegar a ser la IA es un tema que siempre estará vigente conforme se desarrolla cada vez mas estas tecnologías. Creemos que si acaso falto realizar un análisis mas profundo a lo que es el fundamento matemático de las IA pero dado la temática del ensayo se considero que lo mejor era presentar solo las partes mas importantes de las “generalidades” necesarias para que cualquier lector fuera capaz de entender lo que una IA es.
Con esto no queda mas que concluir el trabajo recordando que al igual que cualquier tecnología depende del propio ser humano el como sera que esta progrese, si se usara para el bien o para el mal y que es lo que sera de nosotros en un futuro debido a la implementación de la misma.


## Ensayo 1.2 - sobre el documental sobre IA
## Introducción
El presente ensayo trata sobre la inteligencia artificial vista desde el punto de vista expuesto por el documental “Inteligencia Artificial” que nos otorga Discovery cannel en colaboración con IBM, la cual es una pionera en el desarrollo de esta ciencia. Principalmente el documental nos presenta los distintos ámbitos en los que la IA ha tenido una mayor relevancia, ademas de distintas aplicaciones como es el caso de los juegos de estrategia, la conversación, la industria, la educación y la salud. Por otro lado, abarco como la inteligencia general puede ser un avance para el desarrollo de dicha tecnologia. Considero que es importante conocer las aplicaciones más importantes que ha logrado ademas del futuro que la IA puede llegar a desarrollar.

## Desarrollo
La inteligencia artificial es un tema con una amplia variedad de puntos de vista asi como informacion acerca de la misma, siendo un tema que ha sido tratado incluso por la conocida compañía de televisión Discovery Channel, la cual se dedica, entre otras cosas, a la presentación y realizacion de documentales acerca de diversos temas científicos y sociales con mayor impacto en la actualidad. El documental que desarrollaron en esta ocasión abarca el tema de la inteligencia artificial, considero que el enfoque presentado en dicho documental tiene multiples cosas en comun  con el libro “Inteligencia artificial: un enfoque moderno”. 
El documental fue realizado con la colaboración de IBM, una de las empresas de cómputo y tecnología más importantes y antiguas que existen. El eje central del documental es que la inteligencia artificial no solo es una tecnología o una sola técnica, si no que se basa en diversas técnicas que se pueden aplicar para que un agente pueda aprender, como por ejemplo esta el procesamiento de lenguaje natural o de imágenes por medio de una computadora. Una inteligencia es considerada como artificial cuando no se trata de un ser biológico y es aquella que puede o debe  tener entradas y salidas de información y a la vez contar con capacidad de tomar decisiones para resolver problemas. 

**La inteligencia artificial empleada en trivias** 

El primero de los ejemplos de una aplicacion real de la inteligencia artificial por parte del documental es Watson, la inteligencia artificial creada por IBM, nos muestra como en sus inicios esta fue diseñada para que intentara competir en el juego de televisión Jeopardy, el cual consiste en presentar una definición o un concepto y que los concursantes tengan que contestar en forma de pregunta la palabra clave a la que pertenece dicho concepto. Se puede observar que al principio Watson no era capaz de contestar de forma correcta las preguntas, pero luego de realizar varias sesiones de entrenamiento y haber adquirido un enorme conocimiento de libros con temas de los que se empleaban en el juego, finalmente fue capaz de contestar la mayoría de las preguntas correctamente, haciendo consultas muy rápidamente y ganando con mucha superioridad el concurso. Podemos observar como en base al conocimiento que una inteligencia artificial posee, esta va llegando a mejores conclusiones, pero además emplea la probabilidad para aproximarse a las mejores respuestas, como seria el caso de los debates, donde se van presentando puntos de vista basados en los conocimientos previos que las personas tienen acerca del tema en cuestion y en base a esto se llega a una conclusión sobre si cual de las dos posturas acerca del tema es mas solida.

**La IA en un debate** 

El siguiente ejemplo presentado por el documental sobre la aplicación de la inteligencia artificial se trata de un debatiente que es una máquina capaz de escuchar las afirmaciones de la oposicion y consultar todos los conocimientos que tiene en base a diversos documentos registrados en su memoria, algo llamatico en esta ejemplo es que podemos apreciar que la capacidad de un ser humano de entender su propio lenguaje es naturalmente sencillo, pero en contraparte las maquinas tienen que hacer uso de mucha más capacidad de memoria en relacion a la información que pueden consultar para generar sus respuestas, cuando una maquina es capaz de hacer uso del procesamiento de lenguaje natural consigue incluso comunicarse con una o varias personas, siendo este el caso del debate en el que una de las debatientes es una mujer que argumenta en contra del tema de legalizar las apuestas deportivas, mientras que aquel a favor es la inteligencia artificial que conforme va a aprendiendo más, consulta más información para poder contestar a los argumentos que la mujer dice y llegar a ser capaz de ganarle usando incluso carisma.

**Los automóviles autónomos por medio de IA** 

El siguiente caso presentado por el documental es algo que siempre hemos escuchado acerca del futuro "los autos que se manejan solos", dentro de este tema nos presentan que durante muchos años se ha estado trabajando en el desarrollo de los famosos automóviles autónomos, los cuales como su nombre lo indica no necesitan de un conductor humano debido a que tienen la capacidad de ser manejados por un programa de inteligencia artificial, sin embargo como es natural tienen sus limitaciones, podemos ver que nos explican como esto puede conllevar varios riesgos como accidentes y pérdidas de vidas aunque estos accidentes ocurren igual con conductores humanos, la mayoría de los ejemplares de inteligencia artificial se desarrollaron sabiendo que se equivocarían muchas veces y no habrían consecuencias graves al ser probados en un entorno controlado, sin embargo al referirnos a los carros autónomos entonces si es un tema mas delicado, algo importante que considero importante destacar aquí es que para una persona es muy fácil comprender la subjetividad y la inestabilidad de como suceden las cosas en el mundo real a la hora de estar al volante, ya sea por experiencia propia, emociones individuales o simple sentido común, sin embargo para una maquina esta percepción es más rígida y necesita tener un aprendizaje fuertemente sólido basado en multiples entradas de datos. Por lo que incluso se nos informa que aunque si es posible realizar este avance tecnológico, le tomará muchos años para poder concretarse dependiendo del progreso de la IA y de las tecnologias que hacen posible su funcionamiento.

**La IA en los videojuegos y su uso en redes sociales** 

La inteligencia artificial tambien cuenta con diversas aplicaciones en el ámbito de los juegos y principalmente en los videojuegos, una de las mas conocidas es el juego de damas inglesas, tal como nos muestra IBM que creo su IA llamada DeepBlue, la cual mostró una gran habilidad para jugar juegos de estrategia por turnos como las damas, siendo capaz de vencer al mejor jugador humano en una partida luego de multiples sesiones de entrenamiento. otro ejemplo de esto es el de Go zero, una IA capaz de jugar un juego oriental llamado Go, el cual nos dice que tiene más posiciones o combinaciones en su tablero que el número de átomos en el universo, que es algo inimaginable, pero esta IA logra aprender los patrones para poder llegar a obtener su objetivo con la ruta más corta, es decir, con el menos número de movimientos posibles que es uno de los principales requerimientos que se tiene para ganar en este juego. De esta manera se nos muestra que no solo la IA es capaz de decidir de la forma más acertada sus jugadas, si no que es capaz de llegar a esa decisión de la forma más rápido y de realizar sus actividades de la forma más óptima posible. Otro aspecto en el que se ha aplicado la IA es en las redes sociales como bien son ejemplos Facebook, twitter y redes de música como spotify, en donde la plataforma aprende los patrones que más repite el usuario y le va mostrando información más acercada a sus tendencias que se va actualizando conforme el usuario use mas la aplicacion.

**La IA aplicada en los trabajos** 

Una de las areas mas controversiales en lo que inteligencia artifical se refiere es a las cuestiones laborales, por un lado existe ese temor de una cantidad considerable de personas de que puedan perder sus trabajos y ser reemplazados por una IA, pero por el otro también es importante tomar en cuenta que es una herramienta que se creó con el objetivo principal de ayudarnos no de perjudicarnos o reemplazarnos, uno de los puntos importantes al defender a las IA en este aspecto es que existen muchos trabajos donde se llevan a cabo tareas muy repetitivas e incluso peligrosas, y es principalmente en estos escenarios en donde se le puede sacar un mejor provecho a la IA, el documental nos muestra el ejemplo de un robot, Soyer, el cual se usa para cortar y perforar piezas de madera en un lugar de trabajo, mientras el personal humano le va enseñando la forma en que tiene que hacer sus actividades, de alguna manera vemos que es necesario el apoyo humano para que la IA pueda hacer su trabajo correctamente siguen dependiendo de nosotros y la vez esta no se cansa de llevar a cabo actividades que pueden ser tediosas para una persona,  una maquina solo necesita de su fuente de energía y sigue funcionando, a su vez, puede haber otra oportunidad de trabajo para la persona que ha sido reemplazada por esta atendiendo la propia maquina o sirviendo de apoyo. 
En el ejemplo mencionado en el documental la IA demostro su aprendizaje ya que por medio del entrenamiento pudo guardar los movimientos que la persona la iba mostrando para repetir esas acciones y realizar su trabajo, en este caso parece que las entradas fueron patrones de movimientos del cuerpo que leugo fueron empleadas en la máquina. Si la IA tiene la capacidad de aprender entonces podria desarrollar la capacidad de enseñar. La IA ya ha sido empleada como una herramienta de apoyo en el ámbito de la educación, el ejemplo de la aplicación que se le dio a Watson para poder enseñar a los niños en sus primeros 8 años de vida, hasta ser un compañero de apoyo para estudiantes mayores como los universitarios, un ejemplo de esto es la conocida herramienta de chat GPT, el cual en base a sus conocimientos sobre multiples fuentes de informacion escrita le permite ser una herramienta de consulta rápida de información que puede servir de apoyo para muchos estudiantes y trabajadores, aunque depende de la manera en que estos la utilicen y sobretodo, pienso que se debe de usar como una herramienta para enriquecer el conocimiento que ya tenemos, además de resolver el problema que se nos presente, y además de resolver alguna tarea más rápido, podamos aprender más rápidamente no depender unicamente de ella. 
Como herramienta de apoyo, se plantea que por otro lado la IA puede ser una compañera para personas con discapacidades como por ejemplo los invidentes, el documental nos muestra otro ejemplo de un hombre llamado Simon que padecía de una enfermedad de la retina, la cual ocasionó que perdiera la vista, pero él queria ser lo más independiente posible de otras personas, la solución que encontro a esto fue un brazalete que usaba la aptica, una avanzada tecnología que hace uso de la comunicación por el sentido del tacto, el dispositivo con IA que utilizó para apoyarse era la wayband, la cual le ayudaba por medio de señales apticas a mantenerse corriendo o caminando por el camino correcto, a su vez, este hacía uso de datos como las rutas trazadas por el gps y la comunicación por internet, en este caso podemos ver como la inteligencia artificial está nutrida por los datos y estos a su vez deben ser útiles dentro del contexto en el que se pretende solucionar un problema dado, en el ejemplo presentado poder trazar un camino y comunicarse con una persona que no cuenta con la capacidad de ver.

**La percepción de la IA y la privacidad de la gente** 

En la actualidad las máquinas que emplean el uso de inteligencia artificial ocupan disponer de dispositivos en los que puedan recibir multiples entradas de información dependiendo del contexto en que se empleen como se menciono anteriormente, para tener un "oído" usan micrófonos, para tener una "voz" emplean un altavoz, para una "vista" una cámara y para una especie de "tacto" emplean algún tipo de sensor. Con este tipo de características una maquina es capaz de percibir objetos o personas dentro del entorno en el que esta se encuentre, en el documental se nos presenta el ejemplo en el que la IA haciendo el uso del procesamiento de la imagen con la cámara es capaz de detectar los rostros de las personas, esto debido a que todas las personas comparten características similares en sus rostros, todos tienen dos ojos normalmente, una nariz y una boca distinguibles. Al ser capaces de detectar los rostros de las personas se crearon una cantidad considerable de aplicaciones.
El documental nos habla de que en China se usó una IA para detectar a posibles criminales con solo observar su rostro muy de peliculas la verdad, esto basado en los patrones o características que se presentan en los rostros de personas que han cometido delitos, sin embargo, se nos especifica que esta característica también puede afectar a la privacidad de la gente, es un tema que no es reciente ya que desde antes de las propias IA la privacidad en cuanto a lo que hacemos siempre ha sido cuestionada por cada nueva tecnologia que rastrea nuestras actividades, se podría plantear que debe existir un equilibrio entre la privacidad y la eficiencia pero siendo sinceros la linea que determina que tanto estamos dispuestos a permitir es muy delgada y varia de persona a persona. 
Es cuanto menos llamativo como una maquina es capaz de procesar las imágenes que percibe en forma de matrices de datos numéricos en intervalos de tiempo tan cortos, además de que en el ejemplo anterior se nos menciona que se usan cámaras de video, o sea que hablamos del procesamiento de miles y miles de fotogramas por segundo a mas de un objeto a la vez, esto también resalta la enorme capacidad de procesamiento de información y almacenamiento con la que cuenta dicha tecnologia.

**La inteligencia artificial en la rama de la salud** 

Abarcando el tema de la salud de las personas  se nos muestra un ejemplo en el documental de su aplicación en la que un hombre que padece de parkinson, una enfermedad asociada al movimiento de las articulaciones, se le desarrollo una IA que tiene como iniciativa poder ayudar a personas con situaciones similares a la suya, algo importante que podemos denotar en esto es que la IA a la que se recurre es Watson  la IA de IBM vista con anterioridad pero ahora aplicada al ámbito de la salud, específicamente hacia la enfermedad del parkinson, se presenta como la IA tiene un conocimiento sobre dicha enfermedad y entonces rápidamente puede hacer una recomendación de los fármacos que le pueden servir a cada persona en base a los datos que tenga el sistema de cada uno de los pacientes.
Dicha IA es presentada como una herramienta compañera para los médicos y los enfermeros a quienes se les puede presentar la situación de que necesitan consultar algún medicamento o sustancia que las ayude si por ejemplo se encuentran en una situación de emergencia o incluso alguna operación de un paciente, en este tipo de situaciones el tiempo es una variable e importante ya que puede marcar la diferencia entre la vida y la muerte, por otro lado, cconsidero que en cuestión de los pacientes puede ser una compañera de apoyo para cuando se quieren rehabilitar o para poder llevar correctamente sus tratamientos, como seres humanos, siempre tendemos a ser muy variables y a equivocarnos en la precisión para las cosas que hacemos, como seguir un plan de recuperación por ejemplo o llevar el control de las medicinas que nos tocan a diversas horas.

**La singularidad y la inteligencia general** 

El último apartado que el documental presenta es acerca de cómo puede llegar a ser posible la súper inteligencia artificial conocida como singularidad y cual es la inteligencia que las personas tenemos, la inteligencia general, siendo esta es la capacidad de saber actuar en cualquier tipo de situación o entorno y entenderlo a la vez, hoy en dia las IA modernas carecen de dicha capacidad pero se teoriza que si le damos esta capacidad a la inteligencia artificial entonces esta podría crecer de manera exponencial y convertirse en lo que se llama una singularidad o súper inteligencia artificial, se nos plantea que si llegara a existir un ejemplar de la misma esta sería construida a partir de otra inteligencia artificial ya existente en vez de por humanos, lo cual tiene mucho sentido porque una IA es capaz de ir evolucionado al punto de ser ya tan avanzada que incluso tenga la capacidad de crear a otra, otra que incluso pueda superar a nuestra propia inteligencia al no contar con los limites que nosotros le establecemos a las IA actualmente. 
Pero aun con lo anterior yo considero que un factor que debería de existir para dicho escenario sea posible es que nosotros seamos capaces de entender el origen de nuestra conciencia, el misterio que se encuentra encima de esta de donde inicia realmente el pensamiento, considero que solo de esa manera podriamos llegar a entender esto y de alguna manera dotar a la IA de algun tipo de conciencia para que entonces esta sea capaz de superarnos o por lo menos llegar a nuestro nivel de conciencia o autopercepción. Este último tema es bastante interesante y creo que también plantea una premisa de lo que podría ser un próximo paso clave para una mayor evolución de la inteligencia artificial en los próximos años a la vez que presenta uno de los mayores temores de muchas personas que es las maquinas rebasandonos.

## Conclusiones
La inteligencia artificial ha sido considerado por muchas personas como una amenaza para diversos trabajos e incluso algo que podría reemplazarnos como la especie dominante en el planeta, sin embargo, es importante siempre recordar que esta es desarrollada como una herramienta que debe servirnos como un apoyo, y que a su vez esta recibe el apoyo humano para desempeñar mejor sus tareas, estando aun lejos de ser capaz de autodirigirse. 
Considero que depende de nosotros emplearla como una herramienta para que tenga un buen crecimiento y a la par esta contribuya a que nosotros seamos personas mas productivas y de alguna forma podemos cuidar otros aspectos que nos ayuden a estar mas saludables ya que por ejemplo muchas veces el trabajo puede consumirnos y esto es algo que a una maquina no puede afectar. 
Como podemos observar, en un equipo de trabajo siempre existen miembros con distintas cualidades, si logramos trabajar en equipo con la inteligencia artificial esta puede beneficiarnos en gran medida como lo esta haciendo ya hoy en dia, el ser humano tiene la cualidad de tener una conciencia sobre sí mismo pero no tiene tanta resistencia al trabajo y además es frágil ante tareas peligrosas, por su parte, las máquinas no tienen conciencia de sí mismas  pero pueden soportar largas jornadas de trabajo sin verse agotadas o aburridas evitando asi el riesgo de tener accidentes en algún momento, considerando el tema desde este punto de vista es facil el darnos cuenta de que podemos colaborar como un equipo con la inteligencia artificial si sabemos aprovecharla adecuadamente, sin necesidad de verla como una competencia o como una amenaza, ya que depende de nosotros en que se convertira y para que sera empleada, una vez mas la verdadera amenaza no seria la propia IA sino los hombres detras de la misma.


# Práctica 2: Ensayo. Introducción a la Inteligencia Artificial: Tipos de Inteligencia.
## Teoría de las Inteligencias Múltiples de Gardner

## Introducción
El presente ensayo trata sobre el tema de los tipos de inteligencias que el psicólogo Howard Gardner mencionó en contraparte de la idea de que la inteligencia es única y puede abarcar todas las habilidades. Para el tema de la inteligencia artificial es importante conocer los tipos de inteligencia que pueden tener las personas para tener un amplio punto de vista y comprender que muchas veces es un error el generalizar y catalogar a alguien o algo como inteligente o no inteligente, solo por el hecho de tener o no una habilidad en específico, siendo un ejemplo claro las situaciones que se presentan en la escuela.
Se tratara de enfatizar principalmente en los conceptos generales de la inteligencia y abarcara un poco de informacion acerca de como resulta el aprendizaje para los distintos tipos de inteligencia.

## Desarrollo
De acuerdo con el punto de vista establecido por Gardner, la inteligencia no es una sola, si no que es probable que existan diferentes tipos de inteligencia para diferentes contextos de la vida. Basado en lo que se ha hablado anteriormente sobre la inteligencia artificial, el objetivo principal de dicha inteligencia es resolver problemas en distintos contextos como por ejemplo las ciencias sociales, el arte, o la lógica pueden existir diferentes tipos de inteligencias para cada uno. 
Gardner menciona que existen diversos tipos de inteligencia que podemos considerar como la inteligencia lingüística verbal, la inteligencia física kinestésica, la inteligencia lógico matemática, inteligencia espacial, inteligencia musical, inteligencia interpersonal, inteligencia intrapersonal, aunque también se pueden considerar otros tipos como la naturalista, espiritual y existencial. Cada una de las inteligencias mencionadas se enfoca a diferentes situaciones y esto cobra mayor sentido dado que en muchas ocasiones en la escuela observamos que el alumno más listo en una escuela no siempre es el mejor compañero que te pueda brindar apoyo emocional, si bien dicho alumno con alta inteligencia racional puede ser consciente de cómo funcionan los sentimientos y emociones humanas, en la mayoría de las ocasiones no podrá interpretar adecuadamente la situación de la otra persona, es aquí donde entra la importancia de que Gardner categorice la inteligencia en las que mencionamos anteriormente siendo para este ejemplo mas importante la inteligencia emocional para brindar dicho apoyo emocional. 
Algunos otros ejemplares que Gardner menciona en su libro “La inteligencia reformulada. Las inteligencias múltiples en el siglo XX”, nos habla de que existen otras 3 inteligencias, la naturalista, espiritual y existencial. Estos ejemplos representan a algo más filosófico y humanista, el percibir el mundo en sus plantas y animales, las cuestiones de las cosas en las que cree el ser humano para su crecimiento y bienestar o, mejor dicho, bien actuar, y por otro lado la parte de llegar a su bienestar por medio de llegar a un estado mental de calma siendo conceptos de inteligencia un poco mas complejos de aplicar o probar.
Entre las diversas inteligencias la inteligencia lingüística verbal se enfoca principalmente en la parte de la comunicación como las palabras que se dicen y de alguna forma moldearlas para que estas puedan ser interpretadas de diferentes maneras, es decir, el significado que las palabras adquieren con el tono y organizadas en una oracion. Muchas personas como escritores, mangakas, novelistas y guionistas presentan este tipo de inteligencia y logran conectar con otras personas a través de esta. Un ejemplo conocido relacionado a la IA es el procesamiento del lenguaje natural por parte de la maquina como es chatgpt, en el que la maquina puede leer e interpretar textos de diferentes naturalezas sin necesitar un lenguaje propio de computadora o un compilador. 
Otro caso es el de la inteligencia lingüística kinestésica que según lo que menciona Gardner, son las personas que pueden interpretar el lenguaje de los sordomudos, muchos gimnastas artísticos, etc. Un ejemplo interesante en la inteligencia artificial serían los robots mecánicos que desde su programa de agente logran enviar señales a los actuadores, que serían como sus extremidades, que según el movimiento que necesitan realizar para llevar a cabo una tarea se ejecuta de forma adecuada. 
Gardner menciona también otros tipos de inteligencia más apegadas al aspecto humano, como la inteligencia interpersonal y la intrapersonal, siendo la primera la forma en la que un individuo puede entender las emociones y los sentimientos de otras personas y de esa manera sabe cómo responder o que decisiones tomar para lograr los mejores resultados y resolver una situación de esa naturaleza, por otro lado la intrapersonal es muy similar pero esta vez el individuo se puede comprender a sí mismo y tomar las mejores decisiones para sí mismo. 
Otra de las inteligencias mas conocidas es la inteligencia matemática la cual es la capacidad de manejar números y realizar todo tipo de análisis y operaciones con ellos, en este caso, es uno de los ejemplos más básicos relacionado a las maquinas que emplean la IA, debido a que los datos con los que trabajan las maquinas son principalmente números, de hecho, la base de las señales que trabaja un computador son pulsos eléctricos interpretados como 0 y 1, por lo que cobra bastante sentido. 
Pasando al tema de la inteligencia espacial esta es aquella que se relaciona con la parte de la vista o el procesamiento de las imágenes, los colores, las formas, etc. Por otro lado, la inteligencia musical es aquella que está más relacionada con la parte auditiva, aquí podemos mencionar parámetros como los tonos, frecuencias, tiempos y ritmos. 
Estas inteligencias que menciona Gardner considero que son mas importantes de lo que uno usualmente considera, las he visto en varios libros de auto ayuda y son muy mencionadas sus diversas características, francamente no había leído o escuchado sobre estos nombres de inteligencias fuera de la matematica y emocional. Desde mi punto de vista, este tipo de inteligencias más modernas que el mismo autor nos menciona dan un acercamiento a la conciencia del ser humano sobre sí mismo, su mente y son enfoques mas especializados que quizas en tiempos no tan modernos no se tenian contempladas. 
Otro aspecto importante que se nos menciona es el de la superdotación en las inteligencias que es donde las capacidades intelectuales es muy alta, sin embargo, la falla que se encuentra aquí es que, si una persona fuera muy inteligente en una de las inteligencias mencionadas, esta tendría desbalances en las demás ya que no siempre se puede contar con todas a la vez o siempre se encuentran carencias al tener una de las mismas mejor desarrolladas. Este tema me hace considerar en que sería algo muy idealista el considerar que una persona o entidad pueda poseer simultáneamente todos los tipos de inteligencias y además tenerlas en un nivel de superdotación, sería algo muy cercano a la perfección que no se ha visto en ninguna persona que ha vivido hasta la fecha.

**El aprendizaje**

Otro aspecto importante que menciona Gardner es que la inteligencia de una persona depende principalmente de la manera en que esta absorbe o recibe la información, sin importar la forma. La información sobre música comúnmente no la recibimos como la espacial o como a matemática, de hecho, hay muchas personas que tienen un sentido más desarrollado que otro como aquellos musicos que tienen mas afinado el oido o tiradores que tienen mas desarrollada la vista. El otro punto importante que pude ver es que también cada tipo de inteligencia es autónoma, es decir, se desarrolla de forma independiente, uno no puede desarrollar inteligencia emocional y matematica a la vez ya que la informacion que ocupara para desarrollar cada una es completamente diferente. Gardner nos menciona que el cerebro humano se divide en distintos sectores que se enfocan en diferentes habilidades cada uno y es lo que nos permite tener y aprender diversos tipos de inteligencia.

## Conclusiones
La inteligencia que podemos notar que poseen las personas siempre se enfoca en algún aspecto especifico de un area de conocimiento, o se apega a alguno de los tipos de inteligencia que menciona Gardner vistos en el ensayo. Si tratamos de considerar todo lo anterior expuesto desde el punto de vista de las máquinas y especificamente para la inteligencia artificial, esto nos ayuda a entender que esta ciencia tiene muchas variantes y se especializa en resolver diferentes tipos de problemas en base a las inteligencias que se contemplan actualmente para el desarrollo de los modelos. La inteligencia artificial no está basada en un único y absoluto tipo de inteligencia y hay ocasiones en los que necesitamos trabajar con textos, con imágenes o con sonidos  por lo que puedo afirmar que la teoría de Howard Gardner se aplica muy bien y nos sirve para entender los multiples aspectos intelectuales que se utilizan a la hora de desarrollar las IA.


# Practica 3 Introducción a la inteligencia artificial Introspección
## Introducción
Este ensayo aborda el tema sobre resolver un desafío, el cual consiste en intercambiar la posición de 4 alfiles blancos y 4 negros que se encuentran en la primera y última fila respectivamente en un tablero de ajedrez de 5 x 4, la idea es interpretar la solución desde el punto de vista introspectivo. La importancia de este ensayo radica en conocer o tener un mejor entendimiento del proceso cognitivo y de resolución de problemas que tiene la inteligencia artificial conociendo el que tenemos los seres humanos, la inteligencia artificial pretende funcionar de la misma manera que la inteligencia natural del ser humano, que hasta el momento es el ser vivo con la máxima capacidad de utilizar la misma y además ser consciente.

## Desarrollo
**Percepción y análisis del problema.**
El problema que se presenta es un tablero similar al del ajedrez, pero en una versión más pequeña. En primer lugar, lo que hago es observar el tablero que tiene 5 filas y 4 columnas, la primera y la última fila son las únicas que tienen alfiles, la primera tiene 4 ejemplares blancos y la segundo a su vez tiene 4 ejemplares negros. Después de observar el tablero lo que hago es deducir que al alfil solo puede realizar movimientos en forma diagonales como en el juego tradicional de ajedrez, por lo que la única manera de cambiarlos de posición es llevándolos en pasos con forma de diagonal. Las diagonales como en el juego tradicional, pueden ser de 2 a n cuadros, claro que tomando en cuenta la medida del tablero, ese es otro detalle que también comienzo a tomar en cuenta. En primer lugar, observo que los afiles no se pueden mover en una diagonal más grande de 2 cuadros, puesto que si exceden esta medida entonces quedarían en los posibles caminos de los que están en el extremo opuesto.

**Estrategia inicial**
Desde el punto de vista más fácil lo primero que se me vino a la mente fue mover los alfiles de forma que no importase que quedaran en los posibles caminos de los del otro color, viéndolo con esa lógica el primer movimiento que pensé fue en mover al segundo alfil blanco hacia la fila siguiente, pero en el extremo izquierdo, después hacer el mismo movimiento con el alfil negro de hasta el otro lado, lo que observe en este punto es que se formó una cierta simetría, el campo vacío que dejo el alfil negro lo pudo ocupar el alfil blanco y viceversa. Al notar que, al mantener cierta simetría, lo siguiente que hice mover de la misma manera los alfiles de la primera fila de la misma forma, pero del lado opuesto, es decir, simétricamente con respecto a la fila. Llegue a un punto en el que había que regresar a la primera fila el alfil blanco y el negro para poder repetir otro patrón de simetría y que quedara el camino libre para los demás alfiles y llegaran lo más rápido posible hacia el otro lado.

**Movimientos**
Si se mantenía la simetría se podían mover los alfiles alternadamente entre los dos colores, había por ejemplo ocasiones en las que había que moverse un solo cuadro y otras en las que se movían dos, note que este patrón también se repetía mucho. En los últimos movimientos quedaban diagonales en los extremos del tablero, por ejemplo, en la fila de hasta abajo (donde inicialmente se encontraban los alfiles blancos), quedaban dos diagonales de alfiles negros y en el otro lado el mismo caso, pero del color contrario. Al ver esto me percaté que solo faltaban 2 movimientos respectivamente para cada color, es decir, 4 movimientos en total y se llegaba a la solución. Movimientos para la solución Cada vez que simulaba un movimiento dibujándolo en la libreta iba contando cada uno, otro detalle aquí es que cada vez que un alfil blanco hacia un movimiento, la mejor estrategia era hacer que el siguiente alfil negro hiciera un movimiento similar, pero de forma simétrica, fue así como llegué a la solución. El número total de movimientos fue de aproximadamente 30 o 32, si es que no me comí alguno.

## Conclusión
LA resolución exitosa de este problema requiere de una estrategia con un enfoque cuidadoso que se pueda utilizar para respetar las limitaciones del juego, una de ellas es que cada color tenía que tomar un turno en cada movimiento. Si lo vemos desde ese punto de vista los alfiles blancos tenían que llegar al otro extremo, pero a la vez que los negros necesitaban hacer lo mismo. En lo personal a mí me cuesta trabajo interpretar las estrategias que sigo en mi mente o incluso plasmar la secuencia de pasos que tengo que seguir, más bien la forma en la que llego a la solución de algún problema es, ya sea simulándolo o haciendo los movimientos y necesito apoyarme de alguna bitácora o lista para poder recordar los pasos a seguir, hay personas que tienen mayor facilidad para plasmar su metodología pero en mi caso he notado que me es más sencillo poniéndolo en práctica, quizá desde un enfoque kinestésico. En conclusión, puedo decir que para solucionar un problema de esta naturaleza lo primer es observar detenidamente el tablero del juego y las piezas que hay, cuáles son sus dimensiones, observar cuales son las reglas y las limitaciones para hacer los movimientos, en base a ello pude deducir que si los movimientos eran alternados tenían que tener cierta coordinación y simetría al asociarlo con un numero par, además de que el número de piezas al ser 4 seguía esta lógica, también es importante tomar en cuenta los patrones que se van construyendo ya poniendo en práctica la solución del problema, creo que teniendo en cuenta estas características puede ser una herramienta útil para resolver otro problemas con características similares.

# Practica 4 Introducción a la inteligencia artificial Introspección: Contar islas en una matriz.
## Introducción.
El siguiente ensayo es el planteamiento de cómo resolver un problema, que consiste en contar el número de islas dentro de una matriz de elementos rectangulares o cuadrados, según la perspectiva que se note. El objetivo del mismo es poner en práctica la autopercepción de mi mente para encontrar la metodología para resolver este problema. Es importante conocer la forma en que nuestra mente trabaja y como asociando diferentes conocimientos previos, podemos encontrar la forma más óptima de encontrar una solución para poder implementar las diferentes técnicas de la inteligencia artificial.

## Desarrollo
Lo primero que observamos en este problema es una matriz de 14 x 22 cuadros, que más bien tienen formas rectangulares, dentro del cual la mayoría de los cuadros son blancos y se tienen 6 islas conformadas por cuadros grises oscuro, ese es el color que marca la diferencia y del cual se tienen que contar los cuadros para las islas. Al pedirse resolver el problema de contar los cuadros de diferente color, que serían los que contiene cada isla se toman en cuenta dos métodos, uno iterativo y uno recursivo en forma de algoritmos. Tomando esto en cuenta podríamos asignar un valor numérico a los elementos de color gris oscuro como un 1 y los de color blanco como un cero.

## Método iterativo.
En la parte iterativa se utilizaría una función que pueda recorrer la matriz en el sentido de las filas y en cada fila una columna, se puede pasar un color como referencia numérica, en el caso de querer contar los elementos de color gris oscuro solo se haría referencia al número 1. Al recorrer cada posición, si el cuadro es blanco la referencia sería un 0, por lo que un contador auxiliar que utilicemos podría regresar un valor de 0, referenciando que no encontramos nada. Teniendo como referencia el tamaño de la matriz, esto me hace asociarlo con un ciclo iterativo como por ejemplo el ciclo for, en el que podríamos recorrer fila y las columnas en otro for anidado. Sin embargo, para poder contar las islas que se tendrían en la matriz, debería de haber varios elementos con valor 1 conectados de forma vertical u horizontal, en cualquiera de las dos formas. Si en un dado caso se encuentra un valor de 1, se debería activar una variable que indique que se están contando los elementos dentro de una isla por lo que se debería de guardar la referencia de las columnas en las que se encuentran los elementos 1 en dicha fila y luego continuar en la siguiente fila en el momento que se dejen de encontrar elementos 1, lo que se me ocurre es que después se recorre la siguiente fila específicamente en las columnas referenciadas para así ver si también hay elementos con valor 1. Aunque si hay otros elementos consecutivos en la misma fila, entonces estos también formarían parte de la isla, este proceso se haría hasta llegar a un momento en el que ya no haya elementos 1 consecutivos y se contaría como una isla. Después se repetiría el proceso principal para encontrar más islas.

## Ejemplo iterativo:
```
matriz = [
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0],
[0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0],
[0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 0, 0],
[0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
[0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
[0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
[0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 1, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
]

filas = len(matriz)
columnas = len(matriz[0])


def explorar_isla(matriz, h, w):
    if 0 <= h < filas and 0 <= w < columnas and matriz[h][w] == 1:
        matriz[h][w] = 0 
        explorar_isla(matriz, h + 1, w)
        explorar_isla(matriz, h - 1, w)
        explorar_isla(matriz, h, w + 1)
        explorar_isla(matriz, h, w - 1)


islas_contadas = 0

for h in range(filas):
    for w in range(columnas):
        if matriz[h][w] == 1:
            islas_contadas += 1
            explorar_isla(matriz, h, w)

print(f"El número de islas es: {islas_contadas}")
```
Donde el color a contar seria 1

## Método recursivo.
Para una forma recursiva el método sería similar en su declaración pero tendría que mandarse a llamar dentro pero indicando las diferentes direcciones en las que podría moverse la posición en la que estemos, tomando en cuenta claro, que si estamos en la posición 0, no podemos ir a un número negativo y el límite sería ya sea el ancho o el alto de la matriz, además si devolvemos un valor de 1 cuando vamos encontrando una isla cuando se sume el contador podemos usar como referencia la recursividad del método utilizado.

## Ejemplo recursivo:
```
def contarElementosRecursivo(matriz, fila, columna, color):
    if not (0 <= fila < len(matriz)) or not (0 <= columna < len(matriz[0])) or matriz[fila][columna] != color:
        return 0

    contador = 1
    matriz[fila][columna] = None

    # Llamadas recursivas en todas las direcciones
    contador += contarElementosRecursivo(matriz, fila + 1, columna, color)
    contador += contarElementosRecursivo(matriz, fila - 1, columna, color)
    contador += contarElementosRecursivo(matriz, fila, columna + 1, color)
    contador += contarElementosRecursivo(matriz, fila, columna - 1, color)

    return contador

def contarIslas(matriz):
    islas_contadas = 0

    for h in range(len(matriz)):
        for w in range(len(matriz[0])):
            if matriz[h][w] == 1:
                islas_contadas += 1
                contarElementosRecursivo(matriz, h, w, 1)

    return islas_contadas

matriz = [
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0],
    [0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0],
    [0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 0, 0],
    [0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
    [0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
    [0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
    [0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 1, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
]

print(f"El número de islas es: {contarIslas(matriz)}")
```

## Conclusión
En conclusión, vemos que el método recursivo parece ser más óptimo que el iterativo, aunque pueden adaptarse características del otro según se necesite, en este caso creo que incluso solo con aplicar el segundo es suficiente, sobre todo por la naturaleza del problema, en donde la conexión de los elementos que conforman una isla puede ser tanto de forma horizontal como vertical. Lo que pude observar en este ejercicio, es que yo tenía asociado los métodos que vimos en las primeras clases con los ejercicios que estábamos resolviendo para encontrar islas también, creo que, entrando en contexto con la inteligencia artificial, estas características también podrían ser aprendidas y aprovechadas para resolver el problema.

# Practica 5 Introducción a la inteligencia artificial Introspección: Elementos de color en una imagen.
## Introducción
De manera digital las imágenes se han manejado tomando distintos espacios o píxeles a los que se les asigna un valor que es mostrado en monitor. Esto antes funcionaba de manera monocromática y permitía dibujar imágenes a partir de únicamente dos colores, dibujando en una matriz que sería la representación de la pantalla distintos valores que variarían entre 0 y 1 para mostrar la imagen al unirlos todos en una sola formación bidimensional que se mostraría a través de una interfaz, que en aquel tiempo únicamente podía hacer una pantalla.
Conforme se avanzó la tecnología fue capaz de manejarse valores de arreglos simples dentro de cada valor de esta matriz, estos valores serían la representación de colores más complejos a partir de unos principales, como es en el rgb tres valores y un Alfa que representa la opacidad. Así se podría dibujar una matriz donde cada valor tendría en sí un arreglo de tres valores o cuadros y se incluía el Alfa y estos a su vez generarían un promedio que dibujaría en una pantalla que permite hacer color una imagen con colores mucho más complejos que podrían variar de acuerdo a todas las combinaciones posibles de los valores en cada arreglo de cada pixel de cada imagen aumentando de una cantidad muy baja a una cantidad absurdamente grande de combinaciones y valores que ahora podrían representar distintas imágenes dentro de múltiples tipos de pantalla.
El problema planteado en esta sección en realidad es algo muy similar a lo anteriormente resuelto en una matriz simple solo que ahora se deberá manejar una matriz mucho más grande y darle al que se tendrá que diferenciar elementos que No necesariamente pueden ser valorados de un único modo y generando una igualdad específica a la que se tiene que buscar de modo que si antes teníamos que buscar Islas ahora lo que tenemos que buscar son segmentos con valores dentro de un Rango asociado promediando los valores dentro del arreglo de cada sección de la matriz principal.

## Desarrollo
La primera impresión que tengo de este problema es que veo una imagen con muchos objetos distribuidos y que además hay una gran variedad de colores. La mayoría de estos son alimentos que tienen tamaños, formas y colores distintos. Lo primero que se me viene a la mente en esta situación es que en un concepto muy básico una imagen puede ser considerada como una matriz, una matriz de pixeles, a fin de cuentas, en donde cada uno tiene un color distinto. 
Otra característica que observo es que la imagen es una matriz muy grande que, de hecho, su tamaño puede no siempre estar definido como lo es el caso de una matriz pequeña, pero a fin de cuentas si tomamos las medidas del número de filas y columnas entonces el ejercicio se puede resolver de manera muy similar al anterior, que es el de las islas, a fin de cuentas, en este caso es como si contáramos islas, pero ahora manejando un color como referencia. 
Para tener una referencia más clara y limitar los colores podríamos utilizar los rangos numéricos en que los colores se acercan a los tonos rojos y tener una sola referencia para detectar todos los objetos que puedan considerarse “rojos”. Los colores que normalmente hemos manejado en estos rangos son los RGB que son los tres colores primarios que forman a los demás, aunque solo es un formato de muchos que se manejan para el color digital. 
El primer paso sería poder procesar la imagen para convertirla en una matriz, esto utilizando una librería que permita el manejo de imágenes y colores como el caso de open cv del lenguaje Python, luego definir los colores. Además se debería definir un contador para guardar el número de elementos, objetos o islas encontrados con la característica que se solicita. Ejemplo de algoritmo.

```
r1 = 100, g1 = 0, b1 = 0
r2 = 255, g2 = 100, b2 = 100
islas = 0

mapa = cv.imread('atividad5.png', 1)  #leer los 3 canales con 1
w =mapa.shape[0]
h =mapa.shape[1]   #w y h para el ancho y alto de la imagen (filas y columnas)
#funcion para evaluar el color 
def rojo(i, j):
    if(mapa[i, j][2] >= r1 and mapa[i, j][2] <= r2):
        if(mapa[i, j][1] >= g1 and mapa[i, j][1] <= g2):
            if(mapa [i, j][0] >= b1 and mapa[i, j][0] <= b2):
                return True;
    return False;

Método recursivo. 
def metodoRecursivo(i, j):
    if not(i < 0 or i >= w or j < 0 or j >= h):
        if(rojo(i,j)):
            mapa[i,j][2] = 0
            mapa[i,j][1] = 0
            mapa[i,j][0] = 0
            metodoRecursivo(i - 1, j)
            metodoRecursivo(i + 1, j)
            metodoRecursivo(i, j - 1)
            metodoRecursivo(i, j + 1)
    return

Ejemplo iterativo: 
for i in range(w):
    for j in range(h):
        if(rojo(i, j)):
            islas += 1
            metodoRecursivo(i, j);
Mostrar resultados 
cv.imshow('Original',mapa)
print('islas:',islas)
cv.waitKey(0)
cv.destroyAllWindows()
```

## Conclusión
El ejemplo tratado es muy similar al anterior, donde solo se contaban islas, de hecho, entre más pequeños son los pixeles, más curveadas pueden apreciarse esas islas, pero viéndolos desde la perspectiva de una matriz, sabemos que también son cuadradas como el caso de una matriz que es más pequeña. Para el cerebro humano es más fácil detectar los objetos con colores porque no necesita hacer un análisis tan profundo del mismo, solo observa un todo en el que hay formas, colores, tamaños y diseños. En el caso de una computadora, esta tiene que aprender a procesar las imágenes como en este ejemplo, como si estas fueran una matriz y existen algunas librerías, como lo es open cv de Python que resultan muy útiles para el desarrollo de inteligencias artificial enfocada a la visión.


# Práctica 6. Introducción a la Inteligencia Artificial: El proceso de razonamiento según la lógica
## Problema
El Problema de Josephus se puede plantear matemáticamente como sigue: dado un círculo de n soldados numerados de 1 a n, y una constante k, los soldados son eliminados secuencialmente en pasos de k soldados, comenzando desde el soldado en la posición 1, y el proceso se repite hasta que solo queda un soldado. La pregunta es: ¿En qué posición inicial se debe colocar Josephus para ser el último sobreviviente?

## Solucion
El siguiente programa utiliza una lista para representar a los soldados y elimina secuencialmente a los soldados según las reglas del problema. La función ubicacion toma dos parámetros: el número total de soldados (n) y el proceso de eliminación (k). El resultado es la posición en la que Josephus debe sentarse para ser el último sobreviviente.

```
def ubicacion(n, k):
    soldados = list(range(1, n + 1))
    indice_soldado_actual = 0
    
    while len(soldados) > 1:
        # Calculamos el índice del soldado a eliminar
        indice_soldado_a_eliminar = (indice_soldado_actual + k - 1) % len(soldados)
        
        # Eliminamos al soldado
        soldados.pop(indice_soldado_a_eliminar)
        
        # Actualizamos el índice del soldado actual para el próximo ciclo
        indice_soldado_actual = indice_soldado_a_eliminar % len(soldados)
    
    return soldados[0]

n_soldados = 41
k_valor = 2
posicion_ganadora = ubicacion(n_soldados, k_valor)

print(f"Josephus debe sentarse en la posición {posicion_ganadora} para ser el último sobreviviente.")
```

# Práctica 7. Introducción a la Inteligencia Artificial: El papel de la heurística
## Definicion de heuristica 
Cuando buscamos resolver un problema de una complejidad considerable se puede volver complicado encontrar una solución óptima para este.
La manera en que encontramos soluciones generalmente Busca ser muy concreta o atacar el problema de manera que se entienda perfectamente cómo y de qué modo se puede llegar a la solución. Sin embargo, esto puedo incrementar demasiado la complejidad de la resolución al punto que deja de ser rentable o se vuelve muy ineficiente el encontrar una solución óptima.
Para muchos problemas la solución puede venir de varias maneras y aunque Generalmente existe una solución más óptima se puede resolver el problema de maneras menos eficientes pero más sencillas de pensar, existiendo soluciones comunes debido a la relativa simpleza con las que uno puede llegar a ellas a pesar de existir mejores soluciones.
Aquí es cuando el papel de la heurística se vuelve importante pues esta permite tomar un problema complejo y simplificarlo en uno que se puede resolver de manera más simple aunque sin buscar una solución concreta y eficiente, sino que tomando únicamente los elementos mínimos suficientes para poder resolver el problema en cuestión.
Así se puede llegar a soluciones bastante satisfactorias que además presentan un nivel de simpleza relativamente alto y que puede ser llevadas a cabo de manera aceptablemente eficiente aunque dejando el lugar para una solución más óptima.

## Solucion y algoritmo con recursividad programado
```
def Solucion(matriz, inicio, entrada):
    row, col = inicio
    num_rows, num_cols = len(matriz), len(matriz[0])

    if 0 <= row < num_rows and 0 <= col < num_cols:
        up_value = matriz[row - 1][col] if row - 1 >= 0 else float('inf')
        down_value = matriz[row + 1][col] if row + 1 < num_rows else float('inf')
        left_value = matriz[row][col - 1] if col - 1 >= 0 else float('inf')
        right_value = matriz[row][col + 1] if col + 1 < num_cols else float('inf')

        min_value = min(up_value, down_value, left_value, right_value)

        if min_value == up_value:
            movimiento = row - 1, col
        elif min_value == down_value:
            movimiento = row + 1, col
        elif min_value == left_value:
            movimiento = row, col - 1
        elif min_value == right_value:
            movimiento = row, col + 1
        
        if movimiento[0] == 0 or movimiento[0] == num_rows - 1:
            if  movimiento != entrada:
                return movimiento
        if movimiento[1] == 0 or movimiento[1] == num_cols - 1:
            if  movimiento != entrada:
                return movimiento
        
        matriz[row][col] += 0.1
        
        return Solucion(matriz, movimiento, entrada)

    return None

matriz = [
    [1, 1, 1, 1, 1, 1, 1, 1, 1],
    [0, 0, 0, 0, 0, 0, 1, 0, 1],
    [1, 1, 1, 0, 1, 1, 1, 0, 1],
    [1, 0, 0, 0, 1, 0, 1, 0, 1],
    [1, 0, 1, 1, 1, 0, 1, 0, 1],
    [1, 0, 0, 0, 0, 0, 0, 0, 1],
    [1, 0, 1, 1, 1, 0, 1, 0, 1],
    [0, 0, 1, 0, 0, 0, 1, 0, 1],
    [1, 1, 1, 1, 1, 1, 1, 1, 1],
]

inicio = (7, 0)

end = Solucion(matriz, inicio, inicio)
print("Entrada: ", inicio, "\nSalida:  ", end)
```

## Explicacion
El funcionamiento del algoritmo sigue la solución propuesta y se adapta un código que sea ejecutable por Python.
El algoritmo al ser recursivo funcionará llamándose a sí mismo cada que encuentre un nuevo espacio. Lo primero es definir qué información necesita el algoritmo para funcionar, este requiere de una matriz que representará el espacio, un punto que indicará en dónde se encuentra en la matriz, y una coordenada que indica cuál es la entrada para utilizarla al momento de diferenciar la salida.
Este obtiene las coordenadas del punto en que se encuentra, además del tamaño que tiene la matriz. Después válida que el punto existe en la matriz y una vez hecho eso comienza a obtener los valores de los espacios que se encuentran una coordenada arriba, abajo, a la izquierda, y a la derecha, obteniendo después cuál es la coordenada del espacio que tiene el menor valor para así tomar este como el siguiente paso a dar.
Una vez hecho eso se obtendrá la coordenada de este nuevo espacio y se analizará que esta no sea una salida, de no serlo se volverá a llamar la función de manera recursiva pasando la matriz donde el valor de la coordenada por la que se acaba de pasar se aumentará en 0.1, se le pasará un nuevo punto de inicio qué será el espacio al que se deberá de mover y el mismo punto de entrada para que la pueda diferenciar de la salida.
Una vez hecho esto se le puede mandar una matriz inicial que posea un único cero en el borde y un camino recorrible donde la matriz puede tener cualquier tamaño y se respete los ceros y unos como representaciones de Laberinto. Este lo resolverá recorriéndolo para finalmente devolver el punto de entrada y el de salida.

# Practica 8 Reglas y Búsquedas : Espacio de Estados

## Medida de rendimiento y frecuencia de percepción para el problema de las ranas rojas y azules con un salto cada color

**Para este problema la medida de rendimiento es pasar a todos los individuos de un lado a otro, pero las ranas solo pueden saltar una a la vez, no pueden saltar mas de una rana o un espacio vació, no pueden regresarse y deben saltar una rana azul y luego una roja y así sucesivamente**

| Posiciones | Acción a realizar |
| --------- | --------- |
| ( A1 A2 A3 _ R1 R2 R3 ) | Salta rana azul 2|
| ( A1 _ A3 A2 R1 R2 R3 ) | Reiniciar porque no pueden seguir |
| ( A1 A2 A3 _ R1 R2 R3 ) | Salta rana azul 3|
| ( A1 A2 _ A3 R1 R2 R3 ) | Salta rana roja 1|
| ( A1 A2 R1 A3 _ R2 R3 ) | Salta rana azul 3|
| ( A1 A2 R1 _ A3 R2 R3 ) | Salta rana roja 2|
| ( A1 A2 R1 R2 A3 _ R3 ) | Salta rana azul 3|
| ( A1 A2 R1 R2 _ A3 R3 ) | Salta rana roja 3|
| ( A1 A2 R1 R2 R3 A3 _ ) | Salta rana azul 3|
| ( A1 A2 R1 R2 R3 _ A3 ) | Reiniciar porque no se puede seguir|
| No hay mas combinaciones | El problema no tiene solución |

**Bajo la medida de rendimiento empleada con anterioridad es claro que el problema de las seis ranas no puede ser resuelto de esta forma dado que se atora de forma contundente sin importar que acciones se tomen, por ello a continuación se va a replantear un punto en especifico empleado en la medida de rendimiento**

## Medida de rendimiento y frecuencia de percepción para el problema de las ranas rojas y azules siendo capaz de saltar mas de un color seguido

**Para este problema la medida de rendimiento es pasar a todos los individuos de un lado a otro, pero las ranas solo pueden saltar una a la vez, no pueden saltar mas de una rana o un espacio vació, no pueden regresarse y en este caso pueden saltar en cualquier orden**

| Posiciones | Acción a realizar |
| --------- | --------- |
| ( A1 A2 A3 _ R1 R2 R3 ) | Salta rana azul 3|
| ( A1 A2 _ A3 R1 R2 R3 ) | Salta rana roja 1|
| ( A1 A2 R1 A3 _ R2 R3 ) | Salta rana roja 2|
| ( A1 A2 R1 A3 R2 _ R3 ) | Salta rana azul 3|
| ( A1 A2 R1 _ R2 A3 R3 ) | Salta rana azul 2|
| ( A1 _ R1 A2 R2 A3 R3 ) | Salta rana azul 1|
| ( _ A1 R1 A2 R2 A3 R3 ) | Salta rana roja 1|
| ( R1 A1 _ A2 R2 A3 R3 ) | Salta rana roja 2|
| ( R1 A1 R2 A2 _ A3 R3 ) | Salta rana roja 3|
| ( R1 A1 R2 A2 R3 A3 _ ) | Salta rana azul 3|
| ( R1 A1 R2 A2 R3 _ A3 ) | Salta rana azul 2|
| ( R1 A1 R2 _ R3 A2 A3 ) | Salta rana azul 1|
| ( R1 _ R2 A1 R3 A2 A3 ) | Salta rana roja 2|
| ( R1 R2 _ A1 R3 A2 A3 ) | Salta rana roja 3|
| ( R1 R2 R3 A1 _ A2 A3 ) | Salta rana azul 1|
| ( R1 R2 R3 _ A1 A2 A3 ) | Fin |

## Medida de rendimiento y frecuencia de percepcion para el problema de la lechuga, el pollo y el zorro

**Para este problema la medida de rendimiento es pasar a todos los individuos de uno en uno, utilizando el menor numero de viajes posibles y sin que se coman entre ellos ninguno de ellos**

| Posicion inicial | Barco | Posicion Final | Acción a realizar |
| --------- | --------- | --------- | --------- |
| ( L P Z ) | ( ) | ( ) | Llevarse al pollo |
| ( L Z ) | ( P ) | ( ) | Dejar al pollo y regresar por el zorro |
| ( L ) | ( Z ) | ( P ) | Dejar al zorro y regresar con el pollo |
| ( L ) | ( P ) | ( Z ) | Dejar al pollo y llevarse la lechuga |
| ( P ) | ( L ) | ( Z ) | Dejar la lechuga y ir por el pollo |
| ( ) | ( P ) | ( L, Z ) | Dejar al pollo  |
| ( ) | ( ) | ( P, L, Z ) | Fin |

## Medida de rendimiento y frecuencia de percepción para el problema de los monjes y caníbales

**Para este problema la medida de rendimiento es pasar a todos los individuos sea de uno en uno o pasando de dos en dos, utilizando el menor numero de viajes posibles, que la canoa siempre debe ser manejada por un individuo y que sin importar el movimiento nunca queden mas caníbales que monjes en una de las orillas porque entonces los caníbales se comerían a los monjes**

| Posicion inicial | Barco | Posicion Final | Acción a realizar |
| --------- | --------- | --------- | --------- |
| ( M M M C C C ) | ( ) | ( ) | Cruzar dos caníbales |
| ( M M M C ) | ( C C ) | ( ) | Dejar a un caníbal y regresar |
| ( M M M C ) | ( C ) | ( C ) | Irse los dos caníbal |
| ( M M M ) | ( C C ) | ( C ) | Dejar a un caníbal y regresar |
| ( M M M ) | ( C ) | ( C C ) | Dejar a un caníbal y irse dos monjes |
| ( M C ) | ( M M ) | ( C C ) | Dejar a un monje y regresar uno y uno |
| ( M C ) | ( M C ) | ( M C ) | Dejar al caníbal y irse los monjes |
| ( C C ) | ( M M ) | ( M C ) | Dejar a los monjes y regresar el caníbal |
| ( C C ) | ( C ) | ( M M M ) | Llevarse otro caníbal |
| ( C ) | ( C C ) | ( M M M ) | Dejar un caníbal y regresar |
| ( C ) | ( C ) | ( M M M C ) | Llevarse al ultimo caníbal |
| ( ) | ( C C ) | ( M M M C ) | Quedarse todos del otro lado |
| ( ) | ( ) | ( M M M C C C ) | Fin |
