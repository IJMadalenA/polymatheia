# 3 - Auditoria de seguridad de la información.

---

## 3.1 - Introducción a la auditoría de seguridad de la información.

​	Una auditoria de la seguridad de la información y sistemas de gestión de seguridad de la información describe los siguientes puntos:

- Los procedimientos instalados.
- Servidores, programas, sistemas operativos, equipos instalados, etc.
- Gestión de los sistemas instalados.
- Análisis de seguridad y eficiencia en cuenta a los equipos, red, sistemas y programas informáticos.
- Se verifica si se cumple con la normativa LOPD que se encuentre vigente en ese momento.

Existen diferentes tipos de auditorías, estas pueden ser de las siguientes clases: 

- Forense.
- Web.
- De código.
- Hacking ético.
- Análisis de vulnerabilidades.
- Físicas.
- De redes.

Para hacer una auditoría de seguridad, hay que seguir las siguientes directrices:

- Recuento de los servicios que sean objeto de la auditoría.

- Comprobación del cumplimiento de los estándares de normas de control y calidad.

- Identificas los sistemas operativos instalados, hardware, software.

- Análisis de aplicaciones instaladas y servicios.

- Evaluación y comprobación de las vulnerabilidades que se detecten.

- Rectificación con medidas concretas.

- Establecimiento de medidas precautorias.

  ---

## 3.2 - Ciclo del sistema de gestión de seguridad de la información.

​	Para determinar y gestionar un sistema de gestión de la seguridad de la información basado en ISO 27001, se hace uso del ciclo continuo PDCA, originario en los sistemas de gestión de la calidad.

Las cuatro etapas que forman el ciclo son:

1. Planificar (Plan): Se localizan las actividades susceptibles de mejora y se marcan los objetivos a lograr. Para buscar posibles mejoras se pueden hacer grupos de trabajo, escuchar las opiniones de los trabajadores.
2. Hacer (Do): Se hacen los cambios para incluir la mejora propuesta.
3. Controlar o Verificar (Check): Una vez incluida la mejora, se deja un periodo de prueba para corroborar su correcto funcionamiento. Si la mejora no pasa las expectativas iniciales habrá que cambiarla para ajustarla a los objetivos esperados.
4. Actual (Act): Finalmente, cuando acaba el periodo de prueba se deberá de repasar los resultados y compararlos con el funcionamiento de las actividades antes de haber sido implantada la mejora. Si los resultados son correctos se implantará de forma definitiva la mejora y si no lo son se tomara la decisión de realizar cambios para ajustar los resultados o si desecharla. Una vez acabado el paso 4, se debe volver al primer paso periódicamente para estudiar nuevas mejoras a implantar.

---



## 3.4 - Seguridad de la información.

​	La finalidad de la seguridad de la información es la de evitar su pérdida y cambios sin autorización. La protección tiene que asegurar la confidencialidad, integridad y disponibilidad de los datos.

---



## 3.5 - Seguridad humana, seguridad física y del entorno.

​	El objetivo es minimizar los riesgos de daños e interferencias a la información y a las operaciones de la organización.

---



## 3.6 - Gestión de comunicaciones y operaciones.

​	La monitorización de los servidores y los dispositivos de red es una de las medidas fundamentales que ha de estar prevista por las políticas de seguridad de la institución a modo de facilitar la detección de usos no autorizados así como posibles situaciones anómalas o intentos de ataque contra estos recursos llevados a cabo por la empresa.

​	Para poder poner en marcha la monitorización, es necesario activar y configurar en los equipos los registros de actividad (logs) para que sea más fácil acceder a la información e indicadores de los aspectos:

- Las sesiones que inician los usuarios en los servidores.
- Los procesos que se ejecutan en cada uno de los equipos informáticos.
- Las conexiones externas.
- El acceso y la utilización de los recursos del propio sistema.
- Intentos de violación de la política de seguridad.
- Detección de posibles ataques o de intentos de intrusión.

### 3.6.1 - Seguridad en las conexiones remotas.

​	Es conveniente tomar medidas de seguridad adicionales para la protección de las conexiones remotas, entre las que están:

- __Aislamiento de los equipos remotos:__ Limitando los permisos de acceso que se conceden para estos equipos y registrar toda actividad. 
- __Registrar las sesiones abiertas:__ Registrar el inicio y cierra de todas las sesiones que establezcan conexión e implementar temporizadores que detecten y cierren las sesiones inactivas.
- __Controlar los equipos remotos:__ Utilización de herramientas para poder controlar los equipos remotos y conectarse a los mismo con el objetivo de llevar a cabo tareas administrativas o incluso, proceder a su bloqueo.

Es fundamental que la política de seguridad defina cuál es el procedimiento a seguir para facilitar el acceso remoto a un usuario, teniendo en cuenta las siguientes consideraciones:

- Justificación de la conexión remota.
- Recursos que requiere la conexión.
- Mecanismos de autenticación y de control de acceso a estos recursos.
- Horario y días en que es permitida dicha conexión.
- Período de validez de la conexión.
- Usuario responsable que autoriza la conexión.

