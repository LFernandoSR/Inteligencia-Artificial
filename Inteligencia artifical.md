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
El siguiente ensayo habla sobre la inteligencia artificial vista desde el punto de vista que propone el documental “Inteligencia Artificial” que nos otorga Discovery cannel en colaboración con IBM, la cual ha sido una pionera en el desarrollo de esta ciencia. Este documental nos presenta principalmente los distintos ámbitos más importantes en los que la misma ha tenido gran relevancia y aplicaciones como es el caso de los juegos de estrategia, la conversación, la industria, la educación y la salud. Por otro lado, nos habla de un tema importante el cual es como la inteligencia general puede ser un avance para su desarrollo. Es importante conocer las aplicaciones más importantes que ha tenido y también el futuro que la misma puede tener.

## Desarrollo
La inteligencia artificial es un tema con una amplia variedad de puntos de vista y como era de esperarse, es un tema que ha sido tratado incluso por la compañía de televisión Discovery Channel, la cual se dedica a la presentación de documentales de todos los temas científicos y sociales más importantes de la actualidad. El documental del que hablan en esta ocasión trata sobre esta disciplina, me parece muy interesante el enfoque que le dan y las cosas en común que se tienen con el libro “Inteligencia artificial: un enfoque moderno”. Pero primero hablemos sobre algunos temas que se tratan en el mismo. El documental fue realizado con la colaboración de IBM, una de las empresas de cómputo y tecnología más importantes y antiguas que existen. Un tema del que se aborda en primer lugar es que la inteligencia artificial no solo es una tecnología o una sola técnica, si no que se basa en muchas técnicas que se pueden aplicar para que un agente pueda aprender, tal como es el procesamiento de lenguaje natural o de imágenes por computadora. Es considerada como artificial cuando no se trata de un ser biológico aquel que puede tener entradas y salidas de información, pero con capacidad de tomar decisiones y resolver problemas. Las trivias. El primer ejemplo de aplicación en este campo que el documental nos muestra es Watson, la inteligencia artificial creada por IBM, nos muestra como en sus inicios esta intenta competir en el jugo de televisión Jeopardy, en el cual se presenta un concepto o definición y se tiene que contestar en forma de pregunta la palabra clave. Vemos que al principio Watson no podía contestar muy bien las preguntas, pero después de tener ciertas mejoras y haber adquirido un enorme conocimiento de libros con temas de los que se hablaba en el juego, finalmente pudo contestar la mayoría de las preguntas correctamente y en poco tiempo, haciendo consultas muy rápidamente. Podemos ver que en base al conocimiento que una inteligencia tiene, esta va llegando a mejores conclusiones, pero además se aplica el uso de la probabilidad para acercarse a las mejores respuestas, como en el caso de los debates, donde se van dando puntos de vista basados en los conocimientos previos que las personas tienen y en base a esto se llega a una conclusión sobre si el argumento de la persona que está a favor es mejor o de la que está en contra.

**La IA en el debate.** 
El documental nos muestra un segundo ejemplo de la aplicación de la inteligencia artificial, en donde esta vez se trata de un debatiente que es una máquina capaz de escuchar y consultar todos los conocimientos que tiene en base a muchos documentos que tiene en si memoria, algo interesante en esta parte es que podemos notar que la capacidad de un ser humano de entender su propio lenguaje por ejemplo es muy fácil, pero en contraparte las maquinas tienen mucha más capacidad de memoria con respecto a la información que pueden consultar para generar sus respuestas y otro aspecto importante es que pueden seguir aprendiendo, cuando una maquina puede hacer uso del procesamiento de lenguaje natural incluso es capaz de comunicarse con una persona, como en este caso del debate en el que una debatiente es una mujer humana que argumenta en contra del tema de legalizar las apuestas deportivas, mientras que la inteligencia artificial está a favor y conforme va a aprendiendo más, consulta más información para poder contestar a los argumentos que la mujer dice.

