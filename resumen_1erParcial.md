# Resumen para el primer parcial de Ingenería de Software

## Ciclo de vida del software

Establece el proceso de transformación de una idea hasta convertirse en una aplicación complementamente definida.

**Etapas del ciclo de vida**

1. *Definición:* En esta etapa se recolectan las peticiones del cliente por parte de un analista para diseñar, unn vez terminada la recolección de requisitos, un diagrama que exprese dichos requisitos de una manera clara para el interesado.

2. *Análisis:* En esta fase el analista realiza un modelo en base a los diagramas construidos en la etapa anterior el cual represente de forma coherente las peticiones del cliente. El analista debe plantear diferentes soluciones con el fin de buscar la que más se adecúe a la peticiones y que, además, esté dentro del presupuesto.

3. *Diseño:* En esta etapa se deciden las herramientas con las cuales se van a llevar  a cabo el proyecto, es decir, se escoge el lenguaje de programación, la BD, la arquitectura que tendrá el proyecto, entre otros requisitos no funcionales. Además, se diseña la documentación del software a entregar.

4. *Implementación:* Esta etapa es meramente ejercida por los respectivos desarrolladores, los cuales se guiarán  de los modelos realizados en las etapas anteriores. Para minimizar las incoherencias, se recomienda que el diseño esté completamente finalizado.

5. *Validación:* En esta etapa toma importancia tanto el _testing_ como el _debugging_ con el objetivo de detectar errores (testing) en diferentes partes del software (o documentación) y, en caso encontrar errores, resolverlos(debugging) antes de la entrega al cliente.

6. _Mantenimiento:_ Esta etapa está enfocada en el qué pasa después de entregado el producto. Aquí se intentan corregir errores detectados por los cliente o implementar nuevas características que los cliente quieran para sus productos.

## Mitos del Software

Se denomina _mitos del software_ a las diferentes creencias erróneas sobre el proceso que se utiliza para obtener un producto.

**Tipos de mitos:**

1. _Mitos de gestión:_ 
   
   1. Se está inviertiendo tiempo considerablemente valioso en el análisis y diseño del producto, ¿Por qué invertir ese tiempo en la implementación y validación del producto?
   
   2. No abrazar el cambio. ¿Por qué se debe cambiar la forma en la que se están desarrollando los productos si se tiene implementada desde hace 15 años y nuestro producto es el mismo?

2. _Mitos del cliente:_ 
   
   1. No se tiene la necesidad de llegar a un grado de detalle mayor, solo con  una declaración general de lo que se quiere es necesario para que se empiece a programar.
   
   2. Los requisitos del proyecto cambian continuamente, pero los cambios se pueden acomodar fácilmente debido a que el software es flexible.

3. _Mitos de desarrollador:_ 
   
   1. El trabajo del progamador finaliza una vez entregado el producto funcional.
   
   2. No existe una forma de medir la calidad del producto hasta la fase de implementación, una vez corriendo ya el producto.
   
   3. El programador cumple con entregar el producto funcional, sin importar la documentación acerca de cómo se usará ese producto. Además no se hará cargo de problemas una vez entregado el producto.

## Construcción por prototipos

El prototipo es una imagen a semejanza del producto final. Generalmente es usado para la verificación de los requerimientos exigidos por el cliente. Estos prototipos se pueden clasificar en dos tipos: _baja fidelidad_ y _alta fidelidad_. Los prototipos de _baja fidelidad_ son usados en las primeras partes del desarrollo del proyecto debido a que no se construye con las mismas herramientas que tendrá el producto final. Por otra parte, los prototipos de _alta fidelidad_ ya es una imagen más real del producto final y estos sí se desarrollan con las mismas herramientas.

Los _principales usos_ de los prototipos son:

- Verificación de posibles riesgos en la estructura del sistema.

- Exploración de futuras mejoras en el producto.

- Herramientas de aprendizaje.

Las _limitaciones_ de este tipo de construcción son:

- Debido a que el prototipo es solo una pequeña imagen del producto final, a este le pueden faltar características principales que el producto final debe tener, lo cual conlleve a generar ambigüedades.

- Puede llegar a consumir muchos recursos humanos del proyecto.

