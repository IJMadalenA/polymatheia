# TCP/IP

__TCP/IP__ (_Transmission Control Protocol / Internet Protocol_), Es un protocolo de enlace de datos que se usa en Internet para que los ordenadores y otros dispositivos envíen y reciban datos, posibilitando que los dispositivos conectados a Internet se comuniquen entre sí entre varias redes.

__TCP/IP__ determina cómo los ordenadores transfieren datos de un dispositivo a otro. Estos datos deben ser exavctos para que el receptor obtenga la misma información enviada por el emisor. 

Para garantizar que cada comunicación llegue intacta al destino, el modelo __TCP/IP__ divide los datos en paquetes y luego los vuelve a juntar para formar el mensaje completo en el destino. Enviar los datos en paquetes pequeños hace que sea más fácil mantener la exactitud que enviando todos los datos a la vez.

Después de dividir un mensaje individual en paquetes, estos pueden recorrer diversos caminos en caso de congestión. Es como enviar distintas tarjetas de cumpleaños a la misma casa por correo.

---

## Funcionamiento del TCP/IP.

Cuando se envía algo por Internet, el modelo __TCP/IP__ divide esos datos en paquetes según un procedimiento de cuatro capas. Los datos primero atraviesan esas capas en un sentido, y luego lo hacen en sentido contrario cuando los datos se vuelven a juntar en el destino.

El modelo __TCP/IP__ funciona gracias a que todo el proceso está estandarizado. Sin la estandarización, la comunicación podría volverse impredecible y ralentizar las operaciones, y un Internet rápido depende de la eficiencia. 

## Otros protocolos de transferencia.

El modelo __TCP/IP__ abarca muchos protocolos de Internet que definen cómo se tratan y se envían los datos. Los protocolos de Internet más habituales son: __HTTP__, __FTP__, __SMTP__ y __MQTT__, los cuales se usan a menudo en cominación con el __TCP/IP__.

---

## Diferencia entre TCP e IP.

__TCP__ e [__IP__](./Dirección_IP.md) son protocolos distintos para redes informáticas. La diferencia entre __TCP__ (_protocolo de control de transmisión_) e [__IP__](./Dirección_IP.md) (_Internet Protocol_) es su papel en el proceso de transmisión de datos. 

[__IP__](./Dirección_IP.md) obtiene la dirección a la que se envían los datos (la dirección del ordenador). __TCP__ garantiza la entrega correcta de los datos una vez hallada dicha dirección [__IP__](./Dirección_IP.md). 

[__IP__](./Dirección_IP.md) clasifica la tarjeta postal y __TCP__ la envía y reciba. Aunque los dos protocolos selen considerarse una entidad, otros protocolos, como __UDP__ (_User Datagram Protocol_), pueden enviar datos en el sistema [__IP__](./Dirección_IP.md) sin usar __TCP__. Aún así, __TCP__ requiere una dirección [__IP__](./Dirección_IP.md) para enviar datos. Esa es otra diferencia entre [__IP__](./Dirección_IP.md) y __TCP__.

---

## Capas del modelo TCP/IP.

Hay __cuatro capas__ en el modelo __TCP/IP__: acceso a la red, Internet, transporte y aplicación. Estas capas son un conjunto de protocolos. El modelo __TCP/IP__ pasa los datos por estas capas en un orden concreto cuando un usuario envía información y después en el orden inverso cuando se reciben los datos.

### Capa 1: Acceso a Internet.

La capa de acceso a la red, también conocida como la capa de enlace a los datos, __gestiona la infraestructura física__ que permite a los ordenadores comunicarse entre sí por Internet. Esto abarca, entre otros elementos, cables Ethernet, redes inalámbricas de interfaz de red y controladores de dispositivos en el ordenador. 

La capa de acceso a la red también incluye la infraestructura técnica, como el código que convierte datos digitales en señales transmisibles, que hacen posible una conexión. 

### Capa 2: Internet.

También llamada la capa de red, __controla el flujo y el enrutamiento de tráfico__ para garantizar que los datos se envían de forma rápida y correcta. Esta capa también es responsable de volver a juntar el paquete de datos en el destino. Si hay mucho tráfico en Internet, esta capa puede tardar un poco más en enviar un archivo, pero es menor probable que el archivo se dañe.

### Capa 3: Transporte.

Es la que __proporciona una conexión de datos fiable__ entre dos dispositivos de comunicación. Es como enviar un paquete asegurado: la capa de transporte divide los datos en paquetes, confirma los paquetes que ha recibido del remitente y se asegura de que el destinatario confirme los paquetes recibidos por su parte.

Se establecen canales de datos básicos utilizadas para hacer 

### Capa 4: Aplicación.

Es el grupo de aplicaciones que __permite al usuario acceder a la red__. Para la mayoría de nosotros, esto significa el correo electrónico, las aplicaciones de mensajería y los programas de almacenamiento en la nube. Esto es lo que el usuario final ve y con lo que interactúa al recibir y enviar datos.

---

