## ¿Qué es?
El DOM (Document Object Model O Modelo de Objeto de Documento) se refiere a un interfaz de programación para HTML y XML, sin embargo esto nos puede facilitar una representación estructurada del documento por lo que esto los programas pueden acceder, con el fin de modificar, tanto estructura, su contenido etc.

De lo cual el DOM nos da un representación del documento de nodos y objetos estructurados que tienen propiedades  y metodos.

![[Pasted image 20230925113545.png]]

## Funciones para modificar el DOM
Acceder a elementos
Acceder a elementos Padre/Hijo
Crear elementos
Añadir a DOM elementos 
Añadir / Eliminar clases
Obtener atributos
Escribir texto dentro de un elemento
Modificar atributos


## Funciones para modificar en jquery

#### Acceder a elementos 

- *getElementById()*

El primer método, `.getElementById(id)` busca un elemento HTML con el `id` especificado. En principio, un documento HTML bien construído **no debería** tener más de un elemento con el mismo `id`, por lo tanto, este método devolverá siempre un solo elemento:
![[Pasted image 20230925115918.png]]


- *querySelector()*
El método `.querySelector()` devuelve el primer elemento que encuentra que encaja con el selector CSS suministrado por parámetro. Siempre devuelve un solo elemento y en caso de no coincidir con ninguno, devuelve :

![[Pasted image 20230925120553.png]]

#### Acceder a elementos Padre / Hijo

El padre de un elemento es aquel que se encuentra por encima y que le engloba.
Se utiliza el método **parent()**
![[Pasted image 20230925121809.png]]

Los hijos son todos los elementos que estan por debajo de otro en el DOM, en otras palabras, todo lo que hay dentro de una etiqueta.

Se utiliza el método **children()** y se puede filtrar por el tipo de elemento hijo que se desea.

![[Pasted image 20230925121901.png]]

#### Crear elementos 
Hay cuatro métodos en jQuery para crear elementos HTML:

1. `append()`: este método agregará el elemento al final de los elementos seleccionados.
2. `prepend()`: este método agregará el elemento al principio de los elementos seleccionados.
3. `after()`: este método agregará el elemento después de los elementos seleccionados.
4. `before()` - Este método agregará el elemento antes de los elementos seleccionados.


#### Añadir a DOM elementos 
- *jQuery append()*

Tiene como funcionalidad añadir o **insertar contenido al final del elemento seleccionado**. El caso opuesto lo tenemos con [prepend()](https://www.anerbarrena.com/jquery-prepend-5351/) que añade contenido al comienzo.
Su sintaxis es la siguiente:
![[Pasted image 20230925123141.png]]

- *jQuery prepend()*

Tiene como funcionalidad añadir o **insertar contenido al comienzo del elemento seleccionado**. El caso opuesto lo tenemos con [append()](https://www.anerbarrena.com/jquery-append-5300/) que añade contenido al final.
Su sintaxis es la siguiente:
![[Pasted image 20230925123319.png]]

- *jQuery after()*

Tiene como funcionalidad **añadir elementos después de otro elemento indicado** dentro del DOM de una página web.
![[Pasted image 20230925123429.png]]

#### Añadir / Eliminar clases

Con **jQuery addClass()** y **removeClass()** podemos añadir o eliminar clases a los elementos del DOM de una página web. Hasta ahora habíamos visto una serie de efectos con los que eliminábamos, vaciábamos, añadíamos HTML o modificábamos los estilos CSS.

- *Sintaxis de jQuery addClass()*
La sintaxis de esta función de jQuery para añadir clases.
![[Pasted image 20230925123838.png]]
	- **elemento (obligatorio)**: Objeto al cual queremos añadir una o varias clases.
	- **nombreClase (obligatorio)**: Nombre de la clase existente que queremos asignar.
	- **función (opcional)**: Al usar la [Función callback](https://www.anerbarrena.com/jquery-callback-5110/) por defecto nos devuelve estos valores: **index** con el número de posición del elemento en el DOM, y **oldclass** con la clase actual del elemento.
- *Sintaxis de jQuery removeClass()*

La sintaxis para eliminar clases de los elementos es la siguiente:
![[Pasted image 20230925124009.png]]

- **elemento (obligatorio)**: Objeto del cual queremos eliminar una o varias clases.
- **nombreClase (obligatorio)**: Nombre de la clase existente que queremos asignar.
- **función (opcional)**: Al usar la función por defecto nos devuelve estos valores de las clases a eliminar: **index** con el número de posición del elemento en el DOM, y **claseactual** con la clase actual del elemento.

#### Obtener atributos
- Sintaxis de jQuery attr()
Cuando **attr()** se usa para **obtener el valor de un atributo** devuelve el valor del primer elemento encontrado.
![[Pasted image 20230925124406.png]]}
- **selector (Obligatorio)**: Elemento que queremos examinar a nivel de atributos.
- **atributo (Obligatorio)**: Atributo del cual queremos obtener su valor.

#### Escribir texto dentro de un elemento
De la función **jQuery text()**, de esta manera podemos obtener o asignar el texto que queramos a los diferentes elementos del DOM.
![[Pasted image 20230925125103.png]]

- **selector (Obligatorio)**: Es el nodo del que queremos obtener el texto. Afecta también a la profundidad del nodo, es decir, que saca también el texto de los nodos hijo.

Y ahora explico la sintaxis para asignar el texto:

- **selector (Obligatorio)**: Es el nodo al que queremos asignar el texto.
- **texto (Obligatorio)**: Texto que queremos insertar en el nodo.

#### Modificar atributos

 - *Ejemplo de jQuery attr() para modificar el valor de un atributo*
 
Vamos con el segundo ejemplo de attr para modificar el valor de un atributo:

![[Pasted image 20230925130335.png]]
- Detectamos el [click](https://www.anerbarrena.com/jquery-click-1931/) del botón con id = ‘boton’.
- Modificamos el **valor del atributo** ‘value’ del botón por «OTRO TEXTO».

