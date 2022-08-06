# Platzi - Programación Orientada a Objetos.

​	La programación orientada a objetos (de ahora en adelante: __POO__), es un paradigma de la programación que utiliza objetos en sus interacciones, para diseñar aplicaciones y programas informáticos. Los objetos se utilizan como metáfora para emular las entidades reales del proyecto o negocio que se pretende modelar.

> __Paradigma__: Es una teoría que suministra la base y modelo para resolver problemas.

Y está compuesto por 4 tipos de elementos fundamentales, que son:

- __Clases__: Es el modelo sobre el cual se construirán los objetos.
- __Propiedades__:
- __Métodos__: Son las funciones propias de una clase, es decir, las acciones que esta puede realizar. 
- __Objetos__: Son agrupaciones de datos que poseen métodos, los cuales operan sobre dichos datos.

---

## Características de la POO.

- __Uso de funciones__: En la programación orientada a objetos no se asume el problema de manera global, sino que se fragmenta en tantos subproblemas como se deseen. Cada fragmento es solucionado mediante una función y la suma de todas las soluciones debe resolver el problema global.

- __Mayor orden__: El estructurar el código en pequeños bloques llamados funciones nos permite organizar el código de una forma más clara y entendible, y si el código se entiende, cualquier otra persona podrá actualizarlo o reutilizarlo.

- __Reutilización de código__: Al estar el código dispuesto en funciones, y si estas responden a una organización jerárquica, previo un proceso de clasificación, la POO brinda la posibilidad de reutilizar este código, es decir, si tengo una función que lee datos, y a posteriori necesito leer datos, me es suficiente con invocar la función sin necesidad de volverla a escribir en su totalidad.

- **Encapsulamiento**: Es el ocultamiento del estado, es decir, de los datos de un objeto de manera que solo se pueda cambiar mediante las operaciones definidas para ese objeto.

   ​	Cada objeto está aislado del exterior, es un módulo natural, y la aplicación entera se reduce a un agregado o rompecabezas de objetos. El aislamiento protege a los datos asociados de un objeto contra su modificación por quien no tenga derecho de acceder a ellos, eliminando efectos secundarios e interacciones.

- **Abstracción**: Consiste en aislar un elemento de su contexto o del resto de los elementos que lo acompañan. El término se refiere al énfasis en el ¿qué hace? más que en el ¿cómo lo hace?. 

   ​	También se puede entender como el método que se usa al momento de analizar un elemento particular, despreciando los aspectos no relevantes para el contexto especifico y considerando solo las propiedades esenciales, facilitando con ello la comprensión de dicho elemento.

   ​	En POO la abstracción expresa las características esenciales de un objeto, las cuales distinguen al objeto de los demás.

- **Herencia**: Es la relación entre una clase general y otra clase más especifica, en donde la segunda se crea a partir de la primera, heredando todos sus métodos y variables asociadas, pero con el fin de especificar aun más al objeto. 

   ​	Es una propiedad que permite que los objetos sean creados a partir de otros ya existentes, obteniendo características (métodos y atributos) similares a las de los ya existentes. Es la relación entre una clase general y otra clase más específica. Es un mecanismo que nos permite crear clases derivadas a partir de la clase base, nos permite compartir automáticamente métodos y datos entre clases, subclases y objetos.

- **Polimorfismo**: Se refiere a la propiedad por la que es posible enviar mensajes sintácticamente iguales a objetos de tipos distintos. El único requisito que deben cumplir los objetos que se utilizan de manera polimórfica es saber responder al mensaje que se les envía.

   ​	Un objeto polimórfico es una entidad que puede contener valores de diferentes tipos durante la ejecución del programa. Esto aplica principalmente a las funciones y a los operadores.