Esta _construcción_ es realizada en cinco fases:

1. _Recopilación y refinamiento de datos:_ Se recopilan los requisitos exigidos por el cliente y se realiza la planificación.

2. _Diseño rápido:_ Se realiza el modelo en base a los requisitos ya recopilados, basándose en la estructura del prototipo a desarrollar.

3. _Evaluación del prototipo:_ El cliente es el encargado de evaluar el prototipo una vez finalizado. Este verificará que estén los características fundamentales de lo que él o ella exigió.

4. _Refinamiento del prototipo:_ Una vez obtenida el feedback del cliente, se siguen a implementar o eliminar las características que el cliente detectó que faltaban o sobraban. 

_Ventajas:_

- Incrementa las posibilidades de entregar un producto final más coherente a las peticiones del cliente.

- Al reducir las posibilidades de incorencia entre el producto final y los requerimientos, también se reduce los posibles costos por correción de errores e incrementa las probabilidades de éxito.

_Desventajas:_

- Los clientes se pueden crear falsas expectativas acerca del producto final.

- Con el fin de agilizar el proceso de prototipado, se pueden llegar a tomar decisiones a la ligera que no tiene nada que ver con los requerimientos del cliente.

## Modelo Lineal Secuencial

Propuesto por Winston Royce, este modelo sugiere un enfoque sistemático del desarrollo del software. Consiste en ejecutar secuencialmente una serie de fases deben quedar bien documentadas para la ejecución de una próxima fase. Estas fases no empiezan sin que al anterior haya culminado.

Las _fases_ en las que se basa este modelo son las siguientes:

1. _Ingenería del software_: Analizar el funcionamiento del sistema por medio de diagramas y descripcioness en lenguaje natural. Si se trata de un sistema nuevo, se identifican lo requerimientos del cliente; si se trata de un sistema existente, verificar cuáles pueden ser las posibles características que puede ser automatizadas. 

2. _Análisis:_ En esta fase se requiere conocer los datos que se van a manejar en la aplicación, como además las interfaces que se van a desplegar entre otros requisitos no funcionales. Estos requerimientos deben estar documentados con el fin de que el cliente los revise y verifique que sí son los que él pidió.

3. _Diseño:_ En esta etapa se traducen los requerimientos y se obtienen unos modelos que describan la arquitectura, la funcionalidad y, en algunos casos, la calidad del producto. Se especifican también las estructuras de los datos, sus programas e interfaces.

4. _Codificación:_  Todos los diagramas son traducidos a código fuente en un lenguaje de programación previamente seleccionado.

5. _Prueba:_ En esta fase se verifican que las funcionalidades principales estén realizando su trabajo tal y como lo espera el interesado. En caso de detectar una anomalía en el proceso, se empieza el respectivo _debugging_ de este error.

6. _Utilización:_ El software es entregado a el cliente y comienza su vida útil

7. _Mantenimiento:_ En esta fase se pueden mejorar características en base a las opiniones de los usuarios finales como también añadir nuevas características por decisión del cliente.

_Ventajas:_

- La buena documentación en cada etapa permite tener un producto mucho más entendible para los demás, tanto desarrolladores como usuarios finales.

- Facilita la gestión del desarrollo

_Desventajas:_ 

- Obtener todos lo requerimientos del producto al inicio del proceso suele ser algo casi imposible debido a que a veces ni el cliente sabe qué es lo que quiere del todo.

- Dificultad para alterar el diseño del proyecto debido a los altos costos que esto conllevaría.

- Suelen darse discrepancias entre lo que quería el cliente y lo que se le entregó debido a que el cliente no es un actor que está en constante comunicación, sino la retroalimentación se realiza en las fases tardías del desarrollo.

## Modelo Espiral

Este modelo, propuesto  por Barry Boehm en 1986 en su artículo "A Spiral Model of Software Development and Enhancement", también conocido como _desarrollo o modelo incremental_ surge como una alternativa al modelo secuncial, es decir, es otro modelo de ciclo de vida del software. Este modelo describe el ciclo de vida del software por etapas y una espiral en la cual el producto se trabaja continuamente con el objetivo de que los tiempos entre mejoras sean cortos. Este modelo se enfoca en la _iteratividad_ y en el _análisis de riesgos_, así como también en el proceso secuencial, el cual se repite varias veces hasta alcanzar el objetivo.

