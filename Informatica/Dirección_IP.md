## Dirección IP.

Una dirección __IP__ (_dirección de protocolo de Internet_) es una serie de números asignados a cada dispositivo conectado a una red informática o a Internet. Las direcciones __IP__ identifican y diferencian los miles de millones de dispositivos en linea, incluidos los ordenadores y los teléfonos móviles, y ayudan a esos dispositivos a comunicarse entre sí.

Otros dispositivos conectados a Internet, incluidas las impresoras y un número cada vez mayor de dispositivos del Internet de las cosas (IoT) como altavoces inteligentes, frigoríficos, sistemas de vigilancia doméstica, etc., también tienen dirección __IP__.

Con las direcciones __IP__ se garantiza que los datos transmitidos se dirigen hacia la ubicación adecuada. Los dispositivos conectados a Internet requieren una dirección digital para recibir y enviar datos.

---

## Análisis de las direcciones IP.

Las direcciones __IP__ suelen consistir en cuatro numero del 0 al 255, separados por puntos. Dentro de cada dirección __IP__, puede ver el __ID de red__, asignado a su red por su __ISP__, y el __ID de host__, el identificador único asignado a cada dispositivo conectado a esa red específica.

Ejemplo:

`172.16.254.1`

No hace falta que cada uno de los cuatro números de una dirección __IP__ sea un número de tres dígitos completo. En el ejemplo anterior, el primer número es el 172, el segundo es el 16, el tercero es el 254 y el cuarto es un 1. Conjuntamente, este formato de decimales con puntos se denomina un número de 32 bits.

Otro ejemplo de dirección __IP__:

`2001:db8:0:1235:0:567:9:1`

Este segundo ejemplo es una dirección IPV6, que es más compleja.

## ID de red y ID de host.

El __ID de red__ es la parte de una dirección __IP__ con la que se identifica la red que se está utilizando para conectarse a Internet (como el primer ejemplo de este MarkDown). El __ID__ de red lo asigna un proveedor de servicio de Internet __ISP__ (_Internet Services Provider_) en el caso de conexiones domésticas, por una red de empresa, o por una red pública.

Una red puede ser tan pequeña como de dos ordenadores conectados entre sí o tan grande como todo el Internet, que es una red de redes.

La parte del __ID de host__ de una dirección __IP__ indica el dispositivo concreto que está usando para conectarse a su red (es el «1» al final en el primer ejemplo).

Por ejemplo, en casa tenemos una serie de dispositivos y todos ellos requieren una dirección __IP__ para conectarse a Internet. La configuración de estas direcciones __IP__ para conectarse a Internet. La configuración de estas direcciones __IP__ podrían parecerse al siguiente ejemplo:

```sh
Nombre del dispositivo: ID_de_red.ID_de_host
Portatil_1: 172.16.254.1
Portatil_2: 172.16.254.2
Super_PC: 172.16.254.3
Smartphone: 172.16.254.4
```

Para cada _host_ de una red, la parte de red de la dirección__IP__ es la misma, mientras que el último número es distinto para identificar cada _host_. Un _host_ tiene únicamente una dirección __IP__, mientras que una red tiene muchas.

---

Una dirección __IP__ puede revelar información confidencial, como la ubicación física y otros detalles privados, y ayudar a las empresas a rastrear comportamiento en línea. No puede conectarse en línea sin una dirección __IP__, pero la puede cambiar y ocultar mediante una red privada virtual como un __VPN__.

Una __VPN__ encripta los datos y redigige su tráfico en línea hacia un servidor __VPN__ dedicado antes de que se conecte al área pública de Internet. Al conectarse a un sitio web, el usuario se presenta como si proviniera de la __VPN__, de manera que su dirección __IP__ auténtica se enmascara y el sitio web solo tiene acceso a la dirección __IP__ de la __VPN__.

---

## Direcciones IP estáticas y dinámicas.

Una dirección __IP__ estática (tambien llamada dirección __IP__ dedicada) es fija y no cambia automáticamente. Las direcciones __IP__ estáticas se suelen usar para dispositivos de empresas, porque al tener una dirección __IP__ dedicada mantiene las conexiones de red ininterrumpidas.

