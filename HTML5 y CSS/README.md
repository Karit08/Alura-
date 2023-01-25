HTML

HTML significa Hyper Text Markup Language, que en español sería como lenguaje de marcación de textos.

<!DOCTYPE html> 

La etiqueta <!DOCTYPE> sirve para informar al navegador cuál es la versión de HTML que estamos usando, indica al navegador que el documento está basado en el estándar HTML5, definimos cuál versión de HTML estamos utilizando.

<html> 

La etiqueta <html> sirve para informar al navegador dónde comienza y termina nuestro código. Representa la raíz de un documento HTML. Todos los demás elementos de la estructura HTML deben ser recogidos dentro de estas etiquetas, marca el contenido a ser renderizado en el navegador. Dentro de esta etiqueta, podemos definir el lenguaje de la página, a través de la propiedad lang.

La etiqueta <head> sirve para informar al navegador qué informaciones debe leer. 

<meta> 
Pasa la informacion del encoding de nuestra página para el navegador, a través de la etiqueta <meta> y de la propiedad charset.

<meta charset="UTF-8">  
Es necesario informar al navegador que estamos usando un DICCIONARIO específico que contiene caracteres especiales propios de varios idiomas populares en el mundo, siendo nuestra lengua española uno de ellos, ya que contiene acentos y la letra ñ por ejemplo.

<title>Nombre de la pestaña</title>

La etiqueta <body> sirve para informar al navegador cuáles informaciones debe exhibir.
...................................................................................................................
Se acostumbra estructurar el HTML colocando las informaciones que queremos pasar para el navegador en el head y las etiquetas de contenido en el body

<!DOCTYPE html>
<html lang="en">
<head> //(Etiqueta de estructuración) Etiquetas informativas
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body> // (etiqueta de estructuración) Etiqueta de contenido de nuestra pagina 
</body>
</html>
...................................................................................................................

<h1>Definir el título</h1>
<p>Párrafos de un texto</p>
<strong>Dar destaque para algunas informaciones de texto, dejándolas en negrito.</strong>
<em>Dar énfasis para algunas informaciones de texto, dejándolas en itálico.</em>
<body> para el contenido
<head> para información sobre el documento
<div> división dentro del contenido
<a> para enlaces
<strong> para poner el texto en negrita
<br> para saltos de línea
<h1>…<h6> para títulos dentro del contenido
<img> para añadir imágenes al documento
<ol> para listas ordenadas, <ul> para listas desordenadas, <li> para elementos dentro de la lista
<p> para parágrafos
<span> para estilos de una parte del texto
<ul> lista NO ordenada
<ol> lista Ordenada
<li> list items
<div> Divide el contenido en bloques, ayuda en la organización y estructuración de nuestro HTML.
<header> Es una etiqueta de contenido de HTML que nos permite crear el encabezado de nuestra página web
<a> La etiqueta <a> sirve justamente para colocar un link, que nos va a llevar a otro punto en internet.

...................................................................................................................
CSS
text-transform: uppercase; 
    La propiedad text-transform es la responsable de la transformación del texto a mayúscula, cuando usamos el valor uppercase.
text-decoration: none;
    text-decoration sirve para alterar la propiedad de exhibición de un link. Cuando usamos el valor none, quiere decir que no será subrayado.
font-weight: bold
    La propiedad font-weight sirve para alterar el peso de la fuente, inclusive para negrita, con el valor bold.
position: absolute
    Para cambiar la posición del punto inicial donde se encuentra el elemento, yo puedo posicionar mi elemento en cualquier lugar de la página.
text-align: center
    El text-align: center sirve para alinear el contenido de una div, no el elemento en sí.
margin: 0 auto;
    Delegamos para que el navegador haga la cuenta al calcular la largura restante, dividir entre dos y agregar la mitad en cada uno de los lados.


El navegador crea el estilo para todas las etiquetas que considera adecuadas, entonces, necesitamos moverlo para que el estilo que creemos no sea influenciado por el estilo que el navegador agregue. Por ello se usa un archivo reset.css, el cual trae toda la inforación sobre el reset. https://meyerweb.com/eric/tools/css/reset/
        <link rel="stylesheet" href="reset.css">