**Los automóviles autónomos** 
Cuando hablamos del aprendizaje automática también podemos pensar en conducir un automóvil, y es este otro tema que maneja el documental, dentro de este tema nos plantea que durante años se ha buscado el desarrollo de los automóviles autónomos, los cuales ya no necesitan de un conductor humano, estos tienen las capacidades de ser manejados por algún programa de inteligencia artificial, sin embargo no todo es tan bueno como suena, también podemos ver que nos explica como también puede conllevar muchos riesgos como accidentes y pérdidas de vidas, la mayoría de los ejemplares de inteligencia artificial se desarrollaron sabiendo que se equivocarían muchas veces y no habrían consecuencias graves, sin embargo si hablamos de los carros autónomos entonces si es algo muy delicado, algo importante que yo puedo destacar aquí es que para una persona es muy fácil comprender la subjetividad y la inestabilidad de como suceden las cosas en el mundo real, ya sea por experiencia, emociones o simple sentido común, sin embargo para una maquina esta percepción es más rígida y necesita tener un aprendizaje fuertemente sólido. Por lo que incluso nos menciona que, aunque si es posible este avance tecnológico, le tomará muchos años para poder concretarse. Para este punto me pareció interesante como es que un agente inteligente puede reconocer las cosas que percibe con el procesamiento de imagen, o lo que podríamos considerar sus ojos, o vista, y a su vez, este tiene ya un conocimiento de los objetos, de alguna manera los va clasificando y les pone etiquetas.

**La IA en los juegos y las redes sociales** 
La inteligencia artificial también ha tenido mucha aplicación en el ámbito de los juegos y los videojuegos, una de sus primeras aplicaciones es el juego de damas inglesas, tal como nos muestra IBM que creo su IA llamada DeepBlue, la cual mostró una gran habilidad para jugar juegos de estrategia como las damas, incluso logrando vencer al mejor jugador humano en un dado momento. También podemos ver que existen otros ejemplos como el de Go zero, una IA capaz de jugar un juego oriental llamado Go, el cual nos dice que tiene más posiciones o combinaciones en su tablero que el número de átomos en el universo, que es algo inimaginable, pero esta IA logra aprender los patrones para poder llegar a obtener su objetivo con la ruta más corta, es decir, con el menos número de movimientos posibles. De esta manera podemos también ver que no solo se trata de decidir de la forma más acertada, si no de llegar a esa decisión de la forma más rápido y de hacer las cosas de la forma más óptima. Otro aspecto en el que se ha aplicado la IA es en las redes sociales como Facebook, twitter y redes de música como spotify, en donde la plataforma aprende los patrones que más repite el usuario y le va mostrando información más acercada a sus tendencias.

**La IA en los trabajos** 
El tema de la inteligencia artificial en el ámbito del trabajo ha sido también muy controversial, por un lado es el temor de muchas personas de que puedan perder sus trabajos por culpa de estas, pero por el otro también es importante tomar en cuenta que es una herramienta que se creó para ayudarnos de alguna manera, un punto importante que me gustaría mencionar es que hay muchos trabajos donde se pueden llevar a cabo tareas muy repetitivas e incluso peligrosas, y es principalmente en estos ámbitos en donde más vale la pena tomar en cuenta a la IA, el documental nos muestra el ejemplo de un robot, Soyer, el cual se usa para hacer tareas como cortar y perforar piezas de madera, pero a su vez, el personal humano le va enseñando la forma en que tiene que hacer sus actividades, de alguna manera vemos que es necesario el apoyo humano para que la IA pueda hacer su trabajo correctamente y la vez esta no se cansa de llevar a cabo actividades que pueden ser tediosas, creo que hay muchas ocasiones en las que al hacer cosas tediosas perdemos la concentración y si estamos en un trabajo peligroso como el que mencioné anteriormente si es más probable que suframos un accidente, pero una maquina no se va a cansar, una maquina solo necesita de su fuente de energía y sigue funcionando, a su vez, puede haber otra oportunidad de trabajo para la persona que ha sido reemplazada por esta. También pude notar que en el ejemplo mencionado la maquina tuvo su aprendizaje, pero por medio del entrenamiento, en donde pudo guardar los movimientos que la persona la iba mostrando y esta los tomaba para repetir esas acciones y realizar su trabajo, en este caso parece que las entradas fueron patrones de movimientos del cuerpo de la máquina. Si la IA puede aprender, puede enseñar. La IA también se ha desarrollado como una herramienta de apoyo en el ámbito de la educación como el ejemplo de la aplicación que se le dio a Watson para poder enseñar a los niños en sus primeros 8 años de vida, hasta ser un compañero de apoyo para estudiantes mayores como los universitarios, un ejemplo de este caso es la herramienta de chat GPT, el cual en base a sus conocimientos es una herramienta de consulta rápida de información que puede servir de apoyo para muchos estudiantes, aunque depende de la manera en que estos la utilicen y sobretodo, pienso que se debe de usar como una herramienta para enriquecer el conocimiento que ya tenemos, además de resolver el problema que se nos presente, y además de resolver alguna tarea más rápido, podamos aprender más rápidamente. Como herramienta de apoyo, se plantea que por otro lado la IA puede ser una compañera para personas con discapacidades como los invidentes, el documental nos muestra otro ejemplo de un hombre llamado Simon que padecía de una enfermedad de la retina, la cual ocasionó que perdiera la vista, pero él quiso ser lo más independiente posible de otras personas, la solución a esto fue un brazalete que usaba la aptica, una tecnología que hace uso de la comunicación por el sentido del tacto, el dispositivo con IA que utilizó para apoyarse era la wayband, la cual le ayudaba por medio de señales apticas a mantenerse corriendo o caminando por el camino correcta, a su vez, este hacía uso de datos como las rutas trazadas por el gps y la comunicación por internet, en este caso también podemos ver como la inteligencia artificial siempre está nutrida por los datos y estos a su vez deben ser útiles dentro del contexto en el que se pretende solucionar un problema, en este caso poder trazar un camino y comunicarse con una persona sin la capacidad de ver.

