Esta explicación plantea como objetivo principal brindar de forma sintética el contenido de los temas pertinentes a esta clase 06-JS-V. De manera tal que su comprensión sea inmediata y eficaz.

Ya aclarado esto... COMENCEMOS!!!

#CONSTRUCTORS (de clases)

En JavaScript, a diferencia de otros lenguajes de programación, no utiliza clases en sí, sino que son funciones usadas como tal, que luego nos sirven para construir objetos relacionados entre sí por sus propiedades (de allí el nombre constructors)... ok, ok... dicho en estas palabras puede sonar un poco simple, por lo que a primera instancia es posible que no nos percatemos de la capacidad que puede llegar a tener una clase...

Supongamos que necesitamos crear una gran cantidad de objetos que mantienen relación alguna entre sí, como los usuarios en un Sitio Web. Si lo hacemos de la forma tradicional, es decir, crear un objeto a la vez, nos enfrentaremos a una pequeña cuestión que nos ocasiona la siguiente dificultad: 

"Al crear un nuevo objeto, en nuestro computador se produce una mayor cantidad de espacio y aumenta la probabilidad de que ocurra un error de tipeo."

Para están los constructores, los cuales se establecen de la siguiente manera:

Ejemplo:

function Usuario(nombre, apellido, edad, correo, dirección) {
				this.nombre = nombre,
				this.apellido = apellido,
				this.edad = edad,
				this.correo = correo,
				this.dirección = dirección
}

var usuario0 = new Usuario ('Jario', 'Holgado', 19, 'holgadojairodavid@gmail.com', 'Juan José Castelli');

Con este ejemplo, podemos comprender cómo se instancia una clase o constructor que siempre se debe nombrar la primera con mayúscula, ya que es una convención que existe entre programadores, para lograr identificarlo de una mejor manera. 

Dentro de la clase vemos a "this", el cual se activiará o comenzará a trabajar cuando creemos un objeto nuevo con la palabra clave "new".

Su aplicación es universal, puede usarse para cualquier tarea que te imagines, como clasificar animales, autos, plantas, fichas de alumnos, censo, etc.

#PROTOTYPE

Ahora, supongamos que hemos creado miles de objetos a partir de una clase. Sin embargo, nos vemos en la necesidad de establecer un método para todos ellos. De la forma tradicional tendríamos que escribir la misma función para cada objeto... aunque podemos ahorrarnos toda esa odisea por medio de la palabra clave "prototype" de la siguiente manera:

Ejemplo:

supongamos que tenemos la siguiente clase=

function Guitarra(marca, maderas, caja, boca, cantidadDeCuerdas) {
				this.marca = marca,
				this.maderas = maderas,
				this.caja = caja,
				this.boca = boca,
				this.cantidadDeCuerdas = cantidadDeCuerdas
}

Guitarra.prototype.ejemplo = function (){
				return "Esta guitarra " + this.marca + "de " + this.cantidadDeCuerdas + " cuerdas, caja " + this.caja + " y de boca tipo " this.boca + " es de fabricación Nacional.";
};

Como podemos ver, tenemos nuestra clase a la cual le anexamos la propiedad "prototype.", seguido del nombre que queremos otorgarle para luego asignarle la función. 

Tal como se logra apreciar en el ejemplo, el método también tiene acceso a "this", pues esto no es tan complejo como parece, solo es importante que comprendas que estará enfocado a cada objeto creado a partir de esta clase y los que se generarán en un futuro, los cuales heredarán además, el nuevo método.

											¿¡NO ES GENIAL!?
											
En lugar de escribir miles de métodos solo tenemos que programar una única fumción.