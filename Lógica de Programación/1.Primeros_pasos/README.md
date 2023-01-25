        HTML

Todo navegador (o browser, en inglés) logra leer y entender HTML que es el lenguaje utilizado para la presentación de datos e informaciones. Es un lenguaje estatico, sirve para formatación de la pagina web.

Su sigla significa Hyper Text Markup Language, o sea es un lenguaje de marcación de texto caracterizada por el uso de TAGs (etiquetas).

        TAGS

T-A-G en inglés, que son las etiquetas de HTML. Las TAGs (etiquetas) indican instrucciones especiales para ser ejecutadas por el navegador.

La etiqueta <h1> es usada para exhibir el primer título de una página. Veamos un ejemplo:

                    <h1>Bienvenido</h1>

El contenido de la TAG h1 "Bienvenido" será exhibido en destaque en la página. Vea que el texto está entre la etiqueta de apertura <h1> y la de cierre </h1>, por eso podemos decir que "Bienvenido" es el contenido de la etiqueta <h1>.

Visite <a href="http://www.aluracursos.com"> Alura Latam</a>

La etiqueta posee como contenido la página de Alura Latam, y el contenido puede ser encontrado haciendo clic para que el navegador cargue la página informada en el atributo href de la etiqueta.

        JavaScript en HTML 

Cuando escribimos un código en JavaScript, el primer paso es dar una pista al navegador para que entienda que el trecho de código a ser leído se trata de JavaScript. Eso lo hacemos a través de:

    De la etiqueta <script>


Todo código escrito en JavaScript debe estar dentro de la etiqueta <script>. Veamos un ejemplo que exhibe un alert en la pantalla:

<meta charset="UTF-8">
<h1>Usando JavaScript por primera vez</h1>
<script>
    alert("Este es un pop-up en JavaScript");
</script>
Esto está fuera de JavaScript... esto en HTML


Piensa que todo lo que está entre <script>…</script>, está en el mundo JavaScript. Siendo así, el navegador interpretará ese trecho como JavaScript. Todo aquello que está escrito fuera de <script>…</script>, es considerado mundo HTML y será interpretado como HTML.

                        document.write() 

Para usar el código HTML dentro de JavaScript, puedo definir el texto que quiero que aparezca en mi programa, lo que hace que mi código de JavaScript sea más dinamico.La ventaja es que con el document.write podemos pasar al resultado de un cálculo y, entre otras cosas, de manera dinámica ya que el mundo HTML no es capaz de realizar operaciones matemáticas.

<meta charset="UTF-8">
<script>
    document.write("18" + "2"); //182
    document.write("18" + 2); //182
    document.write(18 + 2); //20
    document.write(12 + " años"); // 12 años
    document.write("Media calculada " + 20); // Media calculada
     document.write(Mi edad es + 12); // error pues todo debe de ir entre '' comillas
</script>

Si observas, estamos usando el operador de suma envolviendo dos textos (dos strings). En este caso, JavaScript irá a concatenar, o sea, juntar el texto antes del + con el texto que viene después. Por eso el resultado final es “182” que será pasado para document.write como parámetro. Es bueno recordar que JavaScript primero evalúa la operación (suma) antes de pasar para los () de la instrucción.



Etiquetas 
 Existe una convención que establece el uso de etiquetas en letras minúsculas en HTML, sin embargo, si usamos letras mayúsculas, para el navegador no habrá diferencia alguna.

- br, que viene del inglés break, salto de línea.
- h1 que viene del inglés head, de destaque o título de mi página.
- a, que viene de ancora, enlace de ancla, vinculo y sirve para crear links.
- script, todo código escrito en JavaScript debe estar dentro de la etiqueta.


Meta Charset 
Los navegadores tenemos que definir el tipo de conjunto de datos que estamos usando, pues en ocasiones no logran reconocer el caracteres especiales, para ello la codificación que se usa es UTF8.

<meta charset="UTF-8"> 


Alert 

Alert es una función, que esta esperando un parámetro "puede ser un mensaje". 

- FUNCIONES

A) Necesitan ser declaradas usando la palabra especial function.

B) El uso de los paréntesis () es obligatorio y una o más instrucciones pueden estar dentro de un bloque.

C) Toda las funciones tienen un bloque, que se caracteriza por el uso de { y }.

D) Una o más instrucciones pueden quedar dentro del bloque de una función.

F) Recibe parámetros y dentro de la función Se pasa este parámetro para pasar usarlo.

- prompt() 

Es un método del objeto Window de JavaScript que se usa para mostrar un cuadro de diálogo con un mensaje que solicita al usuario que ingrese algún texto o información