# Platzi - Introducción al pensamiento computacional 

## Elementos Básicos de Python:

​	Los lenguajes de programación se pueden categorizar de la siguiente manera:

- __Bajo nivel y Alto nivel__: Bajo nivel significa que el lenguaje está mas cerca al lenguaje maquina, mientras que el de Alto nivel esta mas orientado a las personas y se asemeja mas al lenguaje natural. 
- __General y Dominio Especifico:__ Los lenguajes generales tienen como mínimo todos los primitivos de Turing para poder implementar y computar cualquier tipo de algoritmo. Por otro lado los de Dominio Específico son lenguajes especializados a tareas muy especificas.
- __Interpretado y Compilado:__ En los lenguajes interpretados, mientras corre el programa los scripts se van traduciendo al lenguaje maquina o a uno muy cercano a este para poder ser ejecutado, mientras que los Compilados toman las instrucciones y las traducen antes de la ejecución al lenguaje máquina. 

> ​	Python es un lenguajes de alto nivel, general e interpretado.

## Literales y Operadores:

- Los literales son formas simples de inicializar objetos directamente en memoria.

   ``literales = 1, 'abc', 2.0, True``

- Los operadores son los signos con los que podemos operar sobre los literales y ejecutar operaciones algebraicas. 

   ``operadores = + / % ** = ==``

   > ​	Un único paréntesis ``=`` significa asignación de valor, es decir, le asigna un valor a una variable en memoria. Mientras que dos paréntesis ``==`` significa comparación, es decir, compara si dos valores son iguales y retorna un valor buleano.  
   >
   > ​		Las variables son simplemente nombres o IDs que se vinculan con un valor alojado en memoria, y la forma en la que los vinvulamos es a través del operador asignación (``=``).



## Algoritmo:

​	Es una lista finita de instrucciones que describen un cómputo, que cuando se ejecuta con ciertas entradas (inputus), ejecuta pasos intermedios para llegar a un resultado determinado (output).

### 	Búsqueda Binaria:

​	Cuando la respuesta se encuentra en __un conjunto ordenado__, podemos utilizar **búsqueda binaria**. Es altamente eficiente, pues corta el espacio de búsqueda en dos por cada iteración. Los pasos que sigue son:

1. Consideramos como segmento inicial de búsqueda a la lista completa.

2. Analizamos el punto medio del segmento (el valor central), si es el valor buscado, devolvemos el índice del punto medio.

3. Si el valor central es mayor al buscado, podemos descartar el segmento que está desde el punto medio hacia la a derecha.

4. Si el valor central es menor al buscado, podemos descartar el segmento que está desde el punto medio hacia la izquierda.

5. Una vez descartado el segmento que no nos interesa, volvemos a analizar el segmento restante, de la misma forma.

6. Si en algún momento el segmento a analizar tiene longitud 0 o negativa significa que el valor buscado no se encuentra en la lista.

   

   Para verlo de forma gráfica buscaremos el valor 18 en la lista [1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23].

   Para realizar un ejemplo práctico crearemos un programa para buscar raíces cuadradas.

```python
objetivo = int(input('Escoge un numero: '))

epsilon = 0.01  # Definimos nuestro margen de error.

bajo = 0.0      # Inicializamos la parte baja de nuestra búsqueda como 0
alto = max(1.0, objetivo)   # Entre el numero que ingresamos y 1 vamos a tomar el mayor valor.
respuesta = (alto + bajo) / 2   # Definimos la mitad entre bajo y alto.

# Mientras el margen de error sea mayor a epsilon.
while abs(respuesta**2 - objetivo) >= epsilon:

    # Si ((alto+bajo)/2)^2 es menor a nuestro numero objetivo
    if respuesta**2 < objetivo:
        
        # Definimos la parte baja de nuestra búsqueda como (alto + bajo)/2
        bajo = respuesta

    # En caso que (alto+bajo)/2 es mayor a nuestro numero objetivo
    else: 
        # Definimos la parte baja de nuestra búsqueda como (alto + bajo)/2
        alto = respuesta

    # Luego definimos nuevamente la mitad entre alto y bajo.
    respuesta = (alto + bajo) / 2

# Cuando el ciclo ya alcance un error menor a epsilon imprimiremos el resultado.
print(f'La raíz cuadrada de {objetivo} es {respuesta}')
```

