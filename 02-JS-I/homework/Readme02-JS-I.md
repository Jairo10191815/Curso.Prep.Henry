La siguiente explicación tiene como objetivo principal, brindar al lector un contenido sintético y de simples palabras sobre los conceptos básicos del lenguaje de programación de JavaScript.

Ya aclarado esto, COMENCEMOS!!!

#VARIABLES

Imagina una caja pequeña a la que le otorgas un nombre para más tarde poder localizarla de una manera más sencilla, y en la que puedes guardar un solo objeto. Algo así sucede en JavaScript, donde una variable es una forma de almacenar el valor de algo que será utilizado más tarde, por el que se accede por medio de un nombre que cumple la función de identificador.

Ejemplo:

var ejemploNombre= "Jairo";

var ejemploEdad= 19;

var ejemploApellido= "Holgado";

* Puedes crear cuantas variables quieras, a las que podemos llamarlas en nuestra consola de JavaScript de la siguiente manera:

console.log(ejemploNombre); // 'Jairo'

console.log(ejemploEdad); // 19

console.log(ejemploApellido); // 'Holgado'

Como podemos ver, para instanciar una variable, lo que se debe hacer es utilizar la palabra clave "var", seguida de un espacio para otorgarle el nombre que desees, el cual tiene que ser distinto a las palabras resguardadas por el propio lenguaje de programación, como: "var", "function", "return", "console.log()", "prototype", entre otras; aunque son extrañas las ocasiones en las que de forma involuntaria usemos los anteriores identificadores. Por último, mediante el uso del signo "=" le asignamos el valor que se almacenará en esta variable.

Además, podemos reasignar un valor, es decir, lo que en programación se conoce como pisar una variable.

Ejemplo:

* Usemos una de las variables creadas anteriormente...

var ejemploEdad= 19;

* Podemos hacer lo siguiente...

var ejemploEdad= 36;

console.log(ejemploEdad); // 36

Tras pisar la variable "ejemploEdad", el valor ya no es 19, sino que fue modificado al número 36.

Sin embargo, con la nueva actualización de JavaScript, tenemos otras formas de declarar una variable... estas son:

let segundaForma = "valor";

const tercerForma = "valor";

Pero... ¿en qué situaciones usamos cada uno de estos modos? Con la palabra clave "var", el que vimos primero, es utilizado para declarar una variable que tenga alcance global. En cambio con "let", es para tener un alcance local, como en situaciones de funciones, bucles for que aprenderemos en otros artículos. Mientras que, "const", es para instanciar una variable que no se pueda pisar, es decir, volver a reasignar un valor, por lo que tiene un alcnace global.

#STRIGNS

Es un tipo de dato básico en JavaScript, que se caracteriza por ser bloques de textos que siempre deben ir entre comillas, ya sean simples o dobles.

Ejemplo:

* Supongamos que guardamos una string como valor en una variable...

var ejemploString = "Este bloque de texto se caracteriza por ser perteneciente al tipo de datos Strings";

#FUNCIONES(Argumentos, return)

Hoy en día existen una enorme cantidad de máquinas que se dedican a llevar a cabo determinadas acciones y, si las llevamos a cualquier lugar, mientras se den las condiciones necesarias, podrán ser utilizadas. Como una cocina, una licuadora, una dispenser una pava eléctrica, un lavarropas, etc. Pero... ¿qué tiene que ver todo esto con la programación? Pues así sucede con las funciones en todo lenguaje para programar,. las cuales nos permiten realizar una determinada acción (establecida previamente), llamándolas en alguna parte de la consola. Es más sencillo de lo que puede aparentar. Veámoslo en un ejemplo:

Ejemplo:

function ejemploSumar (a, b) {
				return a + b;
}

* Podemos llamar a la función de la siguiente manera:

ejemploSumar(12, 34); // 46

Como podemos ver, iniciamos con la palabra clave "function"; luego le otorgamos un nombre, en este caso "ejemploSumar" (que más tarde nos servirá para referirnos a ella); entre parántesis colocamos los que se conocen como "ARGUMENTOS", los cuales pueden ser cualquier palabra y la cantidad que querramos, siempre y cuando estén separados por un coma. A continuación, abrimos llaves y nos percatamos de la presencia de "RETURN" (retornar, en español), que cumplirá la acción correspondiente de retornar cuando llamemos a la función en alguna parte de la consola. En este caso fue sumar dos números.

Aunque, una función, en realidad, también puede instanciarse de las siguientes dos maneras, un tanto menos utilizadas:

var segundaFunción = function () {};

var tercerFunción = () => {};

Además, dentro de la función puedes establecer lo que quieras, solo debes dejarte llevar por tu creatividad.

#DECLARACIONES IF

Antes de continuar, es importante que sepas dos cosas:

1- La mayoría de las palabras claves en JavaScript se encuentran en inglés, por lo que, conocer su significado nos será de mucha ayuda a la hora de aprender este lenguaje de programación.

2- En JavaScript, el motor de la computadora lee lo que se instancia como código de forma progresiva, línea por línea. Por lo que, si detecta que solo debe ejecutar hasta cierto punto, lo hará hasta allí. Y, si debe continuar ejecutando en caso de ser necesario, así lo hará también.

En esta ocasión nos encontramos con "if" (que enspañol se traduce como: "si"), una palabra clave que por lo general utilizaremos dentro de las funciones, la cual nos sirve para saber si un valor es "true" (verdadero, een español) o no. Pero... ¿de qué manera?

Para responder esta interrogante, podemos observar y analizar el siguiente ejemplo:

* Supongamos que creamos una función...

function ejemploNuevo (a, b) {
				if(a > b) {
								return true;
				} else {
								return false;
				}
}

* Ahora llamamos a la función con los siguientes argumentos para percatarnos si funciona o no...

ejemploNuevo(37, 58); // false

ejemploNuevo(58, 37); // true

Como podemos ver, hemos instanciado una función ("ejemploNuevo") en la que le pasamos como argumento "a, b", para luego abrir llaves y establecer la "Declaración if", en la que le damos la condición de, si "a > b" (si "a" es mayor a "b"; lo que a su vez nos indica que se tratará de una función dedicada a números.) deberá retornar "true"; de lo contrario, lo cual lo hacemos con la palabra clave "else" (de otro modo, en español), tendrá que devolver "false" (falso, en español). No es difícil de comprender, por lo que, si logramos combinar estos conceptos con la práctica, nos será una herramienta muy útil a la hora de programar.

#VALORES BOOLEANOS (true, false)

En JavaScript, los valores booleanos se utilizan para designar si otro valor es verdadero ("true") o falso ("false").

Ejemplo:

1 > 2 // false

7 > 5 // true

21 / 3 === 7 // true

El concepto puede sonar un poco simple, sin embargo, tiene toda una historia de fondo. Hace algunos varios años atrás, se creó un concepto que alimenta el código binario y el núcleo de las computadoras, en el que hay dos opciones: ACTIVAR o DESACTIVAR; 0 o 1; VERDADERO o FALSO.

Esto también es lo interesante de la programación, es una tecnología que cada tanto evoluciona para adaptarse a los nuevos tiempos, para ser más eficaz y poder brindar un mejor soporte técnico a la hora de programar.