Con el objetivo de explicar en qué funciona este modelo, primero se deben tener en cuenta que existen tres tipos de modelo espiral:

1. _Clásico:_ consiste en pasar las cuatro fases por ciclos iterativos y evolutivos. La complejidad del producto incrementa en cada iteración, es decir, aumentará el tiempo de ejecución así como el volumen del código fuente generado y la gestión de riesgos y planificación. Estas cuatro fases son: _Planeación_, _Análisis de riesgo_, _Ingeniería o implementación_  y _evaluación_. Este modelo finaliza una vez entregado el producto final.

2. _6 Regiones:_ En teoría es similar al modelo planteado originalmente por Boehm, sin embargo en esta variante se intenta hacer mayor hincapié en determinadas áreas que estaban más aísladas en el modelo clásico. Se agregan más regiones y se divide en dos la etapa de desarrollo, lo que brinda una mayor precisión en las planificación. Esta variante no se limita a la entrega del producto, sino que brinda un mantenimiento del producto una vez entregado. Las regiones de las que se hablan son: _Comunicación con el cliente_, _Planificación_, _Análisis de Riesgo_, _Ingeniería_, _construcción y adaptacón_, _evaluación del cliente_.

3. _WinWin:_ Basado en la teoría W, en donde se cree que un sistema es éxitoso si todas las partes involucradas en él también lo son. Esta variante añade tres etapas al modelo clásico al inicio de cada ciclo. Estas nuevas etapas son: _Identificación del sistema_, _determinación de las condiciones de victoria de los directivos_, _negociación de la etapa anterior para reunirlas en un conjunto de condiciones para todos los afectados._ Incluye además tres objetivos temporales del proceso: _Objetivos del ciclo de vida_, _Arquitectura del ciclo de vida_, _Capacidad operativa inicial_.

_Ventajas:_

- Es especial para proyecto muy grandes en donde el riesgo es muy alto.

- Minimiza los riesgos en el desarrollo del producto.

- Flexibilidad a la hora de combinar con otros modelos del ciclo de vida.

- Estimula el desarrollo rápido de versiones estrechamente conectadas.

- Se obtiene una retroalimentación por parte del cliente, desarrollador y usarios en las primeras fases del proyecto.

_Desventajas:_

- Puede darse la posibilidad de generar bucles en el proceso de minimización de riesgos.

- Controlar este tipo de proyectos puede ser complejo debido a la evolutiva complejidad del modelo, lo cual conlleva a mantener una buena documentación donde queden registrados los cambios.

- Debido a que estos riesgos tiene un impacto monetario considerable para el bolsillo del interesado, se debe tener un constante control de los presupuestos.

## Diagrama de Casos de Uso - UML

Son una herramienta que ayuda a capturar los requisitos funcionales del sistema. Este permite ver rápidamente la _funcionalidad_ del sistema como también los actores involucrados con una respectiva función.

El principal elemento de los CU son lo actores los cuales representan modelos de los usuarios potenciales del sistema que realizan un intercambio de información. Estos actores se clasifican en:

- _Actores Principales:_ Quien inicia un CU e interacción directamente con el sistema.

- _Actores Secundarios:_ Encargados de mantener o supervisar el sistema.

- _Actores Pasivos:_ son los interesados en el caso de uso.

_Pasos para definir un CU_:

1. Elegir los límites del sistema.

2. Identificar actores principales.

3. Identificar las tareas que realizan.

4. Escribir los casos de uso.

Existen una _relaciones_ entre casos de usos que juegan un papel importante en este diagrama:

1. _Herencia_.

2. _Inclusión_.

3. _Extensión._

## RUP

Proceso iterativo para el desarrollo del software que no cuenta con unos etapas firmementes establecidas, en cambio se cuenta con un conjunto de metodologías adaptables al contexto y las necesidades de la empresa. Es usado mayormente en sistemas orientados a objetos, en cualquiera de sus etapas. Surgió como una mezcla entre un proceso llamado *Rational Approach* y otro proceso llamado *Objectory*. La primera versión fue llamada *Rational Objectory Process*.

