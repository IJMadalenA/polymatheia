# Python - Clase I.

## ¿Que es Python?

Python es un lenguaje de programación de __alto nivel__, __interpretado__, de __tipado dinámico__, __multipropósito__ y __orientado a objetos__.

Python fue creado por el neerlandés [__Guido Van Rossum__](https://es.wikipedia.org/wiki/Guido_van_Rossum) quien comenzó a trabajar en su desarrollo en 1989, en sus vacaciones de navidad, para luego presentarlo en febrero de 1991 como una alternativa y a su vez inspirado en el lenguaje __ABC__, un lenguaje que estaba desarrollando en el __WCI__, en un centro holandés de investigación en el que, entre muchas otras cosas, se encuentran las oficinas centrales del [__W3C__](https://es.wikipedia.org/wiki/World_Wide_Web_Consortium). Sin embargo __ABC__, en contraposición al no nacido Python, era mas difícil de leer y fue bastante difícil de difundir. 

Guido comenzó a trabajar en el desarrollo de Python con tres máximas en su cabeza:

- Que fuese fácil leer. 
- Que fuese sencillo.
- Que fuese un lenguaje de _scripting_.

Python se sigue ciñendo a los primeros dos propósitos, pero actualmente solo responde al tercero a medias, ya que este lenguaje puede ser utilizado para todo (o casi todo), desde escribir simples _scripts_ para tareas simples y repetitivas, hasta para desarrollar grandes aplicaciones y/o servidores web que proveen servicio perpetuo e ininterrumpido. 

> El nombre "Python" viene dado por la afición de Van Rossum al grupo [Monty Python](https://es.wikipedia.org/wiki/Monty_Python).

## Un lenguaje para dominarlos a todos.

A [__Guido Van Rossum__](https://es.wikipedia.org/wiki/Guido_van_Rossum) se le conoce como [__Benevolent Dictator for Life__](https://es.wikipedia.org/wiki/Benevolent_Dictator_for_Life), un titulo que representa bastante bien la filosofía del lenguaje, en donde se prima fundamentalmente dos cosas: la __legibilidad__ y la __transparencia__, y para ello se han ido diseñando a lo largo del tiempo una serie de acuerdos y estándares, todos ellos recogidos en los documentos [PEP](https://peps.python.org/) (_Python Enhancement Proposals_), pensando siempre en la colaboración y hasta llegando a considerar un sentido estético durante el desarrollo.  

> Un ejemplo bastante paradigmático de esta filosofía de consenso y estandarización es el [PEP8](https://peps.python.org/pep-0008/), el cual describe pormenorizadamente como redactar el código Python en lo relativo al estilo. 

__Tim Peters__, un exper to desarrollador de Python escribió el Zen de Python, una serie de enunciados que resumen la filosofía del lenguaje.

```sh
>>> import this

- Bello es mejor que feo.
- Explícito es mejor que implícito.
- Simple es mejor que complejo.
- Complejo es mejor que complicado.
- Plano es mejor que anidado.
- Disperso es mejor que denso.
- La legibilidad cuenta.
- Los casos especiales no son tan especiales como para quebrantar las reglas.
- Lo práctico gana a lo puro.
- Los errores nunca deberían dejarse pasar silenciosamente.
- A menos que hayan sido silenciados explícitamente.
- Frente a la ambigüedad, rechaza la tentación de adivinar.
- Debería haber una —y preferiblemente solo una— manera obvia de hacerlo.
- Aunque esa manera puede no ser obvia al principio a menos que usted sea holandés.
- Ahora es mejor que nunca.
- Aunque nunca es a menudo mejor que ya mismo.
- Si la implementación es difícil de explicar, es una mala idea.
- Si la implementación es fácil de explicar, puede que sea una buena idea.
- Los espacios de nombres (namespaces) son una gran idea ¡Hagamos más de esas cosas!

```



### Lenguaje de alto nivel.

Se refiere a su __nivel de abstracción__, es decir, en cuanto a la especifico o general que es respecto a la arquitectura de computación inherente al sistema que se está utilizando, o en palabras más simples, es que tan cerca o lejos está del lenguaje maquina, sus requerimientos y especificaciones.

### Interpretado.

Es una asignación de significados a las fórmulas bien formadas de un lenguaje de programación. 

Un lenguaje interpretado es aquel que el código fuente se ejecuta directamente, instrucción tras instrucción.

Es decir, el código no pasa por un proceso de compilación, sino que tenemos un programa llamado intérprete que lee la instrucción en tiempo real, y la ejecuta.

El intérprete de Python realiza las siguientes tareas para ejecutar un programa:

- **Paso 1** : El intérprete lee un código o instrucción python. Luego verifica que la instrucción esté bien formateada, es decir, comprueba la sintaxis de cada línea. Si encuentra algún error, detiene inmediatamente la traducción y muestra un mensaje de error.
- **Paso 2** : Si no hay ningún error, es decir, si la instrucción o el código python está bien formateado, el intérprete lo traduce a su forma equivalente en un lenguaje intermedio llamado «código Byte». Así, después de la ejecución exitosa de la escritura o el código python, se traduce completamente en código Byte.
- **Paso 3**: El código del byte se envía a la Máquina Virtual Python, donde de nuevo se ejecuta el código del byte en PVM. Si se produce un error durante esta ejecución, ésta se detiene con un mensaje de error.

> Una **fórmula \*bien formada\***, también llamada **expresión \*bien formada\***, es una cadena de caracteres o palabra generada según una gramática formal a partir de un alfabeto dado. Un lenguaje formal se define como el conjunto de todas sus fórmulas bien formadas.

### Tipado dinámico.

Python es un lenguaje __dinámicamente tipado__ si una variable puede tomar valores de distintos tipos, y es una característica común de los lenguajes interpretado, ya que la comprobación de tipificación se realiza durante la ejecución, en vez de durante la compilación. 

Comparado con el tipado estático, este tipo de tipado es más flexible, a pesar de ejecutarse más lentamente y ser más propensos a contener errores de programación.

````python
variable_1 = 123

variable_1 = "123"
````

### Orientado a objetos.





---

## Bibliografía. 

https://docs.python.org/es/3/tutorial/appetite.html

https://ellibrodepython.com/

---