- __Cohesión__: Se refiere al grado en que los elementos de un módulo permanecen juntos. Por lo tanto, la cohesión mide la fuerza de la relación entre las piezas de funcionalidad dentro de un modulo dado. En un sistema altamente cohesivo, la legibilidad y reusabilidad del código es mayor, mientras que la complejidad se mantiene manejable.

   La cohesión es mayor si:

   - Las funcionalidades embebidas en una clase, accedidas a través de sus métodos, tienen mucho en común.
   - Los métodos realizan un pequeño número de actividades relacionadas, para evitar los trozos grandes de grano o no relacionados con los conjuntos de datos. 

- __Acoplamiento__: Es la forma y nivel de interdependencia entre módulos de software. Una medida de qué tan cercanamente conectados están dos rutinas o módulos de software, así como el grado de fuerza de la relación entre módulos.

   ​	El acoplamiento está comúnmente contrastado con la cohesión. Un bajo acoplamiento normalmente se correlaciona con una alta cohesión, y viceversa. El bajo acoplamiento es frecuentemente una señal de un sistema bien estructurado y de un buen diseño.

---



## Objetos.

 	Son entes abstractos de objetos existentes en el mundo, ya sean estos físicos o conceptuales, que nos permiten separar los diferentes componentes de un programa y nacen como resultado del instanciado de una clase, y se caracterizan por poseer atributos, métodos e identidad.

- __Atributos__: Son los datos que caracterizan al objeto. Son variables que almacenan datos relacionados al estado de un objeto.
- __Método__: Los métodos de un objeto caracterizan su comportamiento, es decir, son todas las acciones, también llamadas operaciones, que el objeto puede realizar por sí mismo. Estas operaciones hacen posible que el objeto responda a las solicitudes externas, o que actúe sobre otros objetos. Además, las operaciones están estrechamente ligadas a los atributos, ya que sus acciones pueden depender de, o modificar, los valores de los atributos.
- __Identidad__: Es lo que lo distingue de otros objetos, sin considerar su estado. Por lo general, esta identidad se crea mediante un identificados que deriva naturalmente de una característica esencial, como un numero de serie, un modelo o un código. 

> ​	Podemos decir que un objeto es todo aquello que podemos percibir con los órganos de los sentidos, es decir que podemos ver, oler, saborear, palpar e inclusive oír. Esto implica que todo cuanto nos rodea puede ser considerado un objeto. Sin embargo el ser humano tiene la posibilidad de concebir cosas mediante su pensamiento, valiéndose de esto para representar situaciones que escapan del ámbito “real”. Esto quiere decir que el término objeto involucra, además de lo real, todo lo abstracto y conceptual, como por ejemplo los números y las letras.
>
> ​	Los objetos, independientemente de su naturaleza, están siempre constituidos por más objetos dispuestos de manera lógica. 

​	De entre todas las clasificaciones de objeto hay dos especiales a tener en cuenta, y son los __objetos físicos__ y los __objetos conceptuales__. Los objetos físicos son todos aquellos que existen materialmente en el mundo, mientras

​	Una forma de identificar a los objetos es utilizando su sustantivo, y a su vez las propiedades que lo componen son aquellos adjetivos que lo caracterizan. Por ejemplo, en un proyecto de carpintería podríamos encontrar al objeto “tabla_de_madera”, el cual tendría los atributos: alto, largo, grosor, tipo_de_madera... y también podríamos tener al objeto “plano_del_mueble”, con los atributos: alto, largo, cantidad_de_madera, nombre_diseñador, metros_cuadrados_de_madera, entre otras tantas propiedades que se nos puedan ocurrir que compongan al objeto. 

​	La madera es un objeto físico, es algo que existe en la vida real, mientas que el plano es un objeto conceptual, es simplemente una idea con la que necesitamos trabajar.

> ​	Los atributos de los objetos son las características que componen al objeto, y estos deben ser definidos como sustantivos.
>
> ​	Para definir el tamaño, como atributo, del objeto “persona”, no colocamos alto, o 1.73cm, sino que definimos al atributo con el adjetivo: “altura”, y dentro de el ingresamos el valor especifico para ese objeto que estamos creando y manejando, ya que al ingresar valor estamos instanciando al objeto y especificandolo.