**La percepción de la IA y la privacidad** 
Las máquinas que usan inteligencia artificial necesitan utilizar dispositivos en los que puedan recibir entradas de información como mencionaba anteriormente, para tener un oído usan micrófonos, para tener una voz usan un altavoz, por ejemplo, para una vista, una cámara y para un tacto, algún sensor. Con estas características una maquina ya puede percibir objetos o personas dentro del entorno en el que esta se encuentre, el documental nos muestra un ejemplo en el que la IA haciendo el uso del procesamiento de la imagen con la cámara puede detectar los rostros de las personas, todas las personas comparten características similares en sus rostros, todos tienen dos ojos, una nariz y una boca, cabe mencionar que puede haber casos excepcionales de los que la IA también tendría que aprender en el futuro. Al poder detectar los rostros de las personas ya se pueden tener muchas aplicaciones, nos habla de que hay un caso en el que en China se usó una IA para detectar a posibles criminales con solo observar su rostro, esto basado en los patrones o características que se presentan en los rostros de personas que han cometido delitos, sin embargo, nos menciona que esta característica también puede afectar a la privacidad de la gente, es un tema bastante claro que el precio de la seguridad es la privacidad individual que tenemos, por lo que creo que es un tema controvertido que también es importante, podríamos plantear que debe haber un equilibrio entre ambos pero la verdad es que solo probándolo en un cierto periodo de tiempo es cómo podríamos realmente saber si es conveniente esta aplicación de la inteligencia artificial. Me parece interesante como una maquina también puede procesar las imágenes que percibe en forma de matrices de datos numéricos en muy poco tiempo, además de que en el ejemplo anterior se nos menciona que se usan cámaras de video, o sea que hablamos del procesamiento de miles y miles de fotogramas por segundo, esto también resalta la enorme capacidad de procesamiento de información y almacenamiento de la misma y es una cualidad que puede tener como ventaja una maquina al hacer uso de la misma.

**La inteligencia artificial en la salud** 
Tocando el tema de la salud de las personas, también se nos muestra un ejemplo de su aplicación en la que un hombre que padece de parkinson, una enfermedad asociada al movimiento de las articulaciones le afecta y tiene como iniciativa poder ayudar a otras personas con situaciones similares a la suya, algo importante que podemos rescatar aquí que es la IA a la que se recurre es Watson de IBM aplicada al ámbito de la salud, específicamente hacia esta enfermedad, vemos que si la IA tiene un conocimiento entonces rápidamente puede hacer una recomendación de los fármacos que le pueden servir a cada persona, y estas recomendaciones se harían en base a los datos que tenga de cada una, creo que también puede ser una herramienta compañera para los médicos y los enfermeros a quienes se les puede presentar la situación de que necesitan consultar algún medicamento o sustancia que las ayude si por ejemplo se encuentran en una situación de emergencia o incluso alguna operación de un paciente, en este tipo de situaciones el tiempo es una variable muy importante que puede marcar la diferencia entre la vida y la muerte y creo que es una de las ventajas más importantes que la IA puede ofrecer en todas estas situaciones, por otro lado, creo que en cuestión de los pacientes también puede ser una compañera de apoyo para cuando se quieren rehabilitar o para poder llevar correctamente sus tratamientos, como seres humanos, siempre tendemos a ser muy variables y a equivocarnos en la precisión para las cosas que hacemos, como seguir un plan de recuperación por ejemplo y sería una aplicación interesante.