## Compilación:

​	Es el proceso que traduce un programa escrito en un lenguaje de programación a otro lenguaje de programación generalmente a un programa equivalente que la maquina será capaz de entender.

## Interpretación:

​	Es una asignación de significados a las expresiones bien formadas de un lenguaje formal. Como los lenguajes formales pueden definirse en términos putamente sintácticos, sus expresiones bien formadas pueden no ser más que cadenas de símbolos sin ningún significado. Una interpretación otorga significado a esas expresiones o formulas. El interprete ejecuta el programa directamente, traduciendo cada sentencia en una secuencia ya compilada en lenguaje maquina.

## Lenguaje Formal:

​	Es un lenguaje cuyos símbolos son primitivos y las reglas para unir esos símbolos están formalmente especificadas. Al conjunto de los símbolos se le llama alfabeto, y al conjunto de las reglas se le llama gramática formal o sintaxis. 

​	A una cadena de símbolos formada de acuerdo a la gramática se le llama una __“expresión bien formada”__ o __”fórmula bien formada del lenguaje”__.

​	Un lenguaje formal es idéntico al conjunto de todas sus formulas bien formadas.

### 	Formula Bien Formada.

​	Es una cadena de caracteres o palabras generadas según una gramática formal o sintaxis o a partir de un alfabeto dado.



## Objeto:

​	Es el resultado de la instanciación de una clase y una encapsulación genérica de datos y de los procedimientos para manipularlos. 

​	Los objetos constan de estado y de un comportamiento, que a su vez consta respectivamente de datos almacenados y de tareas realizables durante el tiempo de ejecución.

​	Un objeto en P.O.O. representa alguna entidad de la vida real, es decir, alguno de los objetos o elementos que pertenecen al negocio en el que trabajamos o al problema con el que nos estamos enfrentando, y con los que podemos interactuar. 

​	Los objetos tienen características fundamentales que nos permiten conocerlos mediante la observación, identificación y el estudio posterior de su comportamiento. Estas características son:

- Identidad.
- Comportamiento.
- Estado.

- ### Identidad de un Objeto:

​	Es la propiedad que permite diferenciar a un objeto y distinguirse de otros. 

​	La identidad de todos los objetos sirve para comparar si dos objetos son iguales o no. Generalmente la identidad de los objetos está determinada por la dirección en memoria.

- ### Comportamiento de un Objeto:

​	Esta directamente relacionado con su funcionalidad y determina las operaciones que este puede realizar o a las que puede responder ante mensajes enviados por otros objetos.

​	La funcionalidad de un objeto está determinada, principalmente, por su responsabilidad y un objeto es más fácil de reutilizar en tanto su responsabilidad sea mejor definida y mas concreta.

- ### Estado de un Objeto:

​	Se refiere al conjunto de atributos y sus valores en un instante de tiempo dado. El comportamiento de un objeto puede modificar el estado de este. 

​	Cuando una operación de un objeto modifica su estado, se dice que tiene efecto colateral.



## Clase:

​	Es un elemento abstracto que define la forma y propiedades de un objeto, podríamos decir que la clase es el molde de un objeto.

> ​	Los objetos son instancias de clases.

​	Las clases se utilizan para representar entidades o conceptos, como los sustantivos en el lenguaje. 

​	Cada objeto creado a partir de una clase se denomina instancia de la clase.

## Instancia:

​	Es la particularización, realización especifica u ocurrencia de una determinada clase.

## Variable:

​	Es un espacio en el sistema de almacenamiento que se asocia e identifica con un nombre simbólico o un identificador. 



## Alcance de las Variables (Scope):

​	El concepto de alcance o “_scope_” determina el contexto en el que una variable esta disponible.

​	El alcance de una variable define los contextos en los que esta está disponible y está accesible. El alcance de una variable depende del lugar del código en donde fue escrita y, al menos en Python se sigue la regla o categorización L.E.G.B.

