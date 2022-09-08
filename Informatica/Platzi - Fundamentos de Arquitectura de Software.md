# Fundamentos de Arquitectura de Software.

---

## Etapas del proceso de desarrollo de software.

````mermaid
flowchart LR
Análisis_de_Requerimientos. --> Diseño_de_la_Solución. --> Desarrollo_y_Evaluación. --> Despliegue. --> Mantenimiento_y_Evolución.
````

### Análisis de requerimientos.

Los requerimientos son todas aquellas características y funcionalidades que un producto debe de poseer para poder solucionar una necesidad específica, dando como resultado una comprensión muy clara del producto y de la problemática a resolver.

#### Requerimientos de usuario.

#### Requerimientos de negocio.

#### Requerimientos funcionales.

#### Requerimientos no funcionales.



### Diseño de la solución.

Análisis profundo del problema, y una propuesta de diseño de una solución. Es la propuesta a nivel de diseño de la solución, en donde se plantea y concretan las posibles soluciones tanto en modelo, documentación, alternativas de productos y herramientas y detalles específicos de la solución.

El resultado de esto es un esquema detallado de la solución tanto en documentación, modelado, diseño, etc. 



### Desarrollo y evaluación.

Etapa en la que se desarrolla y construye el software en función de los criterios de aceptación ya especificados.

__Criterios de aceptación de la solución__: Es el set de requerimientos necesarios para construir la solución y la manera en la que se evaluarán. 



### Despliegue.

Se pone a disponibilidad del usuario final la solución construida, todo esto a través de una infraestructura especializada  controlada y mantenida por un equipo de operaciones quienes se aseguran de llevar y mantener el producto en producción, es decir, a disponibilidad del usuario final.



### Mantenimiento y evolución.

Es una etapa donde se regresa continuamente a las etapas previas de desarrollo y evaluación y luego a la de despliegue, ya que consiste en estar continuamente mejorando el producto y atentos a la detección de errores, para poder cambiar el software y colocarlo de nuevo a disponibilidad del usuario, todo esto se repite hasta que el software deje de ser necesario y su ciclo de vida termine.

---



## Dificultades en el desarrollo de software.

