# Platzi - Introducción al Desarrollo Back-End

## Framework y Librerías:

​	Un __Framework__ es un conjunto de herramientas que trabajan en un proyecto completo bajo ciertas reglas. Este tiene funcionalidades integradas para que no necesitemos de librerías externas y asegura una total compatibilidad entre todas estas funciones, además de que el __Framework__ define la forma en que se debe desarrollar el proyecto.

​	Una __Librería__ es una herramienta que otorga una sola utilidad en especifico y su aplicación e instalación es de libre elección. En otras palabras, un __Framework__ es un marco de trabajo con normas, patrones de desarrollo y múltiples herramientas integradas diseñado para un fin especifico, como diseñar aplicaciones web, diseñar aplicaciones móviles, desarrollar videojuegos, etc. Mientras que una __Librería__ es una herramienta individual que sirve para resolver o un problema en especifico, como crear numero aleatorios, traducir texto, graficar, etc.

## HTTP:

> ​	HyperText Transfer Protocol

​	Es el protocolo de comunicación que permite las transferencias de información a través de archivos HTML o XHTML. Es un protocolo orientado a transacciones y sigue el esquema petición-respuesta entre un cliente y el servidor. En este caso el cliente realiza una petición enviando un mensaje, con cierto formato al servidor, y el servidor le envía un mensaje de respuesta.

​	Los mensajes tienen la siguiente estructura:

