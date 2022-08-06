# 1 - Introducción a la seguridad.

---

## 1.1 - Introducción a la seguridad de la información.

     El objetivo de la __<u>seguridad informática</u>__  es el de proteger a los distintos elementos informáticos activos. los principales elementos a proteger son:

- La infraestructura del equipo.
- Los usuarios.
- La información.

### Terminos relacionados con la seguridad informática:

- __Amenaza:__ Es una situación, evento o persona que tiene el objetivo de causar un daño a un sistema en forma de robo, destrucción, divulgación, modificación de datos, etc.

  Persona o cosa que representa un peligro.

- __Antivirus:__ Software dedicado a la seguridad el cual da protección a un equipo de virus, habitialmente mediante la detección en tiempo real y también mediante análisis del sistema, que pone en cuarentena y elimina los virus. 

- __Blacklisting:__ Es un proceso para identificar y bloquear programas, correos electronicos, direcciones o dominios IP conocidos o maliciosos. 

- __Botnet:__ hace referencia a un conjunto o red de robots informáticos o bots, que se ejecutan de manera autónoma y automática. El artífice de la botnet puede controlar todos los ordenadores/servidores infectados de forma remota.

- __Crimeware__: Software que lleva a cabo acciones ilegales no previstas por un usuario que ejecuta el softwaer. El objectivo de estas acciones es producir beneficios económicos al distribuidor del software.

- __Vulnerabilidades:__ Hace referencia a los puntos débiles que, al ser explotados por amenazas, afectan directamente a la confidencialidad, disponibilidad e integridad de la información de un usuario o empresa.

- __Troyano:__ Es un malware que se presenta al usuario como un programa aparentemente legítimo e inofensivo, pero que, al ser ejecutado infecta al dispositivo. 

- __Exploits:__ Son técnicas que utilizan las vulnerabilidades, un fragmento de software, fragmento de datos o secuencia de comandos o accione del software, que pueden ser usadas para esquivar la seguridad o realizar un ataque a un equipo en la red.

---

## 1.2 - Modelo de ciclo de vida de la seguridad de la información.

* __Seguridad Informatica: __ Es la protección de las infraestructuras tecnológicas sobre las que trabaja la empresa u organización y "seguridad de la información", que tiene como objetivo la protección de sistemas e información en cuanto a que éstos siempre se encuentren accesibles, que no sufran alteraciones malintencionadas o por error y que su acceso se permita exclusivamente a personas autorizadas en la forma debida. 

* __Seguridad de la información: __ Tiene como fin <u>la protección de la información, su confidencialidad, integridad y disponibilidad</u>,  y de los sistemas de información del acceso, uso, divulgación, interrupción o destrucción no autorizada. 
  * __Confidencialidad: __ Propiedad que permite impedir la propagación de una información a personas no autorizadas. Asegura que sólo las personas autorizadas puedan acceder a la información. 
  * __Integridad: __ Capacidad para mantener la información sin alteraciones o modificaciones sin alteraciones o modificaciones no permitidas. 
  * __Disponibilidad: __ Cualidad de la información por la que ésta permanece accesible sin interrupciones para aquellas personas autorizadas del sistema. 
  
  ---
  ## 1.3 - Políticas de seguridad.

     Las politicas de seguridad de la información sientan las bases de la seguridad consritutendo la redacción de los objectivos generales y las implantaciones que ha llevado a cabo la organización.

     Pretenden indicar las líneas generales para conseguir los objetivos marcados, sin entrar en detalles técnicos.

	Deben ser conocidas por todo el personal de la organización. 

	

	Existen tres supuestos principales en los que es imprescindible la revisiónactualización de la política de seguridad.

- Despues de producirse graves incidentes de seguridad.
- Desués de una auditoria de sistemas infructuosa o sin éxito. 
- Frente a cambios queafectan a la estructura de la organización. 

---

