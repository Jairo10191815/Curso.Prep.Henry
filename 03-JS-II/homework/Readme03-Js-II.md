* Bucle FOR

Esta explicación no solo fue creada para personas de 12 años de edad, sino que también para ofrecer una ruta de comprensión simplificada y, desde un punto de vista más práctico en el sentido de relacionarlo con actividades de nuestra cotidianeidad.

Antes de continuar es necesario que sepamos la diferencia entre una expresión y una declaración... 

UN MOMENTO!!! ¿En qué momento pasamos a esto?

Ok, vayamos un poco más hacia el principio.

Javascript es un lenguaje de programación que utiliza expresiones ("expression", en inglés) y declaraciones ("statements", en inglés) que, si bien trabajan juntos para poder concretar nuestros objetivos en mente, uno de ellos suele tener mayor relevancia que el otro. Esta es la "expression", ya que es la instrucción primaria que realizará una ACCIÓN. Mientras que el segundo, es para ordenarle cómo queremos que lo HAGA, generándose así una pequeña retroalimentación entre ambos, debido a que uno no puede estar sin el otro.

Para ponerte en perspectiva, imaginemos que estás parado en un punto arbitrario de la superficie terrestre... estás tratando de decidir qué acción vas a realizar, de pronto, se te ocurre que quieres correr ¡MUY BIEN! Ya tenemos la acción que deseamos programar. Por lo que, en tu mente te estableces esta idea. Sin embargo, ahora precisamos declarar cómo queremos que sea esa carrera, puede ser rápida, lenta o con una velocidad moderada (intermedia), con pasos largos, cortos, hasta qué distancia, etc. Todos estos últimos factores, en el lenguaje de programación de JavaScript, corresponden a las declaraciones: "statements". Ya aclarado esto, procedamos a nuestro motivo principal de este texto. 

For en Javascript es una expresión ("expression") que permite realizar la acción de un bucle, el cual es un suceso que se repite infinitas veces, a no ser que se le establezca un límite o condición. Por ende, a la hora de programar, estableceremos esta expresión de la siguiente manera: 

for ( CONTENIDO-Parte 1 ) { CONTENIDO-Parte 2 }

#CONTENIDO-Parte 1

Acá, entre paréntesis, escribimos las declaraciones pertinentes ("statements") que, de forma curiosa, a su vez, son expresiones ("expression"), un hecho que se conoce como ANIDAMIENTO DE EXPRESIONES, debido a que, dentro de estos paréntesis colocaremos:

for(var i = 0, i < 100, i++) { }

Para comprender esta serie de condiciones escritas en la anterior línea, imagina que VAR hace referencia a una persona cuyo nombre es "i", quien desea comenzar a correr. Por lo que, ahora debe decidir desde dónde quiere partir, en este caso, desde el punto "0" (cero), aunque puedes asignarle cualquier otra declaración (-1; 2; 3; -76; 81; o una variable que haga referencia a un número, etc.), siempre y cuando sea menor al punto al que quiera llegar, lo cual nos da hincapié para hablar sobre la segunda condición, que establece hasta dónde quieres ir y, en este caso, fue hasta "100" (cien), aún así, ten en cuenta que se puede asignar cualquier otra declaración (100; 461; 98; o una variable que haga referencia a un número, etc.), siempre y cuando sea mayor al punto desde el que parte "i". Ahora, solo falta especificarle que queremos avanzar; para ello, colocamos que "i" desea avanzar: "i++". 

#CONTENIDO-Parte 2

Muy bien, ahora solo tenemos que poner en marcha nuestro bucle for con el siguiente código:

for (var i = 0; i < 100; i++) {
				return i;
}

---------------------------------------------
* Operadores lógicos AND= && / OR= || / NOT= !

Antes de continuar conozcamos un poco de qué se tratan los operadores lógicos. Se definen como elementos que se utilizan para preguntar si dos expresiones son verdaderas, son falsas o si alguna de ellas es verdadera. Están anidados, por lo general, a los flujos de control "if", "else if" y "else", en sus respectivos paréntesis.

Pero... ¿Para qué sirve en sí cada uno de ellos?

#&& ("AND", en inglés. "Y", en español.)

Lo usaremos para cuando querramos preguntar si los dos datos son verdaderos; al hacer esto, nos retornará "true". Mientras que, si uno de ellos es falso o si ambos lo son, nos devolverá "false".

Ejemplo: 

1 > 2 && 7 < 2 // false

1 < 2 && 7 > 2 // true

#|| ("OR", en inglés. "O", en español.)

Lo utilizaremos para cuando querramos preguntar, si los dos datos son verdaderos o si algunos de ellos lo es, nos retornará "true". Mientras que, si ambos son falsos, nos devolverá "false".

Ejemplo:

1 < 2 || 2 < 3 // true

1 < 2 || 2 > 3 // true

1 > 2 || 2 > 3 // false

#! ("NOT", en inglés. "NO", en español.)

Este es un operador bastante curioso, ya que lo usaremos para realizar una pregunta con negación y, nos devolverá "true" o "false" respectivamente de lo que se pregunte.

Ejemplo: 

if (1 !== 2) // true

En este caso, es como decir, uno no es igual a dos, o preguntar: uno no es igual a dos, ¿no cierto? Por lo que no retornará "true".

Ahora veamos otro ejemplo:

if (2 !== 2) // false

Como podemos ver, es como si preguntaramos: dos no es igual a dos, ¿no cierto? Por lo que, en este caso, nos devolverá "false" al ser un dato que carece de veracidad.

Teniendo en cuenta el último ejemplo, este operador lógico puede servirnos también para comparar tipos de datos:

if (2 !== "2") // true

Verdadero debido a que, si bien, ambos hacen referencia a un número, el "2" (dos entre comillas) se considera una string y no como un dígito numérico.