- Línea inicial (termina con retorno de carro y un salto de línea)
   - Para las peticiones: la acción requerida por el servidor ([método de petición](https://es.wikipedia.org/wiki/Protocolo_de_transferencia_de_hipertexto#Métodos_de_petición)) seguido de la [URL](https://es.wikipedia.org/wiki/URL) del recurso y la versión HTTP que soporta el cliente.
   - Para respuestas: La versión del HTTP usado seguido del código de respuesta (que indica qué ha pasado con la petición seguido de la [URL](https://es.wikipedia.org/wiki/URL) del recurso) y de la frase asociada a dicho retorno.
- Las cabeceras del mensaje que terminan con una línea en blanco. Son [metadatos](https://es.wikipedia.org/wiki/Metadato). Estas cabeceras le dan gran flexibilidad al protocolo.
- Cuerpo del mensaje. Es opcional. Su presencia depende de la línea anterior del mensaje y del tipo de recurso al que hace referencia la URL. Típicamente tiene los datos que se intercambian cliente y servidor. Por ejemplo para una petición podría contener ciertos datos que se quieren enviar al servidor para que los procese. Para una respuesta podría incluir los datos que el cliente ha solicitado.

​	HTTP define una serie predefinida de métodos de petición que pueden utilizarse. Cada método indica la acción que desea que se efectúe sobre el recurso identificado. Lo que este recurso representa depende de la aplicación del servidor.

​	__GET__: Solicita una representación del recurso especificado. Las solicitudes GET solo deben recuperar datos y no deben tener ningún otro efecto.

​	__HEAD__: Pide una respuesta idéntica a la que correspondería a una petición GET, pero en la respuesta no se devuelve el cuerpo. Esto es útil para poder recuperar los metadatos de los encabezados de respuesta, sin tener que transportar todo el contenido.

​	__POST__: Envía datos para que sean procesador por el recurso identificado en la URL de la línea petición. Los datos se incluirán en el cuerpo de la petición. A nivel semántico está orientado a crear un nuevo recurso, cuya naturaleza vendrá especificada por la cabecera _Content-Type_.

​	__PUT__: Envía datos al servidor, pero a diferencia del método POST, la URL de la línea de petición no hace referencia al recurso que los procesará, sino que identifica al los propios datos. Otra diferencia con POST es semántica, mientras que POST está orientado a la creación de nuevos contenidos, PUT está más orientado a la actualización de los mismos, aunque también podría crearlos.

​	__DELETE__: Borra el recurso especificado.

​	__TRACE__: Este método solicita al servidor que introduzca en la respuesta todos los datos que reciba en el mensaje de petición. Se utiliza con fines de depuración y diagnóstico ya que el cliente puede ver lo que llega al servidor y de esta forma ver todo lo que añaden al mensaje los servidores intermedios.

​	__OPTIONS__: Devuelve los métodos HTTP que el servidor soporta para un URL especifico. Esto puede ser utilizado para comprobar la funcionalidad de un servidor web mediante peticiones en lugar de un recurso especifico.

​	__CONNECT__: Se utiliza para saber si se tiene acceso a un host, no necesariamente la petición llega al servidor, este método se utiliza principalmente para saber si un proxy nos da acceso a un host bajo condiciones especiales, como por ejemplo “corriente” de datos bidireccionales encriptadas, como lo requiere SSL.

​	__PATCH__: Su función es la misma que PUT, el cual sobrescribe completamente un recurso. Se utiliza para actualizar, de manera parcial, una o varias partes. Está orientado también para el uso con proxy.

​	__UPDATE__: Su función es la de modificar el contenido del recurso especificado.

### 	HTTP Status Code:

[Códigos de estado de respuesta HTTP - HTTP | MDN (mozilla.org)](https://developer.mozilla.org/es/docs/Web/HTTP/Status)

![Preview](https://i.imgur.com/8Ql7ST7.jpg)

---



### Entrypoint:

​	Es la URL que el visitante habrá ingresado en su navegador para ver la aplicación o sitio web. 

### Endpoint:

​	Es una sección de la URL del proyecto. Los __endpoints__ son las URLs de un API o un back-end que responden a una petición. Los mismos  __entrypoints__ tienen que calzar con un __endpoint__ para existir. Por cada __entrypoint__ esperando la visita de un usuario puede haber socenas de __endpoints__ sirviendo los datos que se despliega en el __entrypoint__. 

> ​	URL de un servicio que utiliza un sitio web para cargar o consumir informacion

​	La diferencia entre ambos es que los __endpoints__ no están pensados para interactuar con el usuario final. Usualmente sólo devolverán JSON, o no devolverán nada. Y más que frecuentemente, un __entrypoint__ hará varias llamadas a distintos __endpoints__ para mostrar información.

​	Adicionalmente, se asume que cuando se habla de un __endpoint__ estamos en un entorno **RESTfull**, por lo cual (a diferencia del uso de un browser), el cliente *puede usar un mismo __endpoint__ con distintos verbos*.

​	La existencia de __endpoints__ usualmente es proporcional a la cantidad de entidades que quieres modelar en tu back-end o en la API. Por cada entidad debiera existir al menos un __endpoint__, y por cada uno de ellos podrías realizar las acciones de crear, leer, actualizar o borrar datos. Y luego, si consideramos que cada relación entre dos entidades da lugar a otro __endpoint__, puede que tengas muchos más.



# Examen:

1.

Si tuvieras que comparar a una aplicación web con un vehículo automotor, el frontend sería el equivalente a:

La carrocería.

CAMBIAR

2.

¿Qué es un framework?

Un conjunto de librerías y reglas para crear un producto de software.

CAMBIAR

3.

¿Qué formato de transmisión de información utiliza el patrón arquitectónico REST?

JSON

CAMBIAR

4.

¿Qué formato de transmisión de información utiliza el protocolo SOAP?

XML

CAMBIAR

5.

¿Sobre cuál de estos protocolos funciona HTTP?

HTML

CAMBIAR

6.

Una respuesta HTTP está compuesta por:

Cabeceras y un cuerpo.

CAMBIAR

7.

El conjunto de IP y puerto 127.0.0.1:8000 se conoce como:

Localhost

CAMBIAR

8.

¿Cuál de las siguientes no es una estrategia para alojar tu aplicación web o el trabajo de tu empresa?

Endpoint as a Service

CAMBIAR

9.

¿Cuál de las siguientes opciones de alquiler de un servidor suele ser la más económica?

Shared Hosting

CAMBIAR

10.

¿Cuál de los siguientes frameworks NO es un framework de Python para la creación del backend de aplicaciones web?

Symfony

CAMBIAR

11.

¿Cuál de las siguientes herramientas no es un framework de JavaScript para la creación del frontend de aplicaciones web?

React.JS

CAMBIAR

12.

¿Qué es una librería?

Código escrito por otros programadores que es aprovechable por otros proyectos.

CAMBIAR

13.

¿A cuáles de las siguientes estructuras de datos es equivalente un archivo JSON?

Un diccionario de Python.

CAMBIAR

14.

El proceso de llevar una aplicación desde el entorno local a producción se conoce como:

Deploy

CAMBIAR

15.

La nube no es más que:

Un conjunto de servidores interconectados que conforman lo que conocemos como Internet.