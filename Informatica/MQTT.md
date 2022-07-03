# MQTT

___Message Queuing Telemetry Transport___.

Es un protocolo demensajería ligero para usar en casos de clientes que necesitan una huella de código pequeña, que están conectados a redes no fiables o con recursos limitados en cuento al ancho de banda. Se utiliza principalmente para comunicaciones M2M (_machine to machine_) o conexiones del tipo IoT (_internet of things_).

Está basado en la pila [__TCP/IP__](./TCPIP.md) como base para la comunicación. Este protocolo mantiene abierta cada conexión y se "reutiliza" en cada comunicación. Es una diferencia, por ejemplo, a una petición HTTP 1.0 donde cada transmisión se realiza a través de conexión.

## Origen.

Fue creado por el Dr. Andy Stangord-Clark y Arlen Nipper en 1999 para poder solventar las necesidades de comunicación en la industria del petróleo y el gas, para que estas pudieran enviar los datos obtenidos desde los dispositivos de monitoreo en las instalaciones y bases de extracción hacia un servidor remoto.

Podemos imaginar una plataforma petrolera en medio del atlántico para la cual establecer una conexión por cable o radio es directamente imposible y la única alternativa disponible para enviar información es por vía satelital, la cual es muy costosa y se factura en función de la cantidad de datos utilizada, entonces, con miles de sensores en el campo, la industria necesitaba una forma de comunicación que pudiera proporcionar datos de manera suficientemente fiable para su uso, mientras se emplea un ancho de banda mínimo.



## Arquitectura.

### Arquitectura de MQTT.

MQTT se ejecuta sobre [__TCP/IP__](./TCPIP.md) utilizando una topología PUSH/SUBSCRIBE. En la arquitectura MQTT, existen dos tipos de sistemas: clientes y brókeres. Un bróker es el servidor con el que se comunican los clientes: recibe comunicaciones de unos y se las envía a otros. Los clientes no se comunican directamente entre sí, sino que se conectan con el bróker. Cada cliente puede ser un editor, un suscriptor o ambos.

MQTT es un protocolo controlado por eventos, donde no hay transmisión de datos periódica o continua. Así se mantiene el volumen de transmisión al mínimo. Un cliente sólo publica cuando hay información para enviar, y un bróker sólo envía información a los suscriptores cuando llegan nuevos datos.