​	El acrónimo L.E.G.B. significa:

- Local.
- Enclosing (Envolvente).
- Global.
- Built-In (Integrada).

​	Y resume los niveles de alcance que tienen las variables en Python y como hacer al código mas legible, limpio y eficiente. 

- ### Local Scope.

   ​	Es el alcance de las variables definidas dentro de una función. Estas variables solo serán accesibles por la función que las contiene y donde fueron definidas.

- ### Enclosing Scope.

   ​	Es un tipo especial de alcance que solo existe en funciones anidadas, ya que la variable es accesible tanto para la función en donde esta está definida como por la función en donde esta se anida, es decir, una variable definida en una función anidada dentro de otra función es accesible para ambas funciones.

- ### Global (or module) Scope.

   ​	Son las variables que son accesibles desde cualquier parte del programa y es el nivel de alcance más alto en Python.

- ### Built-In Scope.

   ​	Es un tipo de alcance especial que se crea o carga cada vez que se ejecuta una secuencia de comandos, importación o script. Este alcance contiene variables como palabras clave, funciones, excepciones y otros atributos que están integrados en Python.



## Recursividad.

​	Es un termino que se aplica a los métodos o funciones que al ser ejecutadas se llaman a si mismas, pero solo por un numero determinado de veces, y cada llamada o referencia a si misma se denomina como llamada recursiva.

​	La recursión es una alternativa a la iteración o a la implementación de un bucle.

​	La recursión, por su carácter ineficiente y posiblemente peligroso si no tiene un limite claro, no es recomendable si se puede optar por una solución integrada como los bucles, sin embargo es especialmente útil para algoritmos de búsqueda u organización. 

## Funciones como Objetos.

​	En Python todo es un objeto, incluyendo las funciones, las cuales tienen las siguientes características:

- Tienen un tipo.
- Se pueden pasar como argumento.
- Se pueden utilizar en expresiones.
- Se pueden incluir en estructuras de datos como listas, tuplas, diccionarios, etc.



# Tipos estructurales de datos y mutabilidad.

## Tuplas:

​	Son secuencias inmutables de objetos, es decir, una variable con un id que apunta a un lugar en memoria pero que no puede ser modificada, pero si puede ser reasignada. Las tuplas pueden contener cualquier tipo de valor y permite que una función retorne varios objetos y hasta de diferente tipo.

- Son secuencias inmutables de objetos.
- A diferencia de las cadenas pueden contener cualquier tipo de objeto.
- Pueden utilizarse para devolver varios valores en una función.
- Consumen menos memoria que otros tipos de variables.

## Rangos ( range() ):

- Es una función integrada de Python que representa una secuencia de enteros.
- Es un objeto en si mismo.
- Admite tres argumentos, que serían: range(comienzo, fin, pasos)
- Al igual que las cadenas y las tuplas, los rangos son inmutables.
- Muy eficientes en uso de memoria y normalmente utilizados en ``for`` _loops_.

## Listas y Mutabilidad:

- Una lista consta de objetos mutables. (Objetos que se pueden cambiar después de la creación)
- Cuando se modifica una lista pueden ocurrir efectos secundarios ya que diferentes variables pueden apuntar al mismo espacio en memoria, y al modificar alguna de estar variables se modificarían todas, pudiendo causar problemas.

- La lista tiene una gran memoria.

- La lista se almacena en dos bloques de memoria (uno es de tamaño fijo y el otro es de tamaño variable para almacenar datos)

- Crear una lista es más lento porque se necesita acceder a dos bloques de memoria.