*Principios del desarrollo*:

- *Adaptar el proceso:* se debe acomodar a las necesidades del interasado. Se deben establacer las características, las regulaciones y el alcance del proyecto.

- *Equilibrar prioridades:* Los requerimientos del producto debe llevar a un nivel en el cual se satisfagan los deseos de los interesados.

- *Demostrar valor iterativamente:* Una parte del proyecto es entregada al cliente y recibe retroalimentación en cada etapa iterativa.

- *Colaboración entre equipos:* El desarrollo se realizan en múltiples equipos.

- *Enfocarse en la calidad:* El control de la calidad no se realiza al final de la etapa de producción, sino que se realiza en cada iteración del proceso.

- *Elevar el nivel de abstracción:* Estimula el uso de esquemas para presentarle información al cliente.

_Ciclo de vida_ del RUP

- _Fase de inicio_: Las iteraciones realizadas en esta fase se enfocan más en el modelado del negocio y en los requisitos del sistema
- _Fase de elaboración_: Las iteraciones se enfocan en el desarrollo de una infraestructura, del análisis y el diseño del producto.
- _Fase de construcción_: Por medio una serie de iteraciones se construye el producto a entregar.
- _Fase de transición_: Se pretende tener un producto preparado para su entrega al respectivo cliente.

_Características principales_: 

- Forma disciplinada de repartir tareas.

- Implementa las mejoras prácticas de la IS para adaptarse mejor a las necesidades del cliente.

- Desarrollo iterativo.

- Control sobre los cambios realizados en el producto

- Modelado visual del producto

- Control de calidad del software

- Identifica los casos de uso

_Fases_:

- _Inicio:_ En esta fase se ponen en la mesa los riegos del proyecto con una definición previa del alcance del proyecto. Además de producir un plan para las fases e iteraciones siguientes.

- _Elaboración:_ Se diseña una arquitectura del sistemas como también se diseña una solución previa. Esto se gracias a una selección previa de los casos de uso.

- _Desarrollo:_ Se completa el proceso de construcción materializando los que en las fases anteriores se acordó.

- _Cierre:_ Asegurar que el software esté disponible para los usuarios finales, como tambíen corregir posibles errores y capacitar a los usuarios.

_Ventaja_

- No es necesario tener todos los requisitos en el primer encuentro con el cliente.

- El testeo se hace por componentes individuales.

- Se tiene una retroalimentación directa del cliente en cada iteración.

## SCRUM

Es una metodología ágil en donde su principal objetivo es controlar y planificar proyectos con constantes cambios y donde se maneja una gran incertidumbre. Surge en 1986 en un artículo llamado "The New Product Development Game" de Takeuchi y Nonaka.

Las principales _características_ de esta metodología son:

- _Transparencia:_ Todos los involucrados deben tener conocimientos generales de lo se hace en el proyecto.

- _Inspección_ Se inspecciona frencuentemente el progreso para verificar que no se presente inconsistencias.

- _Adaptación_  Se le da acogida al cambio.

Los ciclos en SCRUM son llamados _sprints._ 

Los artefactos involucrados en esta metodología son: _Product Backlog_ (Requerimientos del producto), _Sprint Backlog_ (Requerimientos de la iteración) y los _Incrementos_ (Añadidos que se realizan en cada sprint)

Se cuentan con tres roles importantes: _Scrum Master_, _Dueño del producto_ y --_Equipo de desarrollo_

_Desarrollo de la metodología_:

- _Planificación del sprint_ y aquí se hace la selección de requisitos y la planificación del sprint.

- _Ejecución del sprint_: se realiza una sincronización del trabajo realizando por parte del equipo de desarrollo.

- _Inspección y adaptación:_  Se presenta los requisitos completados al cliente (_Revisión_) y se realiza un análisis acerca de la iteración que acaba de pasar (__Retrospectiva_)

_Ventajas_:

- Agiliza procesos.

- Flexible al cambio.

- Reducción del tiempo a producción.

- Maximiza el retorno de la inversión.

_Desventajas_:

- Difícil implementación.

- Camino corto no siempre conlleva a mayor calidad.
