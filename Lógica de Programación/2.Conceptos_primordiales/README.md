    PROMPT

La función prompt siempre transforma todo lo que digitamos en el formato del texto, o sea, como un string, es una buena práctica siempre convertir el valor digitado para el numero cuando nuestra intención es leer un número.

<meta charset="UTF-8">

<script>
    function saltarLinea() {
        document.write("<br>");
    };
    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    };
    var invitados = parseInt(prompt("Número de invitados"));
    var vips = parseInt(prompt("Número de invitados VIP's"));
    var total = invitados + vips;
    imprimir("El total de invitados es " + total);
</script>

La función prompt retorna lo que digitamos como string y ese retorno es pasado para parseInt. Y es esta función que recibe un string y la convierte en un número. 

    while 
Repetirá TODAS las instrucciones que estén dentro de su bloque { } cuando la condición pasada sea true.El while recibe en sus paréntesis () la expresión a validar. El while estará autorizado para ejecutar la instrucción dentro de su bloque.
Si no se tiene una instrucción de corte, la condición pasada al while dará siempre true y caeremos en una repetición infinita, el famoso loop infinito y muy probable que nuestro navegador se cuelgue.

    for

La declaración for se divide en tres partes que están separadas por un punto y coma. La primera se usa para declarar la variable que usaremos como contador, la segunda para la condición de repetición y la última para el incremento de la variable contador.

for( var contador = 1; contador <= 10; contador = contador + 1 ) {
    alert("Contador actual: " + contador);
}

    Capturar valores del button y el input  

HTML es un lenguaje estático, se muestran tanto el input como el button y no sucede nada. La buena noticia es que en el mundo JavaScript puedes acceder a las etiquetas del mundo HTML. Esto significa que podemos capturar lo que el usuario escribió en el input, incluyendo la programación de una respuesta para cuando hace clic en el button.

<meta charset="UTF-8">

<input />
<button>Haz click aquí</button>

<script>
    var entrada = document.querySelector("input"); 
    var boton = document.querySelector("button");
</script>

A través de document.querySelector que podemos ir hasta el mundo HTML y llevar el elemento al mundo JavaScript para que podamos manipularlo. Pero ten cuidado, el correcto es querySelector con una S mayúscula. Si escribes con una s minúscula, cometerás un error de sintaxis.

document.querySelector recibe un parámetro del nombre de las etiquetas que queremos buscar del mundo HTML. 

.focus() --> 

<meta charset="UTF-8">

<input/>
<button>Mostrar texto escrito</button>

<script>
    var input = document.querySelector("input");//esto es necesario, porque solo así JavaScript podría leer lo que está escrito en <input>

    function mostrarTexto() {
        alert(input.value);//Cuando se llama a la función mostrarTexto, pasará como parámetro de la función alert el valor input.value.
    }

    // La función mostrarTexto, pasará como parámetro de la función alert el valor input.value (queremos que su valor provenga de esa etiqueta input, por eso input.value)

    var button = document.querySelector("button");
    button.onclick = mostrarTexto; // la función mostrarTexto debe llamarse con el botón, cada vez que se hace clic en el botón, se ejecutará mostrarTexto, es como si, por detrás el navegador hiciera mostrarTexto() cada vez que se hace clic en el botón.
</script>

3------------------------
A mejorar la interacción del usuario con uso de botones.
A mejorar la interacción del usuario con uso de cajas de texto.
A mejorar la usabilidad de nuestro programa con focus.

4-------------------------------

Array. Permite que una variable tenga múltiples valores. Cada array se declara entre corchetes, el famoso [ ]. Sin embargo.

Si tenemos una declaración como esta var cosas = [ ], tenemos un array, es decir, una lista vacía sin ningún elemento. Podemos, al declarar un array, agregar elementos. Estos elementos pueden ser de cualquier tipo de dato conocido: var cosas = ["Gisele", 12, true];
El primer elemento de nuestro array es un string, el segundo un número y el último un booleano.

Concepto y dinámica de los arrays.
Usar iteraciones para cargar arrays.
Descubrir el tamaño de los arrays.

5----------------------------------
Todo array tiene una función push que le permite "insertar" elementos en la lista.

Ingresar valores manualmente en los arrays con la función push.
Resolver problemas más complejos usando varios conceptos de programación juntos en un mismo programa (Loops, arrays, condiciones, funciones y fórmulas matemáticas).