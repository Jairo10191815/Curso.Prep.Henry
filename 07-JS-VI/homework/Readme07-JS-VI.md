La siguiente explicación cumple con los objetivos planteados en la consigna, tanto de brindar un contenido concreto y sintético, como así también de permitirme descubrir los agujeros presentes en mi aprendizaje.

#CALLBACKS

En JavaScript, las funciones pueden ser retornadas en cualquier momento (es un funcionamiento tradicional y bastante utilizado). Sin embargo, lo asombroso es que también podemos guardarlas en variables o, incluso, utilizarlas como argumento de otras funciones. Este último hecho se conoce como "Callbacks".

Por lo que, un "Callback" se define como la capacidad de pasar o llamar una función como argumento a otra.

Ejemplo:

// Supongamos que escribimos las siguientes funciones:

function hola(usuario) {
				return 'Hola ' + usuario + '!';
}


function adiós(usuario) {
				return 'Adiós ' + usuario + '!';
}

// Y las llamamos con "cb" (CallBacks) en el argumento de la siguiente función:

function saludar(usuario, cb) {
				return cb(usuario);
}

// Podemos operar con ellas de la siguiente forma:

saludar('Jairo', hola); // 'Hola Jairo!'
saludar('Jairo', adiós); // 'Adiós Jairo!'

Como podemos ver, en este caso, hemos creado tres funciones, las dos primeras son las que utilizaremos como argumento para lograr el "CallBack" y, la última, es la que se usará para cumplir nuestro objetivo, la cual puede recibir cualquier identificador en su argumento en lugar de "cb", solo que, entre programadores existe este convenio de establecerlo de esa manera para lograr reconocerlo mejor, si en alguna ocasión nos toca trabajar en equipo.

Con esto puedes hacer lo que se te ocurra y todo lo que ya sabías sobre las funciones antes de leer este artículo... como así también realizar operaciones matemáticas (sumar, restar, multiplicar, dividir, potencias, etc.)... solo es cuestión pensar diferente.