---



## Modularidad.

​	Es la propiedad que permite subdividir una aplicación en partes más pequeñas (llamadas módulos), cada una de las cuales debe ser tan independiente como sea posible de la aplicación en sí y de las partes restantes.

​	

## Principio DRY: Don’t Repeat Yourself.

​	Es un principio del desarrollo de software que establece que “Cada pieza de información debe tener una única representación autorizada, sin ambigüedades, dentro de un sistema”. Si se aplica correctamente, la modificación en un elemento del sistema no requerirá de un cambio en otros elementos no relacionados lógicamente.

> ​	Toda pieza de información nunca debería ser duplicada debido a que la duplicación incrementa la dificultad en los cambios y evolución del código.

 

## Getters y Setters en Python.

​	En Python los _getters_ y los _setters_ tienen el objetivo de asegurar el encapsulamiento de datos. Claramente los _getters_ se emplean para obtener los datos, mientras que los _setters_ para cambiar el valor de los datos. Son decoradores y se identifican por tener un __@__.

- Si queremos añadir una lógica de validación para obtener y establecer un valor.
- Para evitar el acceso directo a un atributo de clase (un usuario externo no puede acceder directamente a las variables privadas ni modificarlas.)

​	Python `@property` es uno de los decoradores integrados. El propósito principal de cualquier decorador es cambiar los métodos o atributos de su clase de tal manera que el usuario de su clase no necesite hacer ningún cambio en su código. Por ejemplo

```Python
class Geeks: 
     def __init__(self): 
          self._age = 0
       
     # using property decorator 
     # a getter function 
     @property
     def age(self): 
         print("getter method called") 
         return self._age 
       
     # a setter function 
     @age.setter 
     def age(self, a): 
         if(a < 18): 
            raise ValueError("Sorry you age is below eligibility criteria") 
         print("setter method called") 
         self._age = a 
  
mark = Geeks() 
  
mark.age = 19
  
print(mark.age)
```

```python
>>>setter method called 
>>>getter method called 
>>>19
```



## Property en Python.

​	El decorador `@property` viene por defecto en Python, y puede ser usado para modificar un método para que sea un atributo o propiedad, además de aumentar el encapsulamiento del código, ya que la función no será accesible desde el exterior.



## Introducción a la Complejidad Algorítmica.

​	Es una métrica teórica que nos ayuda a describir el comportamiento de un algoritmo en términos de tiempo de ejecución (tiempo que tarda un algoritmo en resolver un problema) y memoria requerida (cantidad de memoria necesaria para procesar las instrucciones que solucionan dicho problema). Esto nos ayuda a comparar entre la efectividad de un algoritmo y otro, y decidir **cuál es el que nos conviene implementar**.

​	A la idea del tiempo de ejecución se le conoce como **complejidad temporal**, y a la idea de la memoria requerida para resolver el problema se le denomina **complejidad espacial.** Dichos valores se encuentran en función del **tamaño del problema** (valor o valores dictados por el número de elementos con los que un algoritmo trabaja), aunque *en algunos casos no*.