Una dirección __IP__ dinámica (también llamada dirección __IP__ compartida) cambia automáticamente en función de las __IP__ disponibles. Las direcciones __IP__ dinámicas se suelen usar para los dispositivos conectados a una red doméstica y no requieren ninguna entrada o configuración manual. Las direcciones __IP__ dinámicas se asignan automáticamente y continuamente por su __ISP__.

La forma en que se asigna una dirección IP a su dispositivo depende de la red, del __ISP__ y de las características del dispositivo.

Una dirección __IP__ se crea automáticamente si es dinámica, y manualmente si es estática. Una dirección estática es fija o permanente, mientras que una dinámica puede cambiar cada vez que se conecte a Internet. Es posible que se asigne una dirección __IP__ dinámica cada vez que se reinicie el ordenador.

---

## Direcciones IP públicas y privadas.

Los dispositivos tienen dos direcciones __IP__ distintas, una pública y otra privada. 

Una dirección __IP__ pública, también llamada dirección __IP__ externa o global, se utiliza para comunicarse entre _host_ (dispositivos) y el área global de Internet. El __ISP__ suele proporcionar para un uso doméstico direcciones __IP__ públicas, que son las que le conectan a Internet.

Una dirección __IP__ privada, llamada a menudo dirección __IP__ local o interna, se asigna a su dispositivo desde una red privada. Las direcciones __IP__ privadas no se dirigen a Internet y están previstas para funcionar únicamente dentro de una red local.

En una red típica, el router utiliza una dirección __IP__ pública para identificar frente al resto de Internet y así garantizar la conexión, y dentro de esa red, es probable que haya varios dispositivos diferentes. El router asigna a cada uno de los dispositivos conectados a él, una dirección __IP__ privada, para así poder enviar datos al dispositivo concreto que los solicita. Los dispositivos en la misma red utilizan direcciones __IP__ privadas para comunicarse directamente. 

Una dirección __IP__ pública es la dirección __IP__ de puertas afuera que asigna a su router su proveedor de servicios de Internet (__ISP__). El router utiliza esta __IP__ pública para acceder a Internet. Otros ordenadores en Internet utilizan su dirección __IP__ pública para comunicarse con los dispositivos de su red.

En una red típica el router sirve como intermediario entre el ordenador e Internet, encargandose de todas las conexiones en nombre de los dispositivos de la red.

---

Los routers asignan una dirección __IP__ privada a los dispositivos que se conectan a ellos. Una dirección __IP__ privada permite al _router_ dirigir correctamente el tráfico de Internet dentro de la red, además de permitir a los dispositivos dentro de una red de comunicarse entre ellos. 

Cuando se utiliza Internet y se envían y reciben datos a través de una dirección __IP__ pública y, a continuación, el _router_ pasa ese tráfico a su dispositivo empleando la dirección __IP__ privada. Este proceso de intercambio entre las direcciones __IP__ pública y privada se denomina __Traducción de Direcciones de Red (NAT)__.

### Intervalos de direcciones __IP__ públicas.

Todas las direcciones __IP__ públicas caen dentro de uno de los siguientes intervalos predefinidos de direcciones:

- 1.0.0.0 - 9.255.255.255
- 11.0.0.0 - 126.255.255.255
- 129.0.0.0 - 169.253.255.255
- 169.255.0.0 - 172.15.255.255
- 172.32.0.0 - 191.0.1.255
- 192.0.3.0 - 192.88.98.255
- 192.88.100.0 - 192.167.255.255
- 192.169.0.0 - 198.17.255.255
- 198.20.0.0 - 223.255.255.255

Todas las direcciones __IP__ con el formato 10.x.x.x quedan excluidas de esta lista, por lo que pude inferir que cualquier dirección __IP__ que comience por 10 es privada.

#### Intervalos de direcciones IP privadas.

Las direcciones IP privadas solo necesitan ser exclusivas dentro de la propia red local.

Los intervalos de direcciones IP privadas son los siguientes:

- Intervalo de direcciones IP privadas de clase A: 10.0.0.0 – 10.255.255.255 
- Intervalo de direcciones IP privadas de clase B: 172.16.0.0 – 172.31.255.255
- Intervalo de direcciones IP privadas de clase C: 192.168.0.0 – 192.168.255.25

Cada dispositivo en una misma red debe tener una dirección __IP__ privada exclusiva. No obstante, como hay disponibles tantas direcciones __IP__ privadas, una res privada puede acomodar una gigantesca cantidad de dispositivos dentro.