**Inteligencia general y singularidad** 
El último punto que el documental toca es acerca de cómo puede ser posible la súper inteligencia artificial o singularidad y la inteligencia que las personas tenemos, la inteligencia general, nos dice que esta es la capacidad de saber actuar en cualquier tipo de situación o entorno y entenderlo a la vez, si por otro lado le damos esta capacidad a la inteligencia artificial entonces esta podría crecer exponencialmente y convertirse en una singularidad o súper inteligencia artificial, de hecho, nos plantea que si llegara a existir un ejemplar de la misma, esta sería construida a partir de otra inteligencia artificial, lo cual hace muchos sentido porque puede ir evolucionado al punto de ser ya tan avanzada que incluso tenga la capacidad de crear a otra, otra que incluso pueda superar a nuestra inteligencia, pero creo yo que un factor que debería existir para que esto sea posible es que nosotros podemos entender el origen de nuestra conciencia, ese misterio que se encuentra encima de esta, creo de solo así podríamos entender esto y de alguna manera dotar a la IA de conciencia para que entonces sea posible que pudiera superarnos o por lo menos llegar a nuestro nivel de conciencia o autopercepción. Este último tema es bastante interesante y creo que también plantea una premisa de lo que podría ser un próximo paso clave para una mayor evolución de la inteligencia artificial en los próximos años.

## Conclusiones
La inteligencia artificial se ha considerado como una amenaza para muchos trabajadores e incluso algo que podría reemplazarnos en muchas funciones o volver a las personas menos funcionales y más perezosas, sin embargo, es importante siempre recordar que esta es una herramienta que debe servirnos como un apoyo, y que a su vez esta recibe el apoyo humano para desempeñar mejor sus tareas. Creo que está en nuestras manos hacer que como herramienta tenga un buen crecimiento y a la par esta contribuya que nosotros seamos mejores personas y de alguna forma podemos cuidar otros aspectos que nos ayuden a ser más saludables ya que muchas veces el trabajo puede consumirnos y esto es algo que a una maquina no puede afectar. Como podemos observar, en un equipo siempre hay miembros con una cualidad y otros con otras, si trabajamos en equipo con la inteligencia artificial esto puede ser algo que nos ayude mucho, el ser humano tiene la cualidad de tener una conciencia sobre sí mismo pero no tiene tanta resistencia al trabajo y además es frágil ante tareas peligrosas, por su parte, las máquinas no tienen conciencia de sí mismas o de la forma en que aprenden pero pueden soportar largas jornadas de trabajo sin verse agotadas o aburridas, evitando el riesgo de tener accidentes en algún momento, viéndolo desde este punto de vista podemos darnos cuenta de que podemos colaborar como un equipo con la inteligencia artificial si sabemos aprovecharla adecuadamente, sin necesidad de verla como una competencia o como una amenaza, simplemente una compañera.


# Práctica 2: Ensayo. Introducción a la Inteligencia Artificial: Tipos de Inteligencia.
## Teoría de las Inteligencias Múltiples de Gardner

## Introducción
Este ensayo habla sobre el tema de los tipos de inteligencias que el psicólogo Howard Gardner mencionó en contraparte de la idea de que la inteligencia es única y puede abarcar todas las habilidades. Es importante conocer los tipos de inteligencia que pueden tener las personas para tener un amplio punto de vista y comprender que muchas veces es un error el generalizar y catalogar a alguien como inteligente o no inteligente, solo por el hecho de tener o no una habilidad en específico, como, por ejemplo, en la escuela.

