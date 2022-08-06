# 6 - Ataques remotos y locales

​	En la seguridad informática existen ataques, estos ataques se dividen en dos Ataques Remotos y Ataques locales.

## Clasificación de los ataques.

### Ataques Lógicos:

​	Este tipo de seguridad está basada en cubrir las amenazas que se muestran sobre la información y el software.

### Trashing (Cartoneo):

​	Un usuario escribe su login y password en un papelito y luego, cuando se acuerda, lo tira a la basura. El _trashing_ suele ser físico o lógico, como revisar buffers de impresora y memoria, bloques de discos, bloc de notas, etc.

### Monitorización:

​	Este tipo de ataque se hace para ver a la víctima y su sistema, con la finalidad de marcar sus vulnerabilidades y posibles métodos de acceso futuros. Se pueden presentar como:

- __Shoulder Surfing:__ Se basa en espiar físicamente a los usuarios para lograr el login y su password correspondiente. El Surfing exprime el error de los usuarios de dejar su login y password anotadas de forma próxima de la computadora (generalmente en post–it adheridos al monitor o teclado). Algún intruso puede continuar por ahí, verlos y memorizarlos para su posterior utilización. Otra técnica unida al surfing es aquella a través de la cual se ve, por encima del hombro, al usuario cuando inserta su nombre y password.
- __Decoy (Señuelos):__ Los Decoy son programas fabricados con la misma interface que otro original. En ellos se simula la solicitud de un logeo y el usuario desprevenido lo realiza. Luego, el programa almacenará esta información y dará paso a las actividades normales del sistema. La información guardada será usada por el atacante para futuras "visitas". Una técnica similar es aquella que, a través de un programa se almacenan todas las teclas presionadas durante una sesión. Después solo hará falta estudiar el fichero generado para conocer nombres de usuarios y claves.

### Spoofing-Looping:

​	Es "hacerse pasar por otro" y el objetivo de esta técnica, justamente, es trabajar en nombre de otros usuarios, normalmente para hacer tareas de Snooping. Una manera común de Spoofing es lograr el nombre y password de un usuario legítimo para, una vez entrado al sistema, tomar acciones en su nombre. El intruso usualmente usa un sistema para obtener información e ingresar en otro, y luego hace uso de este para entrar en otro, y así sucesivamente. Este proceso al que podemos llamar como Looping, tiene la finalidad de "evaporar" la identificación y la localización del atacante. El camino elegido desde el origen hasta el destino puede tener muchas paradas, que exceden obviamente los límites de un país. 

### Ataques pasivos:

​	Cuando se producen ataques pasivos el intruso o atacante no altera en modo alguno la comunicación, sino que solamente se dedica a escuchar o monitorizar con el objetivo de obtener toda la información posible de lo que se está transmitiendo.

​	Sus objetivos principales on interceptar datos y analizar el tráfico, una técnica más sutil para obtener información sobre la comunicación, que puede tratar de:

- Conseguir el origen y destinatario de la comunicación a través de la lectura de las cabeceras de los paquetes monitorizados.
- Control del volumen de tráfico de intercambio entre las instituciones monitorizadas.
- Control de las horas habituales de intercambio de datos entre las distintas instituciones.

Este tipo de ataques son muy dificiles de detectar, ya que no provocan alteración alguna de los datos.

### Ataques activos:

​	Este tipo de ataques implican cambios en el flujo de datos y se dividen en los siguiente:

- __Suplantación de identidad:__ El atacante se hace pasar por una entidad diferente.
- __Reactuación:__ Uno o varios mensajes son repetidos para producir un efecto no deseado.
- __Modificación de mensajes:__ Una parte del mensaje real es alterada para producir efectos no autorizados.
- __Degradación fraudulenta del servicio:__ Impide el uso normal de los recursos informáticos y las comunicaciones.

#### Tipos de ataques más usuales:

- __Sniffing:__ escucha los datos que atraviesan la red.
- __Hijacking:__ Permite a personal no autorizado robar conexión de un usuario.
- __Explotar bugs del software:__ un intruso aprovecha fallos en el software para hacerse con el control del sistema.
- __Negación de servicio:__ se bloquean un determinado número de servicios para que los empleados no los puedan usar con normalidad.
- __Ingeniería social:__ un intruso convence a un empleado de que le transmita información.
- __Phising:__ A través de mensajes falsos se engaña a los usuarios para que faciliten información.
- __Confianza transitiva:__ se utilizan las relaciones UNIX o host para tener privilegios.
- __Ataques dirigidos por datos:__ virus, gusanos, etc.
- __Troyanos:__ el atacante puede hacerse con el control del sistema a través de un software instalado en el ordenador.
- __Mensajes de control de red o enrutamiento fuente:__ se envían paquetes ICMP para hacer pasar paquetes por un router comprometido.
- __Reenvío de paquetes:__ reenvío de paquetes para duplicar un mensaje.
- __Adivinación de password:__ ataques a través de diccionarios.
- __Tempest:__ barrido de emisiones de electrones de los CRT
- __Rubber-hosse:__ obtener información a través de soborno.

---



## 5.2 - ¿Qué hacer si recibimos un ataque?

La principal recomendación para evitar este tipo de ataques, es el sentido común, ya que la mayoría de ellos se basan en la ingenuidad y curiosidad de la víctima. Es por esta razón, que tenemos que intentar evitar:

- Abrir archivos adjuntos de correos electrónicos que no conocemos.
- Evitar abrir documentos web muy publicitados en Internet.
- No abrir videos sensacionalistas muy publicitados o enviados a través de e-mail o redes sociales.
- Tratar en lo posible de no realizar enlaces recortados, publicados en redes sociales.
- Evitar la instalación software pirata.
- No instalar programas descargados de Internet, si no se conoce el origen del software.

Además de estas recomendaciones, es de vital importancia mantener todas nuestras aplicaciones actualizadas, para así evitar errores que pudiesen ser utilizados por un atacante remoto. También, es recomendable tener instalado en nuestro equipo un buen antivirus, un antimalware y cortafuegos para minimizar el riesgo de conexiones no deseadas, y bloquear el acceso de éstas a nuestros equipos.

Lo primero que debes hacer si detectas que eres víctima de un ataque remoto es desconectarte de internet y luego ya empezar a analizar el sistema completo.