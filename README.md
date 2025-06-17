# Introduction-Javascript

# Introduction-Javascript

Parte 1: Explorando JavaScript

1.1 Diferencias entre JavaScript, HTML y CSS?
 Una buena respuesta a esta diferencenciacion es que imagínate que estás armando tu perfil en una red social.
 * HTML es como el esqueleto, la estructura básica de tu perfil. Define donde va la foto, donde el nombre, donde los posts, todo eso. Es puro texto que le dice al navegador "aquí hay un botón", "aquí va un párrafo". Sin HTML, no hay nada, es solo una pantalla en blanco.
 * CSS es como la ropa y el maquillaje de tu perfil. Le da estilo: si la foto es redonda o cuadrada, qué color de fondo tiene tu nombre, el tipo de letra, si los botones tienen sombras. Hace que se vea bien y no como un archivo de texto viejo.
 * JavaScript es como la parte interactiva, la interactividad viva de tu perfil. Es lo que hace que cuando le des "me gusta" a una foto, el contador de likes suba sin recargar la página. O cuando escribes un comentario, se publique al instante. También si hay un carrusel de fotos, JavaScript es el que hace que las fotos se muevan. En resumen, HTML es lo que es, CSS es cómo se ve, y JavaScript es lo que hace.
   
1.2 Tres características principales de JavaScript
 * Es el cerebro de la web interactiva: prácticamente todo lo que ves que se mueve o responde a tus acciones en una página web lo hace gracias a JavaScript. Desde formularios que validan si pusiste bien tu correo hasta jueguitos en el navegador.
 * Corre en el navegador (y en otros lados): Principalmente, JavaScript vive en tu navegador ( Chrome, Firefox, Edge). Pero con algo llamado Node.js, ahora también puede usarse para construir servidores y apps fuera del navegador.
 * Es fácil de empezar pero tiene mucho fondo: Puedes hacer cosas sencillas con pocas líneas de código, lo que está cool para empezar. Pero si te pones más serio, hay un montón de cosas avanzadas y frameworks (como React o Angular) para hacer apps más complejas.
1.3 ¿Qué significa que JavaScript sea "interpretado" y "basado en eventos"?
 * "Interpretado": Imagina que tienes un chef que lee las instrucciones de una receta y las ejecuta en el momento. No necesita tener toda la receta lista y cocinada de antemano para empezar. Así es JavaScript: el navegador lee el código linea por linea y lo ejecuta sobre la marcha. No tiene que "compilarse" (traducirse todo el código a un idioma que la máquina entienda antes de ejecutarlo) como otros lenguajes.
 * "Basado en eventos": Piensa en una fiesta. No sabes cuándo la gente va a llegar, cuándo van a pedir una canción, o cuándo se van a ir. Pero tienes un plan para cada "evento": si llega alguien, lo saludas; si piden una canción, la pones. JavaScript funciona asi: está siempre atento a "eventos" (un click en un botón, alguien tecleando algo, la pagina cargando) y cuando uno de esos eventos ocurre, ejecuta el pedazo de código que le dijiste que ejecutara para ese evento. Es como "si pasa esto, haz aquello".
Parte 2: Variables y Tipos de Datos
2.1 Declarando una variable y saludando
let nombre = "Juan"; // Aquí se crea una variable con el nombre de alguien
console.log("Hola, " + nombre);

2.2 Creando variables de diferentes tipos

* let cantidadProductos = 15; // Un número entero
* let precioUnitario = 9.99; // Un número decimal
* let mensajeBienvenida = "¡Bienvenido a nuestra tienda!"; // Una cadena de texto

console.log(cantidadProductos);
console.log(precioUnitario);
console.log(mensajeBienvenida);

2.3 Declarando una constante PI
const PI = 3.1416;
console.log(PI);

// Intenta cambiar su valor (esto va a dar un error)
// PI = 3.0; // Si descomentas esta línea, verás un error en la consola

Si intentas cambiar el valor de PI después de declararla, la consola te tirará un error diciendo algo como "Assignment to constant variable" (asignación a una variable constante). Es como si le pusieras un candado al valor, ¡no se puede mover!

2.4 Declarando una variable sin valor
let miVariableSinValor;
console.log(miVariableSinValor);

Cuando imprimes miVariableSinValor en la consola, verás undefined. Esto significa que la variable existe, pero aún no le has puesto nada adentro. Es como una caja vacía.

2.5 Variable con null y booleana

let valorNulo = null; // Representa la ausencia intencional de un valor
let estaActivo = true; // Un valor booleano (verdadero o falso)

