# Stack trace.

Un ___stack trace___ es un informe de los elementos activos en la [pila de ejecución o pila de llamadas](./Call_Stack.md) en un momento determinado durante la ejecución de un programa.

>  Es una lista de las llamadas a métodos en las que se encontraba la aplicación cuando se disparó una excepción, que muestra la ruta exacta que el código atravesó hasta el punto donde el programa falló. 

El seguimiento de la pila se suele a utilizar durante el _debugging_ interactivo y post-mortem. 

Un seguimiento de pila permite rastrear la secuencia de funciones anidadas llamadas, hasta el punto donde se genera el seguimiento de pila. En un escenario _post-mortem_, esto se extiende hasta la función donde ocurrió la falla (pero no fue necesariamente causada).