- Un elemento en una lista se puede eliminar o reemplazar.
- [Métodos de un objeto List.](https://docs.python.org/3/tutorial/datastructures.html#more-on-lists)
- Para clonar una lista podemos utilizar la función ``list()`` de Python, ingresamos la lista que queremos clonar como argumento y la función nos retorna una lista con un id diferente. También podemos utilizar la notación de _slicing_ = ``[::]``, que le ordenaría a Python copiar la lista de principio a fin, de esta manera ``lista_2 = lista_1[::]``. De esta manera podemos clonar listas con sus propias direcciones en memoria.

## Diccionarios:

- Son similares a las listas, pero en lugar de usar índices utilizan llaves.
- No tienen un orden interno.
- Los diccionarios son mutables.



## Pruebas y Debugging:

### 	Los  7 principios de Testing  de acuerdo al libro de ISTQB.

- **1 - Las pruebas muestran la presencia de defectos**
  
   ​	Significa que las pruebas pueden demostrar que EXISTEN problemas, pero no que los problemas NO EXISTEN.
   El objetivo principal de llevar a cabo una prueba es para detectar defectos. Trabajando bajo la premisa de que cada producto contiene defectos de algún tipo, una prueba que revela los errores es generalmente mejor que una que no lo hace. Todas las pruebas por lo tanto, deben ser diseñados para revelar tantos errores como sea posible
   
- **2 - Las pruebas exhaustivas son imposibles**
  
   ​	Las pruebas exhaustivas tratan de cubrir todas las combinaciones posibles de datos en el software, a fin de garantizar que ninguna situación puede surgir, una vez probado el software se ha liberado. Excepto en aplicaciones muy simples, el número de combinaciones posibles de datos es demasiado alta, es más eficaz y eficiente que los ingenieros de pruebas se centren en las funcionalidades de acuerdo a riesgos y prioridades.
   
- **3 - Pruebas tempranas.**
  
   ​	Un producto (incluyendo los documentos, tales como la especificación del producto) se puede probar tan pronto como se ha creado. ISTQB recomienda probar un producto tan pronto como sea posible, corregir los errores más rápidamente posible. Los estudios han demostrado que los errores identificados al final del proceso de desarrollo por lo general cuestan más para resolver.
   Por ejemplo: un error encontrado en las especificaciones puede ser bastante sencillo de solucionar. Sin embargo, si ese error se transfiere a la codificación de software, una vez descubierto el error puede ser muy costoso y consume tiempo.
   
- **4 - Agrupamiento de Defectos**
  
   ​	Los estudios sugieren que los problemas en un elemento de software tienden a agruparse en torno a un conjunto limitado de módulos o áreas. Una vez que estas áreas han sido identificadas, los administradores eficientes de prueba son capaces de enfocar las pruebas en las zonas sensibles, mientras que siguen buscando a los errores en los módulos de software restantes. Me recuerda al 80/20.
   
- **5 - La paradoja del “Pesticida”**
  
   ​	Al igual que el sobre uso de un pesticida, un conjunto de pruebas que se utilizan repetidamente en el disminuirá en su eficacia. Usando una variedad de pruebas y técnicas expondrá una serie de defectos a través de las diferentes áreas del producto.
   
- **6 - La prueba es dependiente del contexto**
  
   ​	Las mismas pruebas no se deben aplicar en todos los ámbitos. Distintos productos de software tienen diferentes requisitos, funciones y propósitos. Una prueba diseñada para realizarse en un sitio web, por ejemplo, puede ser menos eficaz cuando se aplica a una aplicación de intranet. Una prueba diseñada para una forma de pago con tarjeta de crédito puede ser innecesariamente rigurosa si se realiza en un foro de discusión.
   En general, cuanto mayor es la probabilidad y el impacto de los daños causados por el software fallado, mayor es la inversión en la realización de pruebas de software.
   
- **7 - La falacia de ausencia de errores**

   ​	Declarar que una prueba no ha descubierto ningún error no es lo mismo que declarar que el software es “libre de errores”. Con el fin de garantizar que los procedimientos adecuados de software de prueba se lleva a cabo en todas las situaciones, los evaluadores deben asumir que todo el software contiene algunos (aunque disimulada) errores.

### Pruebas de Caja Negra:

​	Las pruebas de caja negra se basan en la especificación de la función o el programa, aquí debemos probar sus inputs y validar los outputs. Se llama de caja negra porque no necesitamos conocer exactamente los procesos internos que el programa ejecuta, solo contrastar sus resultados.

​	Estos tipos de pruebas son útiles para dos tipos de tests:

- __Unit Testing:__ Se realizan pruebas a cada uno de los módulos para determinar su correcto funcionamiento.

- __Integration Testing:__ Se realizan pruebas para verificar que todos los módulos funcionan adecuadamente al interactuar entre ellos.

   

   ​	Es una **buena práctica** realizar los test **antes** de crear tus lineas de código, esto es por que cualquier cambio que se realice a futuro los *test* estarán incorporados para determinar si los cambios cumplen lo esperado.

   ### Pruebas de Caja de Cristal:

​	Se basan en el flujo del programa, por lo que se asume que conocemos el funcionamiento del programa, por lo que podemos probar todos los caminos posibles de una función. Esto significa que vamos a probar las ramificaciones, bucles, recursiones, etc.

​	Este tipo de pruebas son muy buenas cuando debemos realizar __Repression Testing__ o __Mocks__, que es cuando debemos descubrir bugs al momento de correr el programa, por lo que vamos a buscar el bug gracias a que conocemos como esta estructurado el código.



## Excepciones y Afirmaciones:

### Manejo de Excepciones:

​	Las **excepciones** de Python normalmente se relacionan con errores de semántica, también podemos crear nuestras propias **excepciones**, pero cuando una **excepción** no se maneja (*unhandled exception*), el programa termina en error.

​	Las **excepciones** se manejan con los keywords: **try, except, finally.** Se pueden utilizar también para *ramificar* programas.

​	No deben manejarse de manera silenciosa (por ejemplo, con print statements). Para crear tu propia excepción utiliza el keyword *raise*.

### Afirmaciones:

​	Las afirmaciones son un método de programación defensiva que sirve para verificar que los inputs cumplan con las características y condiciones que nosotros requerimos para el programa, aunque también sirven para debugear un programa. 

​	Se representa en Python con el método ``assert``.



# Examen:

¿Qué es lo que aportó el Telar de Jaquard al concepto de computadora?

Tarjetas perforadas que representan información.



2.

¿Cuál fue la primera computadora digital?

ENIAC



3.

¿En qué rama del conocimiento se encuentran los algoritmos?

Imperativo



4.

¿Con un lenguaje de programación de tipo “Turing Complete” se puede implementar cualquier algoritmo?

Verdadero



5.

Cuando un lenguaje de programación es de alto nivel significa que:

Está enfocado en el entendimiento de los humanos.



6.

¿Qué implica escribir código en un lenguaje compilado?

Se debe convertir el código en un lenguaje máquina antes de entregarlo a la computadora.



7.

De las siguientes opciones, ¿cuáles son literales?

15, 'abc', 3.5, False



8.

¿Qué sucede si se introduce 5 / 'Platzi' en la consola de Python?

Se muestra un TypeError.



9.

¿Qué son las variables?

Nombres que se vinculan con un valor en memoria a través del operador de asignación.



10.

Como buena práctica, ¿las variables deben tener un nombre que signifique algo para la persona que programa?

Verdadero



11.

¿Qué sucede al realizar la operación ‘123’ + ‘456’?

Python imprime 123456.



12.

Si ejecutas el siguiente código en la consola de Python:

```
a = True
b = False
print (a and b) 
```

¿Cuál sería el resultado?

False



13.

El condicional elif sirve para:

Encadenar otra condición en caso de que if sea falso.



14.

¿Cuál es la ventaja de las iteraciones (loops) comparado con los programas ramíficados?

Establecer que una instrucción se repita constantemente hasta llegar a un resultado en específico.



15.

El algoritmo de enumeración exhaustiva consiste en:

Identificar todas las posibilidades para llegar a un resultado.



16.

¿Cuál es la instrucción de Python que nos permite ver en consola el registro de las soluciones que están dando en un programa?

print



17.

¿Qué hace eficiente al algoritmo de búsqueda binaria?

Buscar rápidamente cuando nuestro conjunto de datos está ordenado.



18.

¿Es una buena práctica escribir largos archivos de código con programas ramificados?

No



19.

La descomposición permite:

Dividir el código en componentes que colaboran con un fin en común.



20.

Una buena forma de identificar nuestros errores en el código es a través del:

print statement