Diseña gráficos con Canvas

El elemento canvas forma parte de HTML5 y habilita la representación (rendering) dinámica y en scripts de figuras en 2D y 3D de imágenes de mapas de Bits.

    document.querySelector('slector');

Devuelve el primer elemento del documento HTML que coincida con el grupo especificado de selectores.

    <canvas>

<canvas> es un elemento HTML el cual puede ser usado para dibujar gráficos usando scripts (normalmente JavaScript). Este puede, por ejemplo, ser usado para dibujar gráficos, realizar composición de fotos o simples (y no tan simples) animaciones.

    HTMLCanvasElement.getContext()

El método HTMLCanvasElement.getContext() retorna un contexto de dibujo en el lienzo, o null si el identificador del contexto no está soportado.

    canvas.getContext(contextType, contextAttributes);

contextType
Es una DOMString que contiene el identificador del contexto que define el contexto de dibujo asociado a el lienzo. Los posibles valores son:

- "2d", dando lugar a la creación de un objeto CanvasRenderingContext2D que representa un contexto de renderizado de dos dimensiones.

More info [https://developer.mozilla.org/es/docs/Web/API/HTMLCanvasElement/getContext]

    fillStyle = color 

Establece el estilo utilizado al rellenar formas.

    fillRect(x, y, width, height)

Dibuja un rectángulo relleno.
//..............2
A usar funciones para encapsular la creación de figuras.
A utilizar ciclos Loop para repetir actividades cuando creamos nuestras figuras.



        Una forma diferente de probar un if
Tenemos el siguiente código:

<script>
    var aprendi = true;
    if(aprendi == true) {
        alert("El instructor queda muy feliz");
    } else {
        alert("El instructor no va a desistir hasta que el alumno sea una eminencia en programación");
    }
</script>

No hay ninguna novedad ¿cierto?, inclusive ya lidiamos con códigos como ese en el curso anterior. Nuestra condición if prueba si el valor de la variable aprendi es verdadera, y para ello, usamos el operador ==.

Sin embargo, podemos simplificar el código para:

<script>
    var aprendi = true;
    if(aprendi) {
        alert("El instructor queda muy feliz");
    } else {
        alert("El instructor no va a desistir hasta que el alumno sea una eminencia en programación");
    }
</script>

Observa que no usé más el operador ==. Puede que estés intrigado por qué funciona correctamente. Pero si analizamos la sintaxis del condicionante if(), él espera recibir true o false para saber si ejecuta el código dentro del if o dentro del else. Si aprendi ya lo estamos inicializando como true es redundante preguntar dentro del bloque if nuevamente aprendi == true.

Las variables booleanas ya guardan true o false y podemos usarla directamente en el if ahorrando algunos caracteres. Sin embargo, si te sientes más seguro con la forma anterior, puedes continuar usándola sin ningún problema.