## 1.7 Lista de amenazas para la seguridad de la información.

	Las amenazas a los sistemas informáticos son situaciones que en potencia pueden causar violaciones de seguridad que afectan a la <u>confidencioalidad, la integridad, la disponibilidad</u> o el uso legítimo de un recurso.

- __Interrupción:__ En este tipo de amenaza, un activo o componenete del sistema, fundamental para la realización del proceso, se destruye o deja de estar disponible (el ataque se produce hacia la disponibilidad del sistema).
- __Intercepcion:__ Ocurre cuando un tercero no autorizado obtiene acceso a un recurso. El ataque se produce en este caso contra la confidencialidad.
- __Modificación:__ En este tipo de ataque, no solo se accede de forma ilicíta a un recurso, sino que este recurso es modificado o manipulado. 
- __Fabricación:__ En este tipo de ataque se atenta contra la autenticidad de los recursos o componenetes de un sistema. Una entidad no autorizada inserta objetos falsificados en el sistema. 

__<u>Clasificación según el origen de la amenaza:</u>__

- __Amenazas naturales:__ Inundaciones, tormentas, explosiones, fallos electricos, etc.
- __Amenazas de agentes externos:__ Ataque de una organización criminal, sabotaje, estagas, intrusos en la red interna, disturbios, conflictos sociales, etc.
- __Amenazas de agentes internos:__ Errores en el uso de herramientas, empleados descontentos o ignorantes de los procesos internos, etc.

__<u>Clasificación según la intencionalidad de la amenaza:</u>__ 

- __Accidentes:__ Averías de la alimentación eléctrica, fallos de software, meteorología, etc.
- __Errores:__ Fallos durante la ejecución de procedimientos, errores de desarrollo de una aplicación del sistema, modificaciones accidentales o por desconocimiento, etc.
- __Actos malintencionados:__ Sabotajes, robos, fraudes, intentos de acceso ilegítimos, etc.

---

## 1.8 Vulnerabilidades.

	Son puntos débiles de un sistema informático que permiten que un atacante comprometa la integridad, disponibilidad o confiencialidad del mismo, causando un perjuicio al sistema o a la organización a la que este pertenece. 
	
	Las vulnerabilidades pueden tener su origen en defectos de fabricación del material informático, fallos en los sistemas físicos o en el software, mantenimiento de los equipos, manipulación humana, procesos ambiguos o mal definidos, errores de programación o bugs, existencia de puertas traseras, etc.

__Vulnerabilidades según el activo afectado:__ 

- __Que afecten al hardware.__
- __Que afecten al software.__ 
- __Que afecten al diseño de los protocolos y cifrados utilizados en las redes.__
- __Que afecten a las políticas de seguridad de la información.__ 
- __Que afecten a los usuarios.__

---

## 1.9 Vulnerabilidades en sistemas Windows.

__Metodos para mejorar la seguridad del sistema Windows.__

- Eliminar cuentas y servicios innecesarios del sistema y cambiar los privilegios de los usuarios por defecto. (Asignar siempre una contraseña a los usuarios del sistema y no deshabilitar el sistema UAC).

	>	__UAC__ significa "User Account Control" y se trata de un control de seguridad que está destinado a avisarte e incluso impedir que se hagan cambios no autorizados en el ordenador, y así asegurarte de que ninguna aplicación modifique nada importante por sí solo.

- Usas siempre el sistema de archivos NTFS.

  > 	__NTFS__ significa "New Technology File System" y se trata de un sistema de archivos que sirve para organizar fatos en discos duros y otros soportes de almacenamiento. En __NTFS__, tosos los datos relativos a los archivos guardados se registran en la tabla maestra de archivos o __Master File Table__ (__MFT__). 
  >		
  > 	Se trata de un índice que contiene, entre otras cosas, información acerca de qué bloques del soporte de almacenamiento pertenecen a qué archivos y qué permisos de acceso y atributos tiene cada archivo.

- Usar el comando `netstat -a` en la consola de Windows para detectar servicios de red que no se estén usando y desinstalarlos o deshabilitarlos. 