console.log(valorNulo);
console.log(estaActivo);

 * null es como decir "aquí no hay nada, y lo sé".
 * true o false son los valores booleanos, perfectos para preguntas de sí o no.
  
Parte 3: Entrada y Salida de Datos

3.1 Pidiendo la edad con prompt()
// La forma en que yo lo haría:
let edadTexto = prompt("¿Cuántos años tienes?");
let edadNumero = parseInt(edadTexto); // Esto convierte el texto a un número por si lo necesito luego
console.log("Tienes " + edadNumero + " años.");

Ahí le pides al usuario que escriba su edad. El prompt() es esa ventanita que sale y te pide algo. Lo que escriba el usuario se guarda en la variable edadTexto. Luego, lo muestro en la consola.

3.2 Mensaje de bienvenida con alert()
alert("¡Qué bueno que llegaste! ¡Bienvenido!");

El alert() es como cuando te mandan una notificación pop-up en el celular, ¡aparece una ventanita con el mensaje!

3.3 Preguntando al usuario con confirm()

let quiereContinuar = confirm("¿Deseas continuar con esto?");
console.log(quiereContinuar);

El confirm() es como si te preguntara: "Oye, ¿vas a ir a la fiesta o no?" Y te da dos botones: "Aceptar" (que sería true) o "Cancelar" (que sería false). Lo que elijas, ese valor se guarda en la variable quiereContinuar y luego lo ves en la consola. 

Parte 4: Operadores

4.1 Varibles numéricas

let num1 = 12;
let num2 = 20;

let sum = num1 + num2;
let resta = num1 - num2;
let multi = num1 * num2;
let divi= num1 / num2;
let modul = num % num2;

4.2 Contatenación de cadenas.

let nombre = "Cristian";
let apellido = "Agudelo";

let concatenación = nombre + " " + apellido;
console.log(concatenación)

4.3 Comparaciones

console.log("5 == \"5\":", 5 == "5"); // true (comparación de valor, coacción de tipo)

console.log("5 === \"5\":", 5 === "5");     // false (comparación de valor y tipo)

console.log("true && false:", true && false); // false (AND lógico)

console.log("false || true:", false || true); // true (OR lógico)

console.log("!true:", !true);   // false (NOT lógico)

Parte 5 

5.1 Programa condicionales

let num = prompt("Ingresa tu numero aquí!");
numerousuario = parsefloat(num);

if (isNaN(numeroUsuario)) {
    console.log("Entrada inválida. Por favor, ingresa un número.");
} else if (numeroUsuario > 10) {
    console.log(El número ${numeroUsuario} es mayor que 10.);
} else if (numeroUsuario < 10) {
    console.log(El número ${numeroUsuario} es menor que 10.);
} else {
    console.log(El número ${numeroUsuario} es igual a 10.);
}

5.2 Usuario Admin

if (nombreUsuario === "Admin") {
    console.log("¡Bienvenido, Administrador!");
} else {
    console.log(Hola, ${nombreUsuario}. ¡Bienvenido!);
}

5.3

let mensajeParImpar = (numParaParImpar % 2 === 0) ? "es par" : "es impar";
console.log(El número ${numParaParImpar} ${mensajeParImpar}.);

Parte 6 

6.1
// Un mensaje informativo (console.info)
console.info("Este es un mensaje informativo.");

// Un mensaje de advertencia (console.warn)
console.warn("¡Advertencia! Algo inesperado ha ocurrido.");

// Un mensaje de error (console.error)
console.error("Error: Ha ocurrido un problema crítico.");

// Un grupo de mensajes (console.group y console.groupEnd)
console.group("Detalles del Usuario");
console.log("Nombre: Juan");
console.log("Edad: 30");
console.log("Ciudad: Madrid");
console.groupEnd();

// El tiempo que tarda un bloque de código en ejecutarse (console.time y console.timeEnd)
console.time("Tiempo de ejecución del bucle");
for (let i = 0; i < 100000; i++) 
console.timeEnd("Tiempo de ejecución del bucle");

Parte 7 
/*
Este es un comentario de varias líneas.
Se utiliza para explicar bloques de código grandes.
*/

// Declaración de una variable para almacenar un saludo.
let saludo = "Hola, "; // Este es un comentario de una línea que explica la variable 'saludo'.
let nombre = "programador"; // Otra variable para el nombre.

// Concatenación de las cadenas para formar un mensaje completo.
let mensajeCompleto = saludo + nombre + "!";

/*
La siguiente línea de código imprime el mensaje completo
en la consola del navegador.
Es util para depurar y ver los resultados intermedios.
*/
console.log(mensajeCompleto); // Imprime "Hola, programador!"