## Desarrollo
De acuerdo con el punto de vista de Gardner, la inteligencia no es una sola, si no que pueden existir diferentes tipos de esta para diferentes contextos. Basado en lo que se ha hablado anteriormente sobre la inteligencia artificial, el objetivo de la misma es resolver problemas, y en lo que se relaciona este tema con el mencionado es que, para cada contexto o campos, como, por ejemplo, las ciencias sociales, el arte, o la lógica pueden existir diferentes tipos de inteligencias para cada uno. 
Gardner nos menciona que existen algunos tipos de inteligencia que podemos mencionar como la inteligencia lingüística verbal, la inteligencia física kinestésica, la inteligencia lógico matemática, inteligencia espacial, inteligencia musical, inteligencia interpersonal, inteligencia intrapersonal, aunque también se pueden considerar otros tipos como la naturalista, espiritual y existencial. Cada una se enfoca a diferentes situaciones y esto cobra bastante sentido para mí, puesto que en muchas ocasiones observamos que el alumno más listo en una escuela no siempre es el mejor compañero que te pueda brindar apoyo emocional, si bien este puede ser consciente de cómo funcionan los sentimientos y emociones humanas, en la mayoría de las ocasiones no podrá interpretar adecuadamente la situación de la otra persona, es aquí donde entra la importancia de que Gardner categorice la inteligencia en las que mencionamos anteriormente. 
La inteligencia lingüística verbal se enfoca en la parte de la comunicación como las palabras que se dicen y de alguna forma moldearlas para que estas puedan ser interpretadas de diferentes maneras, muchas personas como escritores, mangakas, novelistas y guionistas tienen este tipo de inteligencia y logran conectar con otras personas a través de esta. Un ejemplo que se me viene a la mente relacionado a la IA es el procesamiento del lenguaje natural, en el que la maquina puede leer e interpretar textos de diferentes naturalezas. 
En el caso de la inteligencia lingüística kinestésica un ejemplo que me viene a la mente según lo que menciona Gardner, son las personas que pueden interpretar el lenguaje de los sordomudos, muchos gimnastas artísticos. Un ejemplo interesante en la inteligencia artificial serían los robots mecánicos que desde su programa de agente logran enviar señales a los actuadores, que serían como sus brazos o piernas, quizá ruedas, según el movimiento que necesitan realizar para llevar a cabo una tarea. 
También se menciona que la inteligencia matemática es la capacidad de manejar números y realizar todo tipo de análisis y operaciones con ellos, en este caso, creo que es uno de los ejemplos más básicos relacionado a las maquinas que usan IA, ya que los datos con los que trabajan principalmente son números, de hecho, la base de las señales que trabaja un computador son pulsos eléctricos interpretados como 0 y 1, por lo que cobra bastante sentido. 
En lo que es inteligencia espacial podemos relacionarla con la parte de la vista o el procesamiento de las imágenes, los colores, las formas. Por otro lado, la inteligencia musical está más relacionada con la parte auditiva, aquí podemos mencionar parámetros como los tonos, frecuencias, tiempos y ritmos. Gardner menciona también otros tipos de inteligencia más apegadas a la parte humana , como la inteligencia interpersonal y la intrapersonal, la primera es la forma en que un individuo puede entender las emociones y los sentimientos de otras personas y de esa forma sabe cómo responder o que decisiones tomar para lograr los mejores resultados y resolver una situación de esa naturaleza, por otro lado la intrapersonal es muy similar pero esta vez el individuo se puede comprender a sí mismo y tomar las mejores decisiones para sí mismo. 
Otras inteligencias propuestas por Gardner. Algunos otros ejemplares que Gardner menciona en su libro “La inteligencia reformulada. Las inteligencias múltiples en el siglo XX”, nos habla de que existen otras 3 inteligencias, la naturalista, espiritual y existencial. Estos ejemplos me suenan a algo más filosófico y humanista, el percibir el mundo en sus plantas y animales, las cuestiones de las cosas en las que cree el ser humano para su crecimiento y bienestar o, mejor dicho, bien actuar, y por otro lado la parte de llegar a su bienestar por medio de llegar a un estado mental de calma. 
Estas inteligencias que menciona Gardner me parecen muy interesantes, de hecho, las he visto en varios libros de auto ayuda y son muy mencionadas sus características, como tal no había leído o escuchado sobre estos nombres como Gardner menciona para leyendo sus características si me hace bastante sentido. Desde mi punto de vista, este tipo de inteligencias más modernas que el mismo autor nos menciona dan un acercamiento a la conciencia del ser humano sobre sí mismo, su mente, sobretodo. 
Otro aspecto que nos menciona es la superdotación en las inteligencias en donde las capacidades intelectuales es muy alta, sin embargo, la falla que se encuentra aquí es que, si una persona fuera muy inteligente en una de las inteligencias mencionadas, esta tendría desbalances en las demás. Este tema me hace pensar en que sería algo muy idealista el pensar que una persona o entidad pueda poseer simultáneamente todos los tipos de inteligencias y además en un nivel de superdotación, sería algo muy cercano a la perfección de hecho.

