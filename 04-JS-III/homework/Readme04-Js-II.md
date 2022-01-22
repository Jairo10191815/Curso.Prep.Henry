#ARRAYS

La siguiente explicación no solo tratará de cumplir con el objetivo propuesto en la consigna, sino que, además, brindará una comprensión simple y concreta sobre el tema propuesto en esta ocasión.

Pero, antes de continuar, es necesario que refresquemos algunos contenidos, que serán muy importantes a la hora de comprender: qué son los arrays...

*¿Qué es una variable?

Es una expresión a la que, luego de colocarle un nombre (para poder identificarla), se le asigna datos de un solo tipo.

Ejemplo:

var ejemplo ="Este es un ejemplo de variable"; // Este es un ejemplo

Como podemos ver, solo hemos asignado un dato de tipo string... pero, ¿que pasa si necesitamos colocar datos variados en una única variable?... pues, hoy conoceras algo fascinante:

*Arrays (que en español se traduce como arreglos o matrices):

En sí, es un tipo de variable que se caracteriza por permitir asignarle datos de distintos tipos, funciones, otro array, etc. Es decir, es como una caja sin fondo (ya que podemos agregar la cantidad de datos que deseemos), en la que podemos contener cualquier elemento que QUERAMOS... Muy bien, muy bien... pero, ¿cómo lo escribimos?

Ejemplo: 

var ejemplo = ["casa", 276, 1 > 2 && 3 < 4, function LoQueQuieras (str) {return str + " Este dato ingresado permite realizar una función";}, const otroArray["Dentro de un Array", 27], 2 + 4];

En JavaScript para construir una "matriz" tenemos que declarar una variable y establecerla en [], donde podemos anexar al contenedor, separados por coma, tantas cadenas, números, o booleanos como queramos y acceder a ellos cuando lo deseemos.

Basándonos en el anterior ejemplo, en el que se llega a apreciar la capacidad de un array, podemos aplicarle métodos incorporados útiles, como:

- ejemplo.length

Que nos devuelve el número de elementos en una matriz.

- ejemplo.push("DatoDeCualquierTipo");

Que agrega un elemento al final de la matriz, incrementando su longitud en 1 (uno).

- ejemplo.pop();

Que elimina el último elemento de la matriz, disminuyendo la longitud en 1 (uno).

- ejemplo.unshift("DatoDeCualquierTipo");

Que agrega un elemento al inicio de la matriz, incrementando su longitud en 1 (uno).

- ejemplo.shift();

Que elimina el primer elemento de la matriz.

______________________________________________

También podemos acceder a un elemento de la matriz en cualquier momento, solo necesitamos llamar al dato por su posición en la matriz, los cuales reciben una ubicación numérica que siempre comienza en 0 (cero). Es decir que, el primer elemento está en la posición 0 (cero), el segundo en la 1 (uno), el tercero en la 2 (dos), y así sucesivamente.

Además, podemos reasignar elementos en un array, cuantas veces queramos.

Ejemplo:

var ejemplo = ["casa", 276, 1 > 2 && 3 < 4, function LoQueQuieras (str) {return str + " Este dato ingresado permite realizar una función";}, const otroArray["Dentro de un Array", 27], 2 + 4];

ejemplo[1] = "Reasignación"; // ["casa", "Reasignación", 1 > 2 && 3 < 4, function LoQueQuieras (str) {return str + " Este dato ingresado permite realizar una función";}, const otroArray["Dentro de un Array", 27], 2 + 4]

O también...

ejemplo= [2, "datos"]; // [2, "datos"]
