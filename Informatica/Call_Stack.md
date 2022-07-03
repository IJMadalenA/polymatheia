# Call stack.

## Definición.

La ___call stack___, __pila de llamadas__ o __pila de ejecución__, es una estructura dinámica de datos ___LIFO___ (_last in, first out_), que almacena información sobre las subrutinas de una aplicación.

Es un mecanismo para que un intérprete realice un seguimiento de en que lugar se llama a múltiples funciones, qué función se esta ejecutando actualmente y qué funciones son llamadas desde esa función, etc.

- Cuando un _sript_ llama a una función, el intérprete la añade a la pila de llamadas y luego empieza a ejecutar la función.
- Cualquier función o funciones que sean llamadas por esa función son añadidas arriba de la pila de llamadas y serán ejecutadas cuando su llamada sea alcanzada. 
- Cuando la función actual termina, el intérprete la elimina de la pila y reanuda la ejecución donde se quedó.
- Si la pila necesita más espacio del que se le asignó, se producirá un error de "desbordamiento de pila" o "stack overflow". 

> Una pila de llamadas es una estructura de datos en pila, pero hay diferentes tipos de pila. Es decir, todas las pilas de llamadas son estructuras de ordenación en pila pero no todas las estructuras en pila son pilas de llamadas.



## Implementación en aplicaciones informáticas.

Imaginemos que llamamos a una función que en su interior llama a otra función. Cuando el proceso llega a la función anidada, la primera función se abandona, es decir abandonamos su procesamiento para procesar la función definida dentro de la primera, pero antes de procesar la segunda función se almacena en una pila la dirección que apunta a la primera función, que queda en cola. Ahora supongamos que esa nueva función llama a su vez a otra función, igualmente se almacena la dirección de esta segunda función, se abandona su ejecución y se atiende la nueva petición. Así en tantos casos como existan peticiones. De este modo se va generando una pila de procesos que se van ejecutando siguiendo una estructura ___LIFO___.

La ventaja de la pila es que no requiere definir ninguna estructura de control ni conocer las veces que el programa estará saltando entre funciones para después retomarlas, con la única limitación de la capacidad de almacenamiento de la pila. Conforme se van cerrando las funciones, se van rescatando las funciones precedentes mediante sus direcciones almacenadas en la pila y se va concluyendo su proceso, esto hasta llegar a la primera.



---

[Pila de llamadas - Wikipedia, la enciclopedia libre](https://es.wikipedia.org/wiki/Pila_de_llamadas)

[Pila (informática) - Wikipedia, la enciclopedia libre](https://es.wikipedia.org/wiki/Pila_(informática))