**El aprendizaje**

Otro aspecto importante que dice Gardner es que la inteligencia de una persona depende principalmente de la manera en que esta absorbe o recibe la información, en cualquier forma. La información sobre música comúnmente no la recibimos como la espacial o como a matemática, de hecho, hay muchas personas que tienen un sentido más desarrollado que otro. El otro punto importante que pude ver es que también cada tipo de inteligencia es autónoma, es decir, se desarrolla de forma independiente, esto también tiene bastante sentido y se relaciona a la forma en que una persona desarrolla mayores habilidades en un área y otra persona en otra. Gardner nos menciona que el cerebro humano se divide en distintos sectores que se enfocan en diferentes habilidades cada uno.

## Conclusiones
La inteligencia que poseen las personas comúnmente se enfoca en algún aspecto, o se apega a alguno de los tipos de inteligencia que menciona Gardner. Viéndolo desde el punto de vista de las máquinas y la inteligencia artificial, esto nos ayuda a entender que esta ciencia tiene muchas variantes y se especializa en resolver diferentes tipos de problemas. La inteligencia artificial no está basada en único y absoluto tipo de inteligencia y hay ocasiones en los que necesitamos trabajar con textos, con imágenes o con sonidos al utilizarla por lo que puedo decir que la teoría de Howard Gardner se aplica muy bien y nos sirve para entender este aspecto de la misma.


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
def contarElementosIterativo(matriz, fila, columna, color): 
    if matriz[fila][columna] != color: 
        return 0 contador = 0 referencia = [(fila, columna)] 
    while referencia: f, c = referencia.pop() 
        if 0 <= f < len(matriz) and 0 <= c < len(matriz[0]) and matriz[f][c] == color: 
            contador += 1 matriz[f][c] = None
        stack.append((f + 1, c)) 
        stack.append((f - 1, c)) 
        stack.append((f, c + 1)) 
        stack.append((f, c - 1)) 
        return contador 
```

## Método recursivo.
Para una forma recursiva el método sería similar en su declaración pero tendría que mandarse a llamar dentro pero indicando las diferentes direcciones en las que podría moverse la posición en la que estemos, tomando en cuenta claro, que si estamos en la posición 0, no podemos ir a un número negativo y el límite sería ya sea el ancho o el alto de la matriz, además si devolvemos un valor de 1 cuando vamos encontrando una isla cuando se sume el contador podemos usar como referencia la recursividad del método utilizado.

## Ejemplo recursivo:
```
def contarElementosRecursivo(matriz, fila, columna, color): 
    if not (0 <= fila < len(matriz)) or not (0 <= columna < len(matriz[0])) or matriz[fila][columna] != color: 
        return 0 contador = 1 
        matriz[fila][columna] = None 
        contador += contarElementosRecursivo (matriz, fila + 1, columna, color) 
        contador += contarElementosRecursivo (matriz, fila - 1, columna, color) 
        contador += contarElementosRecursivo (matriz, fila, columna + 1, color) 
        contador += contarElementosRecursivo (matriz, fila, columna - 1, color)
```

## Conclusión
En conclusión, vemos que el método recursivo parece ser más óptimo que el iterativo, aunque pueden adaptarse características del otro según se necesite, en este caso creo que incluso solo con aplicar el segundo es suficiente, sobre todo por la naturaleza del problema, en donde la conexión de los elementos que conforman una isla puede ser tanto de forma horizontal como vertical. Lo que pude observar en este ejercicio, es que yo tenía asociado los métodos que vimos en las primeras clases con los ejercicios que estábamos resolviendo para encontrar islas también, creo que, entrando en contexto con la inteligencia artificial, estas características también podrían ser aprendidas y aprovechadas para resolver el problema.



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