![Ver las imágenes de origen](https://miro.medium.com/max/1400/1*QKI1SYAzdHy9uPypVdP8AQ.png)

### Búsqueda Lineal o Secuencial $$O(1)$$.

​	Es un método para encontrar un valor objetivo dentro de una lista. Ésta comprueba secuencialmente cada elemento de la lista para el valor objetivo hasta que es encontrado o hasta que todos los elementos hayan sido comparados.

​	Este tipo de búsqueda en en tiempo el peor, y marca como máximo ___n___ comparaciones, donde ___n___ es la longitud de la lista. Si la probabilidad de cada elemento para ser buscado es el mismo, entonces la búsqueda lineal tiene una media de n/2 comparaciones, pero esta media puede ser afectado si las probabilidades de búsqueda para cada elemento varían. 

```python
def busqueda_lineal(lista, objetivo):
	match = False
     position = 0
	
	for elemento in lista:
          if elemento == objetivo:ç
               match = True
               break
		position = position + 1
     return match
	
     print( f'El elemento {objetivo} {"esta" if encontrado else "no esta"} en la lista')
```



### Búsqueda Binaria o de Intervalo Medio $$O(log \ n)$$.

​	Es un algoritmo de búsqueda que encuentra la posición de un valor en un array ordenado. Compara el valor con el elemento en el medio del array, si no son iguales, la mitad en la cual el valor no puede estar eliminada y la búsqueda continúa en la mitad restante hasta que el valor se encuentre.

​	La búsqueda binaria es computada en el peor de los casos en un tiempo logarítmico, realizando $$O(log \ n)$$ comparaciones, donde n es el número de elementos del arreglo y log es el logaritmo. La búsqueda binaria requiere solamente $$O(1)$$ en espacio, es decir, que el espacio requerido por el algoritmo es el mismo para cualquier cantidad de elementos en el array.

​	Aunque la idea es simple, implementar la búsqueda binaria correctamente requiere atención a algunos detalles como su condición de parada y el cálculo del punto medio de un intervalo.

> ​	La búsqueda binaria asume que la lista que se le ingresa está ordenada.

```python
import random

def busqueda_binaria(lista, comienzo, final, objetivo):
     tamaño_de_lista = int(input('De que tamano es la lista?'))
     objetivo = int(input('Que numero quieres encontrar?'))
     lista = sorted([random.randint(0, 100) for i in range(tamaño_de_lista)])
     
     if comienzo > final:
          return False
     
     medio = (comienzo + final) // 2
     
     if lista[medio] == objetivo:
          return True
     elif lista[medio] < objetivo:
          # si la función descubre que el objetivo esta en la mitad superior, va a ingresar el valor de mitad + 1 como variable 'inicio' de la función, de esta manera la función se aplicará a ese segmento.
          return busqueda_binaria(lista, medio + 1, final, objetivo)
     else:
          return busqueda_binaria(lista, comienzo, medio - 1, objetivo)
     		# si la función descubre que el objetivo esta en la mitad inferior, va a ingresar el valor de mitad - 1 como variable 'final' de la función, de esta manera la función se aplicará a ese segmento.
     
     encontrado = busqueda_binaria(lista, 0, len(lista), objetivo)
     print(f'El elemento {objetivo} {"esta" if encontrado else "no esta"} en la lista')
          
```



### Ordenamiento de Burbuja $$O(n^2)$$.

​	El ordenamiento de burbuja es un algoritmo que recorre repetidamente una lista que necesita ordenarse. Compara elementos adtacentes y los intercambia si están en el orden incorrecto. Este procedimiento se repite hasta que no se requieran más intercambios, lo que indica que la lista se encuentra ordenada.

```python
import random


def ordenamiento_de_burbuja(lista):
    tamano_de_lista = int(input('De que tamano sera la lista? '))
    lista = [random.randint(0, 100) for i in range(tamano_de_lista)]

    n = len(lista)

    for i in range(n):
        for j in range(0, n - i - 1):

            if lista[j] > lista[j + 1]:
                lista[j], lista[j + 1] = lista[j + 1], lista[j]

    return lista

    print(lista)
    lista_ordenada = ordenamiento_de_burbuja(lista)
    print(lista_ordenada)
```

​	Este algoritmo tiene una relación cuadrática, es decir $$O(n^2)$$, ya que la función ejecuta un bucle dentro de otro bucle, y aunque la segunda lista se hace cada vez mas pequeña la relación no deja de ser cuadrático o si se quiere logarítmica $$O(n) * O(n - i) = O(n * n - i)$$. 



### Ordenamiento por Inserción $$O(n^2)$$.

​	Aunque sigue siendo $$O(n^2)$$, funciona de una manera ligeramente diferente. Siempre mantiene una sublista ordenada en las posiciones inferiores de la lista. Cada ítem nuevo se “inserta” de vuelta en la sublista previa de manera que la sublista ordenada sea un ítem más larga.

​	El algoritmo funciona de la siguiente manera:

​	Por cada iteración, índice _j_ tomará el valor del índice _i_. Después recorrerá de manera inversa la lista evaluando los valores de la lista en la posición _j_ y en la posición _j - 1_.

​	Si el valor en la posición _j - 1_ es mayor al valor en _j_ entonces los dos valores son intercambiados y así se llevará a cabo hasta que el valor de  _j_ sea igual a 0. En la siguiente iteración, el índice _i_ aumenta en uno y _j_ vuelve a tomar el valor de _i_ y se realiza el mismo recorrido hasta que _j_ sea igual a 0.

​	El algoritmo termina hasta que el índice _i_ haya recorrido todo el vector y no haya más remplazos durante el recorrido del índice _j_.

```Python
def ordenamiento_por_insercion(lista):

    for indice in range(1, len(lista)):
        valor_actual = lista[indice]
        posicion_actual = indice

        while posicion_actual > 0 and lista[posicion_actual - 1] > valor_actual:
            lista[posicion_actual] = lista[posicion_actual - 1]
            posicion_actual -= 1

        lista[posicion_actual] = valor_actual
```

```python
import random

def ordenamiento_por_incercion(tamaño_de_lista):
    lista = [random.randint(0,20) for i in range(0, tamaño_de_lista)]
    for i in range(len(lista)):
        for j in range(i,0,-1):
            if(lista[j-1] > lista[j]):
                aux=lista[j];
                lista[j]=lista[j-1];
                lista[j-1]=aux;
    print(lista)
    
ordenamiento_por_incercion(10)         
```



### Ordenamiento por mezcla.

​	Funciona dividiendo el array en dos mitades repetidamente hasta que obtenemos el array dividido en elementos individuales. Un elemento individual es un array ordenado en sí mismo. El ordenamiento por mezcla combina repetidamente estas pequeñas matrices ordenadas para producir submatrices ordenadas más grandes hasta que obtenemos un array final ordenado. 

​	El algoritmo toma dos variables, _inicio_ y _final_, y almacena el índice del elemento inicial y del elemento final. Luego encuentra el punto medio del array para dividirlo en dos mitades y repite el procedimiento con las sublistas resultantes utilizando la recursividad hasta que estas solo contengan un dato.

​	Luego comenzamos a llamar a la función `merge()` para construir nuestro array ordenado en el que vamos comparando cada lista generada entre ellas he insertándolas

````python
import random

def ordenamiento_por_mezcla(lista):
    if len(lista) > 1:
        medio = len(lista) // 2
        izquierda = lista[:medio]
        derecha = lista[medio:]
        print(izquierda, '*' * 5, derecha)

        # llamada recursiva en cada mitad
        ordenamiento_por_mezcla(izquierda)
        ordenamiento_por_mezcla(derecha)

        # Iteradores para recorrer las dos sublistas
        i = 0
        j = 0
        # Iterador para la lista principal
        k = 0

        while i < len(izquierda) and j < len(derecha):
            if izquierda[i] < derecha[j]:
                lista[k] = izquierda[i]
                i += 1
            else:
                lista[k] = derecha[j]
                j += 1

            k += 1

        while i < len(izquierda):
            lista[k] = izquierda[i]
            i += 1
            k +=1

        while j < len(derecha):
            lista[k] = derecha[j]
            j += 1
            k += 1
        
        print(f'izquierda {izquierda}, derecha {derecha}')
        print(lista)
        print('-' * 50)

    return lista


if __name__ == '__main__':
    tamano_de_lista = int(input('De que tamano sera la lista? '))

    lista = [random.randint(0, 100) for i in range(tamano_de_lista)]
    print(lista)
    print('-' * 20)

    lista_ordenada = ordenamiento_por_mezcla(lista)
    print(lista_ordenada)
````



## Diagramas de modelado.

### UMT - Unified Modeling Language.

​	El lenguaje unificado de modelado es el lenguaje de modelado de sistemas de software más conocido y utilizado en la actualidad. Es un lenguaje grafico para visualizar, especificar, construir y documentar un sistema. UML ofrece un estándar para describir un “plano” del sistema (modelo), incluyendo aspectos conceptuales tales como procesos, funciones del sistema, y aspectos concretos como expresiones de lenguajes, esquemas de bases de datos y compuestos reciclados.

​	Se utiliza para definir un sistema, para detallar los artefactos en el sistema y para documentar y construir. En otras palabras, es el lenguaje en el que está descrito el modelo.

#### Clases.

​	Las clases se representan así:

![clase.png](https://static.platzi.com/media/user_upload/clase-1897e6cf-84b3-4432-926b-aff4fc4db122.jpg)

​	En la parte superior se colocan los atributos o propiedades, y debajo las operaciones de la clase. El simbolo con el que inicia cada línea representa la visibilidad del atributo o método, según una serie de niveles que serían:

- __-__ private.
- __+__ public.
- __#__ protected.
- __~__ default.



​	Una de las formas de representar las relaciones que tendrá un elemento con otro es a través de las flechas, las cuales son:

#### Asociación.

![associacion.png](https://static.platzi.com/media/user_upload/associacion-d2e1b691-b6e9-4854-85e2-d3ffdf0a9049.jpg)

​	Esta flecha significa que el elemento contiene al otro en su definición, y la flecha apuntará hacia la dependencia.

![uml-relacion-asociacion.jpg](https://static.platzi.com/media/user_upload/uml-relacion-asociacion-99b916c6-1f80-4b61-889a-ebf6e74f4f23.jpg)

​	En este caso la ClaseA está asociada y depende de ClaseB.



#### Herencia.

![herencia.png](https://static.platzi.com/media/user_upload/herencia-2eb98d5e-bcad-4162-b236-aa87eba20e76.jpg)

​	La dirección de la flecha irá desde el hijo hasta el padre.

![herencia-clases.png](https://static.platzi.com/media/user_upload/herencia-clases-53cb3117-def7-433f-adc5-4ad183d6b5e7.jpg)

​	En este caso la ClaseB hereda de la ClaseA.



#### Agregación.

![agregacion.png](https://static.platzi.com/media/user_upload/agregacion-6489d946-cc06-4e3c-a976-f6435531b4f2.jpg)

​	Esta relación es parecida a la asociación en el sentido de que un elemento depende de otro, pero en este caso será un elemento dependiendo de múltiples elementos, es decir una relación de uno a muchos.

![uml-relacion-agregacion.jpg](https://static.platzi.com/media/user_upload/uml-relacion-agregacion-adb20be8-d6c2-41d1-b002-2cfa37639240.jpg)

​	En este caso ClaseA contiene carios elementos de ClaseB. Estos últimos son comúnmente representados con listas o colecciones de datos.



#### Composición.

![composicion.png](https://static.platzi.com/media/user_upload/composicion-1da1dd19-6925-42d9-9727-7fd8cb031b0c.jpg)

Este es similar al anterior solo que su relación es totalmente compenetrada de tal modo que conceptualmente una de estas clases no podría vivir si no existiera la otra.

![uml-relacion-composicion.jpg](https://static.platzi.com/media/user_upload/uml-relacion-composicion-2d4cb1fa-5422-44e3-849b-3a3e2d276733.jpg)

---