- Usar siempre la última versión del protocolo de autenticación y de la red de Windows (Protocolo NTLM-2 y SMB) y deshabilitar las compartición de carpetas sin usuario y contraseña.

  > 	__NTLM__ significa "New Technology LAN Manager" y consiste en una serie de protocolos de autenticación que permite que diferentes ordenadores y servidoresse verifiquen entre sí. 

  ```sequence
  Cliente->Host: Solicitud de autenticación.
  Note over Cliente, Host: El cliente envía un nombre de usuaios al host.
  Host -> Cliente: Desafío NTLM.
  Note over Cliente, Host: El host response con un número aleatorio.
  Cliente -> Host: Respueste NTLM.
  Note over Cliente, Host: El cliente response con un valor hash.
  Host -> Cliente: Confirmación/Rechazo.
  Note over Cliente, Host: El host autoriza o bloquea el acceso.
  
  ```

- Aplicar políticas de complejidad e histórico de contraseñas, para evitar la reutilización de las mismas.

- Restringir el acceso a carpetas y ficheros del sistema a partir de ACL de Windows (sólo en el sistema NTFS), y proteger el acceso al registro de Windows.

  > __ACL__ significa "access control list", y es una forma de determinar los permisos de acceso a propiados a un determinado objeto, dependiendo de ciertos aspectos del proceso que hace el pedido.

---

## 1.10 Vulnerabilidades en aplicaciones multiplataforma. 

	Las aplicaciones web o aplicaciones multiplataforma, generalmente emplean una arquitectura de sistema cliente-servidor, y varían en complejidad y funcionalidad. 

> Se consideran 'multiplataforma' ya que, idealmente, se puede acceder desde cualquier navegador web y en diferentes sistemas operativos.

Entre las vulnerabilidades de los sistemas web, se encuentran:

- __Inyección de codigo:__ Introducción de código externo en la aplicación web, y sucede cuando los datos pasan sin filtrar directamente como parte de la consulta. Se puede usar para acceder a datos sin autorización o para ejecutar comandos, siendo las inyecciones de SQL las más comunes. 
- __Gestión de la sesión del usuario:__ Corresponse al mal manejo de las sesiones en aquellas aplicaciones que utilizan autenticación, permitiendo que usuarios accedan y utilicen la cuenta de otros, listas de claves, etc. 
- __Cross-Site Scripting (XSS):__ Ocurre cuando existe una validación incompleta de la información ingresada por el atacante. 
- __Referencia directa a objetos inseguros (IDOR):__ Exposición de estructura interna y de elementos de desarrollo que permita al atacante suponer métodos y datos predecibles. 
- __Errores de configuración:__ Malas configuraciones de seguridad a nivel de framework, sistemas operativos, aplicaciones de terceros, etc.
- __Falta de control de nivel de acceso a funciones:__ Mediante la alteración de una URL o de un parámetro, se accede a una función sobre la cual no se tiene privilegios.
- __Intercepción de peticiones entre sitios (CSRF):__ Permite generar peticiones falsas de forma que el usuario piense que las está realizando en el sitio correcto cuando se trata de uno falso. 
- __Uso de componenetes vulnerables:__ Componentes usados en una aplicación que tienen vulnerabilidades conocidas y podrían ser detectadas mediante un análisis automático. 
- __Falta de validación de redirecciones:__ Un enlace legítimo de la aplicación, una vez cargada, redirigída hacia otro sitio sobre el cual el atacante puede tener control.

---



## 1.12 Buenas practicas y salvaguardas para la seguridad.



En la revision de equipos y servidores se deberían de analizer y evaluar los siguientes aspectos:

