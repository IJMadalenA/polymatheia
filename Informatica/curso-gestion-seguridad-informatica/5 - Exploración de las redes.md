# 5 - Exploración de las redes.

## 5.1 - Exploración de la red.

​	Las redes inalámbricas denominadas como WLAN recurren a medidas de seguridad muy básicas para poder evitar su utilización por parte de personal no autorizado.

​	Los identificadores SSID (_Service Set Identifier_) son un instrumento elemental para la seguridad, y se refieren a todos los equipos o puntos de acceso que incluyen una red inalámbrica.

> ​	Los SSID son secuencias de un máximo de 32 caracteres, que la mayoría de las veces son alfanumericos, y que debe ser compartido por 2 dispositivos inalámbricos para que estos puedan comunicarse entre sí.

​	Uno de los metodos más básicos para proteger una red inalámbrica es desactivar la difusión (_broadcast_) del SSID, ya que para el usuario medio no aparecerá como una red en uso. Sin embargo, no debería ser el único método de defensa para proteger una red inalámbrica.

​	Aun con la difusión del SSID desactivada, un intruso puede usar un _Sniffer_ de radio para detectar dicha transmisión por parte de cualquier usuario de red inalámbrica.

​	En lo que respecta a la autenticación de los equipos cliente se han determinado dos opciones de esquemas en los protocolos más básicos de las redes inalámbricas: **"Open Systems Authentication"** o bien **"Shared Key Authentication"**.

​	Además, también se ha recurrido a una autenticación optativa de terminales a partir de determinadas direcciones como por ejemplo MAC (Media Access Control), que es capaz de identificar cada una de las tarjetas de red de estos dispositivos.

​	La __dirección MAC__ puede ser falseada por algún intruso a través de técnicas __spoofing__ o lo que es lo mismo, suplantación de identidad. Esto se puede realizar cambiando la dirección de su propia tarjeta inalámbrica, por lo que la autenticación que se realiza a partir de direcciones MAC es una metodología poco fiable que conlleva una gran carga de trabajo manual.

​	En lo que se refiere a la confidencialidad de los datos que son transmitidos por los equipos que están conectados a la red, hay que tener presente que una red inalámbrica transmite y recibe toda la información vía radio por lo que es fácil que cualquier intruso pueda estar al tanto de este tráfico con un equipo de radiofrecuencia.

​	Debido a esto, es conveniente aplicar algoritmos de encriptación tales como los que son previstos en el estándar WEP (_Wired Equivalent Privacy_). 

> ​	El sistema de cifrado WEP es un sistema incluido en el estándar IEEE 802.11 como protocolo para redes _Wireless_ que permite cifrar la información que se transmite. Proporciona un cifrado a nivel 2, basado en el algoritmo de cifrado RC4 que utiliza claves de 64 bits o de 128 bits

---



## 5.2 - Herramientas de análisis de red.

### Nmap (_Network Mapper_):

​	Es una utilidad de software libre para explorar, administrar y auditar la seguridad de redes de ordenador. Detecta hosts online, sus puertos abiertos, servicios y aplicaciones corriendo en ellos, su sistema operativo, que firewalls corren en una red y de qué tipo son.

​	Es una herramienta de escaneo de puertos de un servidor de hosting o de reconocimiento de una red, que es utilizada para localizar los servicios abiertos, los servicios filtrados y los puertos cerrados de un cierto servidor, el sistema operativo de un host y las versiones de los servidores que operan en el host en los diferentes puertos TCP o UDP.

	### NetCat:

​	Es una herramienta de red bajo licencia GPL (en la versión de GNU) que permite a través de intérprete de comandos y con una sintaxis muy sencilla para abrir puertos TCP/UDP en un HOST, asociar una shell a un puerto en concreto (para conectarse por ejemplo a MS-DOS o al intérprete bash de linux remotamente) y forzar conexiones UDP/TCP (útil para realizar rastreos de puertos o realizar transferencias de archivos bit a bit entre dos equipos.)

​	Sus capacidades hacen que sea a menudo usada como una herramienta para abrir puertas traseras una vez invadido un sistema y obtenido privilegios de administrador o root del equipo. También resulta extremadamente útil a efectos de depuración para aplicaciones de red.

### NBTScan:

​	Es un explorador del nameserver de NETBIOS. Se trata de una herramienta que a través de línea de comandos permite hacer un escaneo de todos los nombres de servidores NETBIOS en una red local TCP/IP o remota, en busca de recursos compartidos.

​	Es una herramienta que permite realizar escaneos al puerto 137/UDP hasta buscar servidores de nombres NETBIOS, mostrándonos aquellos equipos de nuestra red que podrían estar compartiendo recursos.

​	Su funcionamiento es sencillo, básicamente se envían peticiones de estados de NetBios a una dirección o rango de estas, y por cada respuesta de un servidor obtenemos información sobre su dirección, nombre NetBios, dirección MAC y nombre del usuario con sesión iniciada. 



## Reconocimiento y enumeración.

### The Dude:

​	Es una herramienta gratuita que nos permite realizar de forma rápida un mapa de la red local y nos muestra información de todos sus componentes. Permite trabajar con diversos protocolos, como TCP o DNS, entre otros. Además ofrece otras utilidades, como la comprobación de puertos o realización de acciones como ping o traceroute.

### LANSurveyor:

​	Es una herramienta desarrollada por SolarWinds. Este software explora la red y nos va creando el mapa local. Nos entrega informes de las condiciones de la red, de los switch, VLANs, subredes, los elementos que conforman la red, etc. Esta herramienta es software propietario (se debe pagar licencia de uso), aunque tiene una versión de prueba que ofrece durante un tiempo limitado.

### WirelessMon 4.0:

 	Esta herramienta nos permite gestionar la conexión inalámbrica. En distintos submenús nos ofrece gran variedad de opciones, como comprobar que la configuración de red 802.11 es correcta, realizar análisis de las posibles interferencias que puedan estar afectando a nuestra señal, pruebas de WiFi y cobertura de red o comprobar la configuración de seguridad de la red. Es un software privado y de pago, aunque existe una versión de prueba durante un periodo de 30 días.

### Inssider: 

​	Es una herramienta de pago que nos permite, además de ver las redes que nos rodean y los puntos de acceso, analizar el entorno de nuestra red, mostrándonos interferencias y medidas de ruido. Además en su versión completa, incluye análisis de interferencias de otro tipo de redes, como cámaras de seguridad u otro tipo de señales. Todo ello nos ayudará a escoger el canal por el que enviar nuestra señal para se vea poco perjudicada.