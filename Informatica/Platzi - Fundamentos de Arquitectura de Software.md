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