- Parches del sistema Operativo.
- Seguridad del Sistema de Ficheros. 
- Cuentas de usuarios.
- Servicios y aplicaciones instaladas.
- Protocolos y servicios de red. 
- Control de accesos  a los recursos.
- Registro y auditoría de eventos.
- Configuración de las herramientas de seguriad: antivirus, cortafuegos personales, gestores de copias de seguridad, gestores de contraseñas, etc.
  -      Aspectos a tener en cuenta a la hora de utilizar herramientas para el análisis y evaluación de vulnerabilidades en el sistema informático:
    - Definición del alcance y objetivos de las pruebas a realizar.
    - Conocimiento y experiencia del equipo que analiza las vulnerabilidades y realiza las pruebas de intrusión en el sistema.
    - Nivel de automatización de las pruebas realizadas.
    - Actualización periódica de la base de datos de vulnerabilidades a analizar.
    - Controlar y limitar los posibles riesgos que se deriven de las pruebas.
    - Realización de las pruebas de forma periódica o en momentos puntuales.
    - Registrar las puntuaciones y resultados obtenidos en las distintas pruebas realizadas.

## 1.13 Recomendaciones para la seguridad de la res.

1. __Configuración adecuada del equipo informático:__ Servicios instalados, cuentas y grupos de usuarios, contraseñas, permisos de acceso, etc.

2. __Revisión y actualización de los softwares instalados.__

3. __Configuración del nivel de seguridad en función de la zona de trabajo del usuario:__

   	Se pueden distinguir 4 zonas de trabajo en el navegador:

   1. <u>Zona "internet":</u> Se aplica al nivel de seguridad medio, en el que se permite la ejecución de applets java, o scripts, así como la descarga de ficheros desde internet, pero solicitando confirmación antes de ejecutar controles ActiveX.
   2. <u>Zona "intranet local":</u> Reservada para Websites dentro de la red local, que se supone más segura que el internet. Se aplica el nivel de seguridad medio-bajo, similar al medio pero con menos restricciones.
   3. <u>Zona de "sitios de confianza":</u> Pensada para aquellos websites que no se consideran como una amenaza para el equipo. Se aplica el nivel de seguridad bajo.
   4. <u>Zona de "sition restringidos":</u> Pensada para aquellos websites que se consideran peligrosos. Se aplica en este caso el nivel de seguridad alto, en el que se inhabilida la ejecución de código activo, asi como descarga de ficheros.

4. __Control de la utilización de "cookies":__ una __cookie__ es un pequeño fichero de texto que se guarda en el disco duro del equipo del usuario y que permite recordar el servidor web, algunos datos sobre el usuario.

5. __Control del contenido activo en las páginas web:__ Estos componenetes y "miniaplicaciones" de código activo, pódrian comprometer la seguridad del equipo en que se ejecutan. 

6. __Conexión a servidores web seguros mediante protocolos de encriptación:__ En determinadas conexiones a servidores web, la comunicación debería estar cifrada mediante el protocolo SSL. Para ello, el navegador se encarga de abrir una sesión HTTP sobre un canal SSL, inficándolo mediante el texto "https://" que se incluye al comienzo de la dirección de la pagina web. 

7. __Control de los contenidos que se pueden visualizar:__ El propio navegador, generalmente, dispone de una herramienta (llamada "asesor de contenido") que permite restringir el acceso a páginas con determinado tipo de contenidos. Para ello, se utiliza la clasificación de contenidos en distintas categorías que ha sido propuesta por la ICRA62 (Internet Content Rating Association).

---



## 1.14 Recuerda.

- La irrupción y el desarrollo actual de las nuevas tecnologías están dando lugar a una serie de cambios estructurales a distintos niveles: económico, laboral, social, educativo, político, relacional, etc.
- La __disponibilidad__ asegura que el acceso sin interrupciones a los datos o a los recursos de información por personal autorizado, se produce correctamente y en el tiempo.
- Para la seguridad de la información, la __Integridad__ es la propiedad que busca mantener los datos libres de modificaciones no autorizadas.
- Generalmente, la seguridad de los sistemas informáticos se concentra en __garantizar el derecho a acceder a datos y recursos del sistema__ configurando los mecanismos de autentificación y control que aseguran que los usuarios de estos recursos sólo posean los derechos que se les han otorgado. 