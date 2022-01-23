La realizaación de esta actividad cumple con el objetivo planteado en la misma y, además, promueve un aprendizaje dinámico al relacionar la programación con otros campos de estudio que nos rodean en nuestro día a día. Por lo que, lo escrito en las siguientes líneas serán de índole interdisciplinaria.

#OBJETOS

Al igual que los arrays, los objetos pueden contener una cantidad ilimitada de datos y de cualquier tipo, con la diferancia de que, toda la información que introduzcamos en ellos, se refiere a una sola cosa y que, en lugar de usar corchetes, se utilizan llaves.

Ejemplo:

var Jairo = { 
				Nombre: 'Jairo',
				Apellido: 'Holgado',
				Edad: 19,
				Aplica en Henry: True
};

Como pudimos observar, en el anterior ejemplo, se parece a describir a un elemento, similar a cuando en Lengua y Literatura debíamos recolectar o reunir los adjetivos de algo o alguien para luego plasmarlos de forma literal en narraciones para darles vida a los correspondientes personajes que creábamos.  Solo que, en programación, a esas cualidades las denominamos como PROPIEDADES.

#PROPIEDADES

Para ponernos en perspectiva y sin la necesidad de caer en complejos dilemas, una PROPIEDAD (en programación) se define como un sistema de pares que utiliza una CLAVE y un VALOR= 

KEY: VALUE, (que en español se traduce como Clave: Valor).

Donde, "Key" es el identificador y, "value" es el valor que queremos guardar en la clave pertinente.

Como si quisiéramos describir un personaje, para lo que primero nos basamos en un parámetro y luego establecemos la cifra que le pertenece.

Ejemplo:

var personaje = {
				Nombre: 'Jairo',
				Edad: 19,
				Altura: 1.87
				
};

Como se dijo anteriormente, los objetos pueden contener una gran cantidad de propiedades (pares Key: value), separados por una coma. Sin embargo, en un objeto todos los pares clave: valor deben tener un identificador ÚNICO E IRREPETIBLE, mientras que, los valores sí pueden repetirse, los cuales pueden ser de cualquier tipo de dato. 

#NOTACIÓN DE PUNTOS VS NOTACIÓN DE CORCHETES

Antes de continuar, es importante que sepas comprender que nosotros podemos acceder a los objetos y conocer el valor que está dentro de las claves, como así también modificarlo o agregar uno nuevo, por medio de dos opciones:

*Utilizando punto seguido=

Objeto.clave // valor

Ejemplo: 

Supongamos que tengamos el siguiente objeto...

var personaje = {
				Nombre: 'Jairo',
				Edad: 19,
				Altura: 1.87
				
};

Para acceder a alguna de sus propiedades, haríamos lo siguiente: 

- personaje.Nombre // 'Jairo'
- personaje.Edad // 19
- personaje.Altura // 1.87 

Para modificar a alguna de sus propiedades:

- personaje.Nombre = 'David';

Para anexar una nueva propiedad:

- personaje.Apellido = 'Holgado';

Para eliminar una propiedad:

- delete personaje.Altura;

*Utilizando corchetes:

Objeto['propiedad'] // valor

Ejemplo:

Supongamos que tengamos el siguiente objeto...

var guitarra = {
				Marca: 'Alpujarra', 
				Madera: 'Jacarandá o sicómoro laminado',
				Tienealma: True,
				CantidadDeCuerdas: 6,
				Ecualizador: 'Fishman'
}

Para acceder a alguna de sus propiedades, haríamos lo siguiente: 

- guitarra['Marca'] // 'Alpujarra'
- guitarra['Tienealma'] // True
- guitarra['Ecualizador'] // 'Fishman'

Para modificar a alguna de sus propiedades:

- guitarra['Madera'] = 'Ébano y nogal';

Para anexar una nueva propiedad:

- guitarra['TieneBoca'] = True;

Para eliminar una propiedad:

- delete guitarra['Tienealmma'];


Para concluir con este apartado, en los anteriores ejemplos observábamos las diferencias en la utilización de la Notación por puntos y con corchetes. Cualquiera de las dos es funcional. Con el punto es llamar a la propiedad, como cuando lo hacíamos con .length, solo que ahora es mediante el uso de la Clave del sistema de pares Key: Value. Y, en notación con corchetes es parecido a cuando citábamos a los datos de un array, con la diferencia de que, ahora nuestro índice no es numérico, sino que lo hemos creado nosotros en el momento de realizar nuestra propiedad a la que podemos acceder colocándola entre comillas, de esa manera nos retornará el valor que deseamos conocer.

#MÉTODOS

¿Recuerdas que mencionamos que en un objeto puedes colocar datos de cualquier tipo? Pues... cuando colocamos una función como valor de una clave, se denomina como MÉTODO.

Ejemplo:

var nuevoEjemplo = {
				estoEsUnMétodo: function (str) { return "Esto es un Método " + str;
				},
};

Al cual podemos invocarlo con notación de puntos o con corchetes, con la peculiaridad de que, al final le anexaremos paréntesis, tanto para indicar que se está tratando de un método, como así también para incluir la información necesaria en ellos mismos, si la función asi lo requiere.

Ejemplo: 

Supongamos que creamos el siguiente objeto, en el cual contendremos nuestro método= 

var objeto = {
				método: function (str) {
								return str + " es el dato anexado";
				},
};

Para acceder al método hacemos lo siguiente:

objeto.método ('Sistema de puntos') // 'Sistema de puntos es el dato anexado'

objeto['método'] ('Sistema de corchetes') // 'Sistema de corchetes es el dato anexado'

#BUCLES FOR...IN

En algunas ocasiones, no sabemos qué valores tenemos dentro de las claves de las propiedades y, para tratar de hacerlo de una manera eficaz, rápida y para tratar de simplificar nuestra tarea, usamos el Bucle "for...in". De tal manera que podamos iterar sobre cada elemento que esté dentro de un objeto. Podemos hacerlo de la siguiente manera...

Ejemplo:

Supongamos que tenemos el siguiente objeto con las correspondientes propiedades=

var ejemploDeObjeto = {
				propiedad0: 'Primer valor',
				propiedad1: 27459,
				propiedad2: True,
				propiedad3: 2 > 4 || 6 < 7,
				propiedad4: 'Último valor'
}

Ahora nuestro bucle "for... in" sería el siguiente= 

for(var i = 0 in ejemploDeObjeto) {
				console.log(ejemploDeObjeto[i]);
				
}
_____________________________________________

De esta manera, podemos realizar cualquier cosa que se nos ocurra, solo hay que ser creativos.