---

## IPv4 e IPv6.

### IPv4.

Creado en 1978, el protocolo IPv4 estandariza la forma en que los ordenadores se comunican entre sí en Internet. Es un protocolo sin conexión, lo cual significa que los datos se pueden enviar sin que las partes inviertan tiempo en establecer una conexión directa, y solo requiere pequeñas cantidades de memoria.

IPv4 ofrece más de 4 mil millones de direcciones únicas, lo que parecía suficiente en su momento, pero en 40 años ya ha llegado a su limite. 

### IPv6.

Es un estándar actualizado para identificar ordenadores en Internet. Al igual que IPv4, proporciona un identificador único a cada dispositovo.

IPv6 aumenta el número de direcciones __IP__ posibles desde los 4 mil millones de IPv4 a los 340 billones de billones de billones. IPv6 se escribe como una cadena hexadecimal de dígitos de 128 bits, y una dirección IPv6 típica es parecida a esto:

`2001:0ab8:85a2:0000:0000:8a3a:0370:7334`

IPv6 agiliza las transferencias de datos al hacer que dos direcciones sean directamente accesibles entre sí nuevamente. A diferencia de la IPv4 que introdujo pasos adicionales para compensar la relativa falta de direcciones únicas.

Ya no será necesario verificar cada paquete de datos recibidos para asegurarse de que sea idéntico a lo que se envió, por ejemplo, como es necesario en un protocolo sin conexión. IPv4 utiliza un proceso llamado *suma de verificación* para comprobar la integridad de los datos que se envían. La suma de verificación suele llevarse a cabo varias veces, ya que un router dirige el tráfico a varios ordenadores de una dirección. Cuando cada dispositivo pueda tener su propia dirección permanente, configurarlas será mucho más sencillo.

IPv6 se ha desarrollado para que los datos se muevan de forma más eficiente. El soporte para la Calidad de servicio (QoS) supone una asignación de recursos más eficiente. Cuando su velocidad de Internet es lenta o limitada, la QoS prioriza qué bits de datos deben ir primero.

### Diferencias entre IPv4 e IPv6.

#### Velocidad.

Si bien el encabezado de IPv6 es más grande y significa que hay más datos que transferir, la estructura optimizada en realidad permite envíos más rápidos. Con IPv4, la mayoría de datos que recibe pasan por una dirección __IP__ compartida por muchos otros antes de que se le reenvíen. La comunicación IPv6 tarda menos tiempo porque un dispositivo envía datos directamente a otro.

Las conexiones directas se aseguran de que todos los mensajes se reciben intactos. 

IPv4 busca errores en varios puntos durante la comunicación, lo que prolonga el tiempo de transferencia. Por su parte, IPv6 comprueba la transmisión de datos precisa a nivel de __TCP__. 

#### Seguridad.

A pesar de que el IPv6, al poseer una cantidad abismal de diferentes números de identificación, un _hacker_ de igual manera podría conseguir una dirección IPv6, con mayor esfuerzo, pero sigue sin ser imposible.

---

## Amenazas de seguridad.

Con una __VPN__ puede ocultar su dirección __IP__ para evitar los riesgos que conlleva su exposición. Sin una __VPN__ que oculte su verdadera dirección __IP__, podría ser vulnerable a una serie de amenazas de seguridad. 

### Acceso al dispositivo.

Si un hacker puede acceder al tráfico __IP__, sus datos personales enviados en ese momento podrían quedar expuestos. 

### Descargar contenido ilegal.

Un riesgo creciente de las direcciones __IP__ desprotegidas es la replicación. Un _hacker_ puede copiar su dirección __IP__ y usarla para acceder o descargar contenido ilegar, que posteriormente se podría rastrear hasta el ordenador victima.

### Rastrear la ubicación.

Un _hacker_ puede determinar su ubicación mediante una combinación de direcciones __IP__, __GPS__, redes Wi-Fi y otros sistemas.

### Acoso.

Un individuo sospechoso puede llevar el rastreo de la ubicación más allá y encontrar la dirección real de su casa basándose en su dirección __IP__ expuesta. 

### Ataque a la red.

Se podría usar la dirección __IP__ para lanzar un ataque DDoS dirigidos contra la red, generando cantidades masivas de tráfico falso con el objetivo de colapsar un sitio específico. 