[No hay balas de plata - Wikipedia, la enciclopedia libre](https://es.wikipedia.org/wiki/No_hay_balas_de_plata)

[Ensayo — “No Silver Bullet” de Frederick P. Brooks, Jr. | by Jose Alejandro Gómez Castro | Medium](https://josegomezdev.medium.com/ensayo-no-silver-bullet-de-frederick-p-brooks-jr-e11c6884677d)

### Problemas esenciales.

Especificación, diseño y comprobación del concepto.

> Entender el concepto de lo que queremos desarrollar y su diseño.

#### Complejidad.

#### Conformidad.

#### Tolerancias al cambio.

#### Invisibilidad.

### Soluciones esenciales.

#### No desarrollar.

En cambio optar por adquirir una solución ya existente, ya sea privada o de código abierto, o conseguir una herramienta, del tipo que sea, que permita adelantar lo más posible su desarrollo.

#### Prototipado rápido.

Como podrían ser las metodologías ágiles, donde la idea es obtener información lo antes posible sobre si estamos resolviendo el problema correcto y de la forma adecuada, para ello el sistema va evolucionando de forma paulatina y a traves de cambios pequeños en función de las referencias e información aportada por el usuario.

#### Desarrollo evolutivo.

Más alineado a la creación y acumulación de sistemas, donde se intenta obtener resultados pequeños que poco a poco vayan evolucionando, muy alineado tambien con las metodologías agiles. 

#### Grandes diseñadores.

Son desarrolladores que saben como abstraerse del problema específico y entender las generalidades del mismo, sabiendo diseñar una solución elegante y simple al resolver de la mejor forma el problema.



### Problemas accidentales.

Detalles de la implementación y producción actual.

> Plataforma, lenguaje, framework y su integración.

#### Lenguajes de alto nivel.

#### Multiprocesamiento.

#### Entornos de programación.

---



## Objetivos del arquitecto.

El arquitecto tiene varias partes interesadas (o _stakeholders_) las cuales tienen necesidades independientes y especificas, y el papel del arquitecto es poder conectar estos requerimientos con la implementación del sistema.

Las partes interesadas con sus distintos requerimientos son:

- __Cliente:__ Obtener un sistema que se amolde al presupuesto y a los tiempos acordados.
- __Manager:__ Asociado a los requerimientos del cliente, desarrollar el software de manera independiente, formar equipos con capacidad de autogestión y una comunicación clara entre los equipos que participan en el desarrollo del sistema.
- __Desarrolladores:__ Fácil implementación y mantenimiento, caracteristicas dependientes de la flexibilidad y escalabilidad.
- __Usuario:__ Disponibilidad y confiabilidad del sistema.
- __Q.A:__ Fácil testeo y comprobación de calidad.

El arquitecto de software debe gestionar los siguientes requerimientos de para cada parte interesada:

- __Cliente:__ Encontrar los riesgos más altos que afecten en el desarrollo del sistema.
- __Manager:__ Modularización y flecibilidad del sistema que se está desarrollando.
- __Desarrollador:__ Modularidad, mantenibilidad y capacidad de cambio del software.
- __Usuario:__ Decidir estrategias para la dispobibilidad del sistema. 
- __Q.A.:__ Que el sistema pueda ser modularizado y cada una de estas partes pueda ser probada de forma sencilla. Que el sistema pueda responder de forma consistente, que pueda ser modularizado y que dichos módulos puedan ser probados independientemente.

La unión de estos requerimientos, tanto funcionales como no funcionales, va a llevar al arquitecto a tomar decisiones que impactan directamente en el desarrollo del software.

---



## Entender el problema.

Al momento de rocopilar requerimientos y procesarlos, es importante entender el problema que se pretende resolver. La parte más importante es separar la comprensión del problema de la propuesta de solución, ya que al no ser capaces de separar dichos aspectos, se puede caer en el error de percibir ciertas caracteristicas como la plataforma, el framework, la arquitectura general, etc, como parte del problema, cuando en realidad son detalles de implementación.

### Espacio del problema.

#### Idea.

Aquí se plantean preguntas como: ¿Qué es lo que vámos a hacer? ¿Qué es lo que se quiere resolver? ¿Cual es la problemática identificada que podemos solucionar con la implementación de un proyecto de software?

#### Historias de usuario.

Es la historia o la narrativa de como un usuario, a traves de la solución a desarrollar, puede llegar a tener una experiencia que resuelva su problemática. No se habla del sistema sino que se describe el problema que se quiere resolver, detallando esta problemática e intentando describir la solución.

#### Criterios de Éxito.

Luego de entender el problema a resolver y delimitarlo, entendiendo por supuesto su alcance y aquellas otras problemáticas fuera del proyecto y de las intenciones del mismo, se pasa a listar aquellas características o acciones que resolverían las necesidades del usuario.



### Espacio de la solución.

Es un reflejo del espacio del problema, ya que toma en cuenta su narrativa para luego intentar solventarla a través de un planteamiento técnico. 

#### Diseño.

Todo lo referente a la planificación del software, desde el diseño de la interfaz, la experiencia de usuario, hasta el diseño del sistema.

#### Desarrollo.

#### Evaluación.

#### Criterios de aceptación.

Son características que relacionan las funcionalidades del software con las necesidades descritas y demandadas por el usuario. Se describen criterios para coordinar y alinear el proyecto y sus funcionalidades con el usuario y la problemática que este puede poseer y que se pretende solventar.

#### Despliegue.

---



## Requerimientos.

### Requerimientos de producto.

```mermaid
flowchart RL
	
	Requerimientos_de_usuario --> Requerimientos_funcionales
	
	Atributos_de_calidad --> Requerimientos_no_funcionales
		
    subgraph Funcional.
    Requerimientos_de_sistema --> Requerimientos_funcionales
    Restricciones
    end
    
    subgraph Usuario.
    Requerimientos_de_usuario-->Atributos_de_calidad
    Requerimientos_no_funcionales
    end
    
    subgraph negocio.
    Reglas_de_negocio --> Requerimientos_de_negocios
    Reglas_de_negocio --> Requerimientos_de_usuario
	Reglas_de_negocio --> Atributos_de_calidad
	Reglas_de_negocio --> Requerimientos_funcionales
	
	Requerimientos_de_negocios --> Requerimientos_de_usuario

    end
```

Los __requerimientos de producto__ se separan en tres grupos o capas: __requerimientos de negocio__, __requerimientos de usuario__ y __requerimientos funcionales__.

> __Regla:__  
>
> - Principio o fórmula sobre la manera de hacer una cosa.
> - Conjunto de principios o normas que indican cómo comportarse.
> - Modo de ejercer o de ejecutar una cosa.
>
> __Requerimiento:__
>
> ​	__Requerir:__
>
> -  Pedir una cosa la autoridad.
> - Tener una persona o una cosa necesidad de otra.

- __Negocio:__ Las __reglas de negocio__ son aquellos requerimientos que forman el núcleo o la esencia de la solución, es decir, son todas aquellas funcionalidades y características que le dan forma y sentido a la funcionalidad y que le permiten poder solventar la problemáticas en cuestión.
  Estas __reglas de negocio__ siguen siendo funcionalidades o características inespecíficas que alimentarán a los requerimientos de negocio (y a muchos otros requerimientos del producto) al poder brindarle una descripción general de la solución al problema que luego tendrá que ser concretada en los __requerimientos de negocio__.
  Por ejemplo, una __regla de negocio__ puede ser el poder ofrecerle hospedaje seguro y económico a las personas como alternativa a los costosos hoteles al conectar a los arrendadores con los turistas, y el __requerimiento de negocio__ sería el poder conectar a ambas partes generando diferentes roles de usuario con características bien definidas. 
  Estas __reglas de negocio__ condicionan e interceden en todas las capas del requerimiento de producto, ya que describen las funcionalidades esenciales del producto, la manera en la que se debe de comportar para lograr solventar la necesidad que se tiene identificada.
- __Usuario:__ Los __requerimientos de usuario__ tienen que ver con la manera en la que el usuario se puede desenvolver usando el sistema, estos requerimientos, los de usuario, también tienen que ver con los atributos de calidad, los cuales condicionan a los __requerimientos no funcionales__, ya que determinan la manera en la que el usuario interaccionará con la solución, sus tiempos de espera, las garantías de seguridad (un __atributo de calidad__), recolección de información, etc.
- __Funcional:__ Estos se alimentan de los dos requerimientos previos y su propósito es bajar a tierra, concretar, las funcionalidades, aquí se dejan de lado las historias genéricas, los valores de negocio o las estrategias generales, en este paso hablamos puntualmente de que es lo que hay que hacer en este sistema en concreto para implementar una funcionalidad en concreto.
  Los __requerimientos funcionales__  se alimentan de los __requerimientos de sistema__ en la medida en la que estos describen lo que tiene que pasar operativamente para poder realizar dicho __requerimiento funcional__,
  Los __requerimientos funcionales__ también determinan las restricciones del sistema, como los permisos de acceso de cada tipo de usuario, las restricciones de comunicación, restricciones de conectividad, etc. Todo esto tiene que ver con las restricciones contextuales de los requerimientos.

Los requerimientos de producto se pueden separar en __funcionales__ y __no funcionales__. 

Los __funcionales__ detallan específicamente como el sistema se va a comportar. Los requisitos funcionales establecen los comportamientos propios del software.

Los __no funcionales__ representan características generales y restricciones de la aplicación o sistema a desarrollar, son las expectativas que se tienen de las funcionalidades. Se pueden entender como aquellas características relativas al rendimiento, eficiencia e interacción con el usuario, como podría ser el poder manejar una $n$ cantidad de peticiones, permitir el acceso a los usuarios en un lapso especifico y corto de tiempo o que toda funcionalidad del sistema y transacción responsa en menos de $n$ segundos.



### Requerimientos de proyecto.

Estos requerimientos tienen más que ver con el rol de gestor de proyecto, a pesar de que el arquitecto tiene que estar al tanto de estos requerimientos y poder trabajar en conjunto con el gestor de proyecto para poder entender y priorizar ambos requerimientos, los de proyecto y los de producto, ya que a mbos se condicionan.

De entre todos los requerimientos de proyecto podríamos destacas los siguientes:

- __Recursos.__
- __Capacitación.__
- __Certificaciones.__
- __Documentación de usuario.__
- __Infraestructura.__
- __Licencias.__
- __Plan de despliegue.__
- __Plan de transición.__
- __Acuerdos de servicio.__

Estos requerimientos describen todas aquellas características y recursos que harán falta para poder llevar a cabo el proyecto.

---



## Riesgos.

La implementación de cualquier sistema incurre en riesgos específicos propios de dicho sistema, ya que no existe un sistema o una arquitectura perfecta e infalible, es importante tener en cuenta todos los riesgos en los que se incurren. 

Estos riesgos van a ser importantes para poder priorizarlos y poder solventarlos en orden y que eso nos garantice que las soluciones arquitectónicas que estamos tomando solucionen los problemas más importantes, y no cualquier problema que se cruce en el camino. 

### Describir el riesgo.

Usar escenarios de fracaso que sean medibles y accionables. 

#### Riesgos de ingeniería.

Relacionados con el análisis, diseño e implementación del producto.

#### Riesgos de gestión del proyecto.

Relacionados con la planificación, secuenciamiento de trabajo, entregas, tamaño de equipo, etc.



No es posible cubrir todos los riesgos en un primer momento, por lo que es fundamental tener la capacidad de priorizar los riesgos para poder cubrir aquellos que se consideren más acuciantes y puedan generar mayores daños, ya que el no saber priorizar de manera acertada podría hacer que se solventen riesgos menores dejando al descubiertos potenciales fallos de un mayor nivel. 

En cuanto a priorizar, la ley de Pareto es sumamente útil, ya que generalmente el el 80% de todos los daños sufridos por un sistema vienen del 20% de las vulnerabilidades del mismo.

![Preview](https://cdn.exceltotal.com/wp-content/uploads/2011/09/diagrama-de-pareto-en-excel-01.png)

---



## Restricciones. 

> Una restricción limita las opciones de diseño o implementación disponibles al desarrollo. 

Las restricciones en el contexto de un proceso de desarrollo de software tienen que ver con limitaciones en las opciones que tendremos, tanto de diseño como de implementación. 

El contexto, en general, está dado por las partes interesadas (los ___stakeholders___), los cuales colocan limitaciones relativas a su ecosistema, su contexto de negocio, regulaciones, normas legales, etc. También habrá limitaciones debido a la integración con otros sistemas, ya que esta comunicación condicionará y por consiguiente restringirá ciertas posibles características del desarrollo, como el tipo de protocolo de comunicación o la vía por la que se efectuará la comunicación. Por ultimo está el ciclo de vida del producto, el cual irá gradualmente agregando restricciones a medida que va evolucionando la aplicación, ya que el modelo de datos se va volviendo cada vez más rígido y difícil de cambiar.  

---



## Estilos de arquitectura.

Un estilo de arquitectura es un modelo genérico de estructura en donde no se habla en detalle sobre el problema que resuelve el dominio, sino que hable de que problema se está resolviendo arquitectonicamente a nivel de los conectores entre diferentes aplicaciones, entre dos sistemas, entre usuarios, etc. Todo esto define algo genérico que si nos permite reutilizar, en diferentes softwares, un estilo que nos ayuda a poder reutilizar estos esquemas. 

> Un estilo de arquitectura es una colección de decisiones de diseño, aplicables en un contexto determinado, que restringen las decisiones arquitectónicas específicas en ese contexto y obtienen beneficios en cada sistema resultante.

Los estilos de arquitectura toman los esquemas previos que ya otras soluciones utilizaron en el pasado y describieron como útiles y eficaces y los estandariza y esquematiza en plantillas aprovechables para que otras personas con problemáticas generales similares las puedan aprovechar. 

---

## Flujo de datos.

### Llamada y retorno.

  ```mermaid
  flowchart BT
  
  Programa_principal\ny_subrutinas.
  
  Orientado_a_objetos.
  
  Multi-nivel.
  
  Cliente-Servidor --> Multi-nivel
  ```

### Flujo de datos.

```mermaid
flowchart BT

Lote_secuancial

Tubos_y_filtros.
```

---



## Centradas en datos.

### Pizarrón.

El pizarrón es el núcleo de la arquitectura, en donde cada componente externo a él se encargarán de procesar el dato y escribirlo en el pizarrón, el cual funciona como centralizador de la información. Cuando el pizarrón ya tiene todos los datos necesarios, este mismo podría generar una salida.

```mermaid
flowchart TB

Process_1 --> blackboard

process_2 --> blackboard

Process_3 --> blackboard

process_4 --> blackboard

blackboard --> Out-Put.
```

### Centrada en base de datos.

Un estilo común; se trata de que una cantidad de componentes comparte una misma base de datos, los cuales pueden ser desplegados al unisono y consumir de la misma base de datos, como por ejemplo una API, la cual está compuesta por varios componentes dentro de un mismo sistema, o también podrían ser componentes desplegados de forma independiente y que consumen la misma base de datos.

```mermaid
flowchart TB

Component_1 --> B.D.

Component_2 --> B.D.
```

### Sistema experto o basado en reglas.

Un componente A (tipo cliente) consulta a uno B, donde este se encargará de tratar de entender si la petición del cliente es una consulta o una regla. Para que el componente B logre resolver la petición se va a comunicar con un tercer componente C, el cual trabajará como una __KDB__ (_Knowledge DataBase_).

```mermaid
flowchart TB

Client --> Inferir_Regla

Inferir_Regla --> Rule

Inferir_Regla --> Query

Inferir_Regla --> Knowledge_Base

```



## Componentes Independientes.

En este estilo se desarrollan aplicaciones de forma independiente, en donde no existe un fuerte acoplamiento entre los componentes.

Hay dos grandes familias dentro de este tipo de arquitectura, definidos por la manera en la que se comunican los componentes del sistema,y estos son los de __invocación implícita__, la cual suele ser basada en eventos y donde las aplicaciones se mandan mensajes entre si sin que estas conozcan exactamente con quien está hablando; y el tipo de __invocación explícita__ habla de como desarrollar componentes que si se conozcan entre si pero estén desarrollados independientemente.

### Invocación implícita.

En general cuando tenemos eventos, lo que tenemos son varios componentes y tenemos además un BUS de eventos, en el cual los componentes publican o escriben eventos y luego el BUS los notifica a los componentes interesados en dichos eventos.



Se tienen varios componentes y se cuenta con un BUS de eventos en el cual los componentes van a escribir algunos eventos y luego el BUS los comunica a los componentes a los que les conciernan dichos eventos.

```mermaid
flowchart BT

Públicar-Suscribir --> Basado_en_eventos

Orientado_a_servicios_2.0 --> Basado_en_eventos

Basado_en_eventos --> Invocación_implícita
```





Respecto a los __BUS de eventos__, tenemos dos tipos:

- __Publicar suscribir:__ El componen inicial publica un evento y luego otros componentes están suscritos y reciben dicho evento.

  ```mermaid
  flowchart TB
  
  Componente_publica --> BUS
  
  BUS --> Componenete_suscribe
  ```

  

- __Orientación a servicios:__ Tienen un BUS inteligente al que se le notifica a través de eventos al BUS y este es el que decide a quien le envía instrucciones. En este esquema los componentes no se conocen entre ellos, y se comunican utilizando al BUS como intermediario.

```mermaid
flowchart TB 

Enterprise_service_BUS --> Component_1
Component_1 --> Enterprise_service_BUS

Enterprise_service_BUS --> Component_2
Component_2 --> Enterprise_service_BUS

Enterprise_service_BUS --> Component_3
Component_3 --> Enterprise_service_BUS
```



### Invocación explícita.

Los componentes se desarrollan separados, pero estos se conectan entre si, lo que significa que los componente de alguna forma deben publicar cual será la vía de comunicación que tienen disponible. Estos componentes se registran en un punto central y luego determinan la forma en la que se van a comunicar entre si. 

```mermaid
flowchart BT

Orientado_a_servicios_1.0 --> Invocación_explícita
```

---



## Comparación de estilos.



### Monolíticos.

- Se despliega un solo artefacto de software.

- Se le da prioridad a la eficiencia de ejecución al tener un solo artefacto de software el cual está optimizado y con una comunicación interna bastante detallista y eficiente.
- Son más fáciles de probar de principio a fin.
- La curva de aprendizaje es menos pronunciada.
- Todas las piezas constituyentes del sistema se encuentran en el mismo lugar.
- Más fácil de modificar, ya que el cambio de un componente interno solo afectará a la misma estructura que lo aloja. 

### Distribuido.

- Cada despliegue es independiente aunque interconectados. 
- Son más difíciles de probar de principio a fin ya que deberíamos tener todos los componentes disponibles e incluso un BUS disponible en el caso de eventos.
- La curva de aprendizaje es mucho más pronunciada.
- El sistema está compuesto por componentes independientes y separados los cuales habrá que entender de forma separada.
- Los cambios son más difíciles de realizar, ya que al modificar un componente se pueden ver afectados otros componentes que dependan de el. 
- Es un sistema modular en donde se pueden desplegar los componentes de manera independiente.
- Su disponibilidad es mayor ya que se pueden hacer copias de los componentes, los cuales tienen un tamaño significativamente menor, lo que optimiza recursos.
- Fácil de escalar.
- Mucho más adaptable para desplegar en contextos diferentes. 

---



## Examen.

## Estas son tus respuestas

### Puedes revisar y cambiar las respuestas. Al terminar presiona “Calificar respuestas” para enviar las preguntas y conocer tu puntuación.

1.

En el contexto de metodologías tradicionales, ¿en qué etapa del proceso de desarrollo de software se toman las decisiones de arquitectura?

Diseño de la solución



2.

Y en el contexto de metodologías ágiles, ¿cuándo se toman las decisiones de arquitectura?

En cada iteración



3. X

¿Por qué no existe la bala de plata que resuelva las dificultades del desarrollo de software?

Porque siempre habrá dificultades accidentales y esenciales que se combinan de formas diferentes en cada contexto

Porque seguirán apareciendo dificultades accidentales que tienen que ver con las nuevas tecnologías que se inventan



4. X

De las formas en las que podemos trabajar con las dificultades esenciales, ¿cuál es la que más involucra a los arquitectos de software?

Todas las opciones son correctas.

Decidir si hacer el producto o comprarlo ya hecho.



5.

En el contexto de metodologías ágiles, ¿dónde encontraremos el rol del arquitecto?

En el equipo de desarrollo



6.

¿Cuál de estas definiciones mejor describe la arquitectura de software?

Es la estructura de un sistema, sus interconexiones, y las decisiones de diseño que llevaron a éstas



7.

La ley de Conway nos dice que:

El diseño del sistema va a ser una copia de la estructura de comunicación de la organización



8.

La empresa GitJam es una organización multinacional con desarrolladores distribuidos en todo el mundo. Su metodología de trabajo es principalmente remoto: No tienen oficina más allá de un pequeño headquarters en San Francisco, donde se reúnen los directivos. Los desarrolladores se comunican por email y disponen de una plataforma de chat. ¿cómo es el diseño de su sistema?

Distribuido, comunicación entre componentes principalmente asincrónica



9. 

¿Cuál de los siguientes mejor describe el objetivo de un arquitecto?

Comprender las necesidades de sus stakeholders al diseñar el sistema



10.

¿Cuál de estas prácticas es esencial para un arquitecto en contexto de metodologías ágiles? 

Reevaluar la arquitectura en cada iteración a través de métricas y alertas.



11.

En la toma de requerimientos, trabajamos para entender y definir:

El problema a resolver



12.

El usuario podrá comprar con tarjeta de crédito a través del sistema, ¿qué tipo de requerimiento es?

Funcional



13.

“El sistema incrementará nuestra capacidad de venta a clientes extranjeros en un 25%.” ¿Qué tipo de requerimiento es?

De negocio



14.

“Los precios podrán ser actualizados desde un panel de administración.” ¿Qué tipo de requerimiento es?

Funcional



15.

“El sistema deberá estar disponible para ser presentado en la conferencia de la empresa en abril de este año.” ¿Qué tipo de requerimiento es?

De proyecto



16.

“Toda interacción con el sistema debe ser compatible con usuarios con discapacidad visual.” ¿Qué tipo de requerimiento es?

No funcional



17. X

¿Cuál de los siguientes requerimientos funcionales incluye explícitamente un requerimiento no funcional?

“Se podrán canjear puntos acumulados por el uso de tarjetas de crédito por beneficios varios, a definir por el banco.”

“El administrador podrá cancelar un préstamo si detecta la posibilidad de fraude.”



18.

“El sistema podría ser atacado a través de una denegación distribuida de servicio.” ¿Qué describe esto?

Un riesgo



19.

Luego de identificar los riesgos, ¿qué hace el arquitecto con esta información?

Los prioriza para resolver sólo los más importantes



20.

¿Por qué no podemos resolver todos los riesgos detectados?

Porque dedicaremos esfuerzo que no estaremos usando para desarrollar las funcionalidades del sistema



21.

En la compañía ACME-Products quieren comenzar un nuevo producto, capaz de analizar datos de compras y comportamiento de compradores en tiempo real. En una conversación sobre requerimientos, el dueño del producto le comunica al arquitecto que deben usar la base de datos GuayabaDB, ya que tienen un acuerdo previo con la compañía que la desarrolla. ¿Qué es esto?

Una restricción de diseño



22.

¿Cuáles de estas puede ser considerada una restricción de diseño?

Hay leyes sobre la privacidad de datos que nuestro sistema almacena



23.

Un sistema contable permite a sus usuarios el mantener el estado actual de las finanzas de la organización. Además, el departamento de finanzas encargó el desarrollo de un nuevo sistema para tener reportes trimestrales, semestrales y anuales y filtrarlos por tipo de transacción. ¿Qué estilo de arquitectura es más pertinente?

Centrado en base de datos



24.

Un *ecommerce* en crecimiento quiere hacer mejor uso de sus recursos para que pueda crecer de forma más eficiente. Luego de un proceso de análisis y medición, encontraron que calcular las promociones para cada producto bloquea la mayor parte del uso de memoria del sistema. ¿Cuál de estas propuestas mejor ataca la situación?

Usar una arquitectura distribuida y separar el cálculo de promociones



25.

En los frameworks web modernos existe el concepto de middleware, que describe una forma de interceptar el pedido o la respuesta del sistema con componentes desarrollados independientes uno del otro. ¿Qué estilo de arquitectura están implementando?

Flujo de Datos: Tubos y filtros



26. X

En un centro de investigación, científicos de diferentes áreas utilizan un sistema para, a través de un modelo común de física, química y biología, simular hipótesis de procesos que se podrían haber dado durante la historia de nuestro planeta. Para esto, le deben describir al sistema los hechos que forman parte de su hipótesis y luego consultar el resultado simulado. ¿Qué estilo de arquitectura usará el sistema?

Pizarrón

Centro en base de datos



27.

De los siguientes estilos, ¿cuál es que más se usa al desarrollar aplicaciones web?

Cliente - servidor



28.

Se desarrolló un pequeño script en Python para sincronizar los logs de varios servidores. Pasó el tiempo y la cantidad de logs a sincronizar creció, y con ellos las responsabilidades del pequeño script. ¿Qué estilo de arquitectura podemos usar para mejorar esta situación?

Programa y subrutinas



29. 

Una librería desarrolló un sistema para administrar su venta y existencia de libros. Diez años más tarde, la empresa cuenta con más de 800 librerías distribuidas en 30 países de américa y europa. El sistema de administración de ventas y existencia se sigue usando para cada librería, mientras que muchos otros sistemas se encargan de la gestión global de la compañía, sus métricas por región y su expansión. ¿Qué estilo de arquitectura estamos describiendo?

Orientado a servicios



30. 

¿Cuántos estilos de arquitectura puede haber en un sistema?

Cada sistema puede tener múltiples estilos; no hay regla fija