![mqtt architecture](https://hlassets.paessler.com/common/files/infographics/mqtt-architecture.png)

### Arquitectura del mensaje.

Otra forma en que MQTT minimiza sus transmisiones es con un tamaño de mensaje pequeño y bien definido. Cada mensaje tiene un encabezado fijo de apenas 2 a 5 bytes. Se puede utilizar un encabezado opcional, pero eso incrementa el tamaño del mensaje. La carga útil del mensaje está limitada a únicamente 256 MB. Tres niveles diferentes de calidad de servicio (QoS) permiten a los diseñadores de redes elegir entre minimizar la transmisión de datos y maximizar la fiabilidad.



- **QoS 0**: ofrece la cantidad mínima de transmisión de datos. Con este nivel, cada mensaje se entrega a un suscriptor una vez, sin confirmación, por lo que no hay forma de saber si los suscriptores recibieron el mensaje. Este método a veces se denomina “lanzar y olvidar” o “una entrega como máximo”. Debido a que este nivel asume que la entrega está completa, los mensajes no se almacenan para entregarlos a los clientes desconectados que luego se vuelven a conectar.
- **QoS 1**: el bróker intenta entregar el mensaje y, luego, espera una respuesta de confirmación del suscriptor. Si no se recibe una confirmación dentro de un período de tiempo especificado, el mensaje se envía de nuevo. Usando este método, el suscriptor puede recibir el mensaje más de una vez si el bróker no recibe el acuse de recibo del suscriptor a tiempo. Esto se suele denominar “entregado al menos una vez”.
- **QoS 2**: el cliente y el bróker utilizan un protocolo de enlace de cuatro pasos para garantizar no sólo que el mensaje se reciba, sino que lo haga una única vez. También se conoce como “entrega exactamente una vez”.

QoS 0 puede ser la mejor opción para situaciones donde las comunicaciones son fiables pero limitadas. En aquellos casos en que las comunicaciones no sean fiables, pero donde las conexiones tampoco gozan de recursos limitados, QoS 2 sería la mejor opción. QoS 1 proporciona una solución a caballo entre ambos mundos, pero requiere que la aplicación que recibe los datos sepa cómo gestionar los duplicados.

Tanto en QoS 1 como en QoS 2, los mensajes se guardan o se ponen en cola para los clientes que están desconectados y que tienen una sesión persistente establecida. Estos mensajes se reenvían (de acuerdo con el nivel de QoS apropiado) una vez que el cliente vuelve a conectarse.

---

![img](https://www.luisllamas.es/wp-content/uploads/2019/04/mqtt-message.png)

- **Cabecera fija**. Ocupa 2 a 5 bytes, obligatorio. Consta de un código de control, que identifica el tipo de mensaje enviado, y de la longitud del mensaje. La longitud se codifica en 1 a 4 bytes, de los cuales se emplean los 7 primeros bits, y el último es un bit de continuidad.
- **Cabecera variable**. Opcional, contiene información adicional que es necesaria en ciertos mensajes o situaciones.
- **Contenido(payload)**. Es el contenido real del mensaje. Puede tener un máximo de 256 Mb aunque en implementaciones reales el máximo es de 2 a 4 kB.

---



## Ultima voluntad y testamento.

Cuando las comunicaciones no son fiables, es posible que un editor se desconecte de la red sin previo aviso. En tales casos, un editor puede registrar un mensaje para enviarlo a los suscriptores por si se desconecta inesperadamente, en lo que se denomina *última voluntad y testamento*. Este mensaje se almacena en la caché del bróker y, normalmente, incluye información que permite identificar al editor desconectado para que se puedan tomar las medidas adecuadas.



## Mensajes en MQTT.

Para mantener el protocolo al mínimo, sólo se pueden efectuar cuatro acciones en cualquier comunicación: publicar, suscribirse, cancelar suscripción o hacer ping.

- **Publicar**: envía un bloque de datos que contiene el mensaje que se va a enviar. Estos datos son específicos de cada implementación, pero pueden ser algo tan simple como una indicación de encendido/apagado o un valor de un determinado sensor, como temperatura, presión, etc. En el caso de que el tema que se está publicando no exista, este se crea en el bróker.
- **Suscribirse**: convierte a un cliente en suscriptor de un tema. Se puede suscribir a temas en concreto o mediante comodines, que permiten suscripciones a toda una rama de temas o a parte de ella. Para suscribirse, un cliente envía un paquete SUBSCRIBE y recibe un paquete SUBACK a cambio. Si hay un mensaje retenido para el tema, el nuevo suscriptor también lo recibe.
- **PING**: un cliente puede hacer ping al bróker. El suscriptor envía un paquete PINGREQ y, como respuesta, se recibe un paquete PINGRESP. Se pueden utilizar pings para garantizar que la conexión siga funcionando y que la sesión TCP no haya sido cerrada inesperadamente por otro equipo de red, como un router o una puerta de enlace.
- **DESCONECTAR**: un suscriptor o editor puede enviar un mensaje de DISCONNECT al bróker. Este mensaje informa al bróker de que ya no necesitará enviar o poner en cola mensajes para un suscriptor y que ya no recibirá datos de un editor. Este tipo de cierre permite al cliente volver a conectarse utilizando la misma identidad de cliente que en ocasiones anteriores. Cuando un cliente se desconecta sin enviar un mensaje de desconexión, se envía su última voluntad y testamento a los suscriptores.



## Seguridad.

El objetivo original del protocolo MQTT era hacer posible la transmisión de datos de una forma más pequeña y eficiente a través de líneas de comunicación costosas y poco fiables. Como tal, la seguridad no fue una de las principales preocupaciones durante el diseño e implementación de MQTT.

Sin embargo, hay algunas opciones de seguridad disponibles a costa de una carga superior en la transmisión de datos y una mayor impronta.

 

- **Seguridad de red**: si la red en sí puede protegerse, la transmisión de datos inseguros en MQTT es irrelevante. En tal caso, los problemas de seguridad tendrían que producirse desde el interior de la propia red, quizás a través de un actor malicioso u otra forma de penetración en la red.
- **Nombre de usuario y contraseña**: MQTT permite nombres de usuario y contraseñas para que un cliente establezca una conexión con un bróker. Lamentablemente, para mantener la claridad, los nombres de usuario y las contraseñas se transmiten en texto sin cifrar. En 1999, esto era más que suficiente porque interceptar una comunicación por satélite para lo que era esencialmente una lectura de sensor sin importancia habría sido prohibitivamente difícil. Sin embargo, hoy en día, la interceptación de muchos tipos de comunicaciones de red inalámbrica se ha convertido en algo trivial, lo que hace que dicha autenticación sea casi inútil.
  Muchos casos de uso requieren un nombre de usuario y una contraseña ya no como protección contra actores maliciosos, sino como una forma de evitar conexiones involuntarias.
- **SSL/TLS**: al ejecutarse sobre TCP/IP, la solución obvia para proteger las transmisiones entre clientes y brókeres es la implementación de SSL/TLS. Lamentablemente, esto añade una sobrecarga sustancial a unas comunicaciones, por lo demás, livianas.



## Ventajas del MQTT.

Son varias las ventajas del protocolo __MQTT__ como sistema de comunicación M2M (_machine to machine_). Por un lado posee las ventajas del patrón _pub/sub_, como la escalabilidad, asincronismo y desacoplamiento entre clientes.

Además, __MQTT__ aporta una serie de características que le han hecho sobresalir sobre otros competidores. La principal sería su sencillez y ligereza, lo que lo hace adecuado para aplicaciones ___IoT___, donde frecuentemente se emplean dispositivos de escasa potencia.

Además, esta menor necesidad de recursos se traduce en un menor consumo de energía, lo cual es interesante en dispositivos que funcionan de forma perpetua o alimentados por baterías.

También al requerir de un ancho de banda mínimo es ideal para redes inalámbricas o conexiones con posibles problemas de calidad. También dispone de medidas adicionales importantes, como la seguridad y calidad del servicio ___QoS__. 



## MQTT v5.0.

El 3 de abril de 2019, OASIS publicó el estándar oficial 5.0 de MQTT

### Principales novedades de MQTT v5.0

- **Códigos de motivo**: originalmente, si se producía un error, MQTT simplemente no realizaba ninguna acción. El fallo en sí era el único código de error. En la versión 5.0, los reconocimientos admiten el uso de códigos de retorno que pueden proporcionar una razón clara y representable en forma de error. Por supuesto, el uso de códigos de retorno aumenta ligeramente la huella.
- **Suscripciones compartidas**: demasiados suscriptores a un tema específico en un bróker pueden crear problemas de carga. Las suscripciones compartidas permiten equilibrar la carga entre los clientes.
- **Caducidad del mensaje**: se pueden configurar los mensajes para que se eliminen si no se entregan dentro de un período establecido. Esto evita la entrega de mensajes antiguos y desactualizados a los suscriptores que estuvieron desconectados durante un cierto período de tiempo.
- **Alias de tema**: los nombres de los temas en sí pueden llegar a ser tan largos como para afectar al reducido tamaño del protocolo. Las cadenas de temas ahora se pueden reemplazar con un solo número cuando se usan repetidamente los mismos temas.

---



[¿Qué es MQTT? Definición y detalles (paessler.com)](https://www.paessler.com/es/it-explained/mqtt)

[¿Qué es MQTT? Su importancia como protocolo IoT (luisllamas.es)](https://www.luisllamas.es/que-es-mqtt-su-importancia-como-protocolo-iot/)



[OASIS Message Queuing Telemetry Transport (MQTT) TC | OASIS (oasis-open.org)](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=mqtt)