Únicamente un usuario autorizado podrá realizar operaciones de entrada o salida de datos sensibles a través de sistemas de transferencia de ficheros por medio de conexión remota.

---



## 3.7 - Control de accesos.

​	El manejar el acceso por medio de un sistema de restricciones y excepciones a la información es una base de todo sistema de seguridad informática. Para bloquear el acceso no autorizado a los sistemas de información se tendrían que implementar procedimientos formales para controlar la ejecución de derechos de acceso a los sistemas de información, bases de datos y servicios de información, y estos tienen que estar claramente documentados comunicados y controlados.

### 3.7.1 Gestión de usuarios.

​	La empresa ha de incluir en sus políticas de seguridad las directrices vinculadas al proceso tanto de solicitud como de creación, configuración, seguimiento o cancelación de cuentas de usuario. Así, también se ha de establecer una norma homogénea para la identificación de los usuarios de toda la institución.

### 3.7.2 Identificación y autenticación de usuarios.

​	La empresa debe tener siempre actualizada una lista de aquellos usuarios que tienen acceso autorizado a los datos del sistema de información, llevando siempre a cabo determinados procesos tanto para la identificación como para la autenticación de dicho acceso.

​	A la identificación y autenticación de usuarios se les conoce como el modelo de seguridad "AAA" (Authentication, Autorization and Accounting) que significa "Autenticación, Autorización y Contabilidad". Este modelo es utilizado para identificar a todos los usuarios y poder controlar su acceso al sistema informático.

​	Este paradigma esta basado en tres elementos que han de estar presentes en la política de seguridad:

- __Identificación y autenticación de los usuarios:__ La identificación permite que el usuario revelo su identidad como modo de acceder al sistema y la autenticación es el proceso por el que se valida dicha identificación.
- __Control de acceso al sistema informático:__ Esto se lleva a cabo a través de la autorización en función de los permisos de los usuarios.
- __Registro del uso de los recursos existentes por parte del usuario__. 



Elementos utilizados para identificar al usuario:

- __Lo que sabe:__ Contraseñas.
- __Lo que se posee:__ Móvil, llave USB, Tarjetas de crédito, etc.
- __Lo que es:__ Características biométricas del usuario.
- __Lo que se sabe hacer:__ Firma manuscrita.
- __Dónde se encuentra el usuario:__ Conexión con determinado equipo o en determinada ubicación GPS.



Requisitos que garanticen la seguridad de una contraseña:

- __Tamaño mínimo__ de caracteres que esta debe incluir.
- __Caducidad__.
- __Registro del historial de contraseñas__ para evitar que se utilicen contraseñas ya empleadas.
- __Control de la composición de la contraseña__.
- __Bloqueo de las cuentas luego de un numero máximo de intentos.__
- Ocultar el último nombre del usuario que ha usado determinado equipo.



### 3.7.3 Seguridad en el puesto de usuario.

Conceptualmente podríamos decir que __los virus informáticos se caracterizan por su capacidad de infectar a otros programas__, por lo general inyectando su propio código malicioso dentro del código original del programa huésped.

Tipos de troyanos:

- __Troyano downloader__: Al comprometer un ordenador se encarga de descargar otros códigos maliciosos.
- __Troyano bancarios:__ Utilizados para realizar fraudes a través de la obtención de datos confidenciales de los usuarios.
- __Troyano Clicker:__ Aquellos que realizan fraudes a través de clic en sitios con publicidad.
- __Troyano Backdoors:__ Permite el acceso a un sistema de una manera no convencional.
- __Troyanos Bot:__ Convierte los ordenadores en equipos zombie que luego forman parte de botnets.



### 3.7.4 Técnicas de recuperación y desinfección de datos afectados.

​	__<u>Análisis forense informático</u>__ es el conjunto de técnicas para conseguir información importante de discos duros, pero siempre sin alterar el estado de éstos. Esto posibilita la búsqueda de datos que son conocidos previamente con el objetivo de encontrar un determinado patrón o hallar información oculta, es decir, consiste en la recopilación de información del ataque, para a posteriori poner las medidas oportunas para que el ataque no se repita.

El análisis forense informático pasa por distintas etapas que determinan la metodología que se sigue en una investigación:

1. Identificación.
2. Preservación o adquisición.
3. Análisis.
4. Presentación de los resultados.

---



## 3.8 Gestión de continuidad del negocio.

​	El objetivo es mantener la seguridad de la información en el proceso de las fases de activación, de desarrollo de procesos, procedimientos y planes, para continuar el negocio y de vuelta a la normalidad luego de un ataque.

​	Se tendrían que analizar las consecuencias de los desastres, fallas de seguridad, pérdidas de servicio y la disponibilidad de la ayuda y desarrollar e implementar planes de contingencia para corroborar que los procesos del negocio se tienen que restaurar en los plazos requeridos las operaciones esenciales, aguantando las consideraciones en seguridad de la información usada en los planes de continuidad y función de los resultados del análisis de riesgos.