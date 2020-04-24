# -Practica01-Mi-Primer-Sitio-Web

UNIVERSIDAD POLITECNICA SALESIANA. 

OBJETIVO ALCANZADO: Mediante esta práctica he conocido la estructura principal de HTML5  y la implementación de diseños mediante CSS. 

1. Apariencia de la Pagina Home.

La apariencia de la oagina home, basicamente se divide en 6 partes: Cabecera, cuerpo (novedades, testimonios, equipo) y pie de pagina, a continuación las etiquetas mas importantes para desarrollar cada uno de estos puntos. 

Para la cabecera dentro de la qtieuta <header> he puesto el logo principal de la pagina con la etiqueta <img> donde los principales argumentos son: la ruta de la imagen "src", la descripcion de la imagen "alt", anchura de la imagen "width" y la altura de la imagen "height".

Codigo Representativo:

<img src="/Imagenes/netflixPrincipal.png" alt="Todo Sobre Netflix" width="400" height="150">

Para el cuerpo se ha dividido la pantalla en dos, del costado derecho se a colocado informacion relevante de la pagina y en la parte derecha se a colocado una imagen representativa del medio. Para ello se ha definido dos selectores id, con el nombre de contenedor2 y contenedor3 respectivamente. Mientras que el archivo de css se definio el posicionamiento de las cajas y los estilos de las mismas. 

Codigo Representativo:

#contenedor2{
    background: rgb(233, 41, 41);
    width: 45%;
    height: 380px;
    margin-left: -685px;
    margin-top: 1px;
    padding: 100px;
    float: left;
    overflow: hidden;
}

#contenedor3{
    background: rgb(0, 0, 0);
    width: 26%;
    height: 380px;
    margin-left: 904px;
    margin-top: 193px;
    padding: 100px;
    padding-left: 150px;
    position: absolute;
    float: left;
}

Es importante recalcar el desarrollo de los testimonios de los usuario, pues se ha hecho uso de "slider" y "keyframes" que nos permite deslizar de forma automatica los comentarios de los distintos usuarios. 

Codigo Representativo:

@keyframes cambio {
    0% {margin-left: 0;}
    20% {margin-left: 0;}

    25% {margin-left: -100%;}
    45% {margin-left: -100%;}

    50% {margin-left: -200%;}
    70% {margin-left: -200%;}

    75% {margin-left: -300%;}
    100% {margin-left: -300%;}
}

En el pie de pagina, haciendo uso de la etiqueta <footer> he colocado la imagen de la Universidad, asi como tambien nombre y marca de derechos reservdos. 

2. Diseñar Paginas de Dos Columnas. 

Para desarrollar y diseñar paginas con una estructura de dos columnas, he dividido el contenido html en dos grupos, con el selector de id, la primera caja es nombrada: <div id="MENU">, contenedor que como es obvio encerrara el menu interactivo de la pagina, mientras la segunda caja es nombrada: <div id="contenedor">. 

En el arhivo de estilos, css lo mas importante ha sido posicionar correctamente las cajas, y de tal manera adoptar una estructura parecida a la de la imagen de la guia de practica. 

Codigo Representativo: 

#MENU{
    border: 1px solid rgb(63, 51, 51);
    width: 25%;
    padding-top: 50px;
    padding-bottom: 60px;
    float: left;
}

#contenedor{
    background-color: rgb(233, 41, 41);
    margin-left: 399px;
    margin-top: -570.9px;
    padding: 50px 50px 50px 50px;
    float: left;
}

3. Diseñar Paginas de Tres Columnas.

Para desarrollar y diseñar paginas con una estructura de tres columnas, he dividido el contenido html en tres grupos, con el selector de id, la primera caja es nombrada: <div id="MENU">, contenedor que como es obvio encerrara el menu interactivo de la pagina, la segunda caja es nombrada: <div id="texto">, esta caja contendra toda la informacion textual del archivo html en cuestion y finalmente, la tercera caja es nombrada: <div id="Audio-Visual"> esta caja contandra todo el contenido auditivo y visual de la pagina. 

En el arhivo de estilos, css lo mas importante ha sido posicionar correctamente las cajas, y de tal manera adoptar una estructura parecida a la de la imagen de la guia de practica.

Codigo Representativo:

#texto{
    background-color: rgb(233, 41, 41);;
    width: 40%;
    margin-left: 10px;
    padding: 5px 20px;
    border-width: 3px;
    float: left;
}

#Audio-Visual{
    border: 1px solid rgb(63, 51, 51);
    width: 40%;
    margin-left: 10px;
    border-width: 3px;
    padding-left: 6.3px;
    padding-right: 6px;
    height: 800px;
    float: left;
}

4. Organizacion de Archivos y Directorios. 

Se a organizado el proyecto, bajo lo pedido en la guia de practica, existiendo entonces 6 carpetas: Audio, css, Fuentes, html, Imagenes y Videos. 

Dnetro de la carpeta css, •	Un archivo será para el diseño a dos columnas, otro archivo para el diseño a tres columnas, otro archivo para el diseño de la página home. Por último, un archivo para las reglas CSS relacionas a textos, colores, tablas, secciones, artículos, imágenes, etc.

5. Selectores por etiquetas. 

Se a utilizado selectores tanto de id como de clase, si bien es cierto, no existe una regla especifica y estricta que indique cuando utilizar un selector de id o uno de clase, es importante tomar en consideracion que, los selectores por id son exclusivos en determinado archivo, mientras que los selectores de clases, pueden ser llamados varias veces dentro del mismo archivo. 

Codigo Representativo:

Selector id: <a href="/html/informacion.html" id="menuInfo"><img src="/Imagenes/Informacion.jpg" alt="Imformación General" id="imgInformacion"/></a>

Selector de clase: <div class="slider">

6. Personalizacion de Fuentes.

Se ha descargado para el proyecto 4 distintas fuentes, meiante el enlace https://fonts.google.com/, cada fuente aplicada ya sea a titulos <h1>, subtitulos <h2> o <h3>, para texto <p> o para referencias <aside>.

En el archivo css se a tenido que importar las fuentes, indicando un nombre y la URL (direccion de la fuente). 

Codigo Representativo: 

@font-face{
    font-family: 'MiFuente-Bangers-Regular';
    src: url(/Fuentes/Bangers-Regular.ttf);
}

Las etiquetas <h1> y <h2> utilizan la fuente: AbrilFatface-Regular.ttf

La etiqueta <h3> utiliza la fuente: DancingScript-VariableFont_wght.ttf

La etiqueta <p> utiliza la fuente: RobotoSlab-VariableFont_wght.ttf

La etiqueta <aside> utiliza la fuente:
Bangers-Regular.ttf

7. Menú de Navegacion. 

Para crear el menu de navegacion, se a lincado imagenes representativas de cada tema a las distintas paginas html, usando etiquetas tales como <nav>, <a> y <img>, a continuacion se presenta mediante codigo la mencionado anteriormente. 

<nav>
    <a href="/html/informacion.html" id="menuInfo"><img src="/Imagenes/Informacion.jpg" alt="Imformación General" id="imgInformacion"/></a>
    <a href="/html/proximamente.html" id="menuProx"><img src="/Imagenes/proximamente.jpg" alt="Proximamente" id="imgProximamente"/></a>
    <a href="/html/top10.html" id="menuTop"><img src="/Imagenes/top10.jpg" alt="Top 10" id="imgTop10"/></a>
    <a href="/html/polemicas.html" id="menuPole"><img src="/Imagenes/polemicas.jpg" alt="Polemicas" id="imgPolemicas"/></a>
    <a href="/html/TopPeliculas.html" id="menuTopP"><img src="/Imagenes/peliculas1.jpg" alt="Peliculas" id="imgTopPeliculas"/></a>
    <a href="/html/TopSeries.html" id="menuTopS"><img src="/Imagenes/series.jpg" alt="Series" id="imgTopSeries"/></a>
    <a href="/html/TopDocumentales.html" id="menuTopD"><img src="/Imagenes/documentales.jpg" alt="Documentales" id="imgTopDocumentales"/></a>
    <a href="/html/estadisticas.html" id="menuEst"><img src="/Imagenes/estadisticas.jpg" alt="Estadisticas" id="imgEstadisticas"/></a>
    <a href="/html/contacto.html" id="contacto"><img src="/Imagenes/contacto.png" alt="Contacto" id="imgContacto"></a>
</nav>

8. Crear una nueva página HTML, en donde, se muestre un formulario de contacto o crear cuenta que tenga campos como: nombre, mensaje y botón para enviar.

Para la creacion de la barra de "remitente" use la etiqueta <input> que recibe como argumento: type (tipo de entrada), name (nombre de la variable), placeholder (ayuda impresa en el campo de texto).

Codigo Representativo: 

<input type="text" id="txtRemitente" name="txtRemitente" placeholder="Introduce Tu Nombre">

Para la creacion de la area de texto, use la etiqueta <textarea> que recibe como argumento: name, rows, cols y placeholder. 

Codigo Representativo: 

<textarea name="textarea" rows="20" cols="63" placeholder="Escribe Aquí tu Nombre"></textarea>

Para la creacion del boton de envio, use la etiqueta <imput> que recibe como argumentos: type (tipo de entrada), name (nombre de la variable), placeholder (texto en el boton).

Codigo Representativo: 

<input id="button4" type='button' name='boton4' value='Enviar' style='width:200px; height:50px'>

9. Validacion de los archivos html y css.

Para la validacion del correcto desarrollo y diseño de la pagina, se ha hecho uso de la pagina web W3C: https://validator.w3.org/, cerciorandonos de este modo la correcta sintaxis de todos los archivos del proyecto. 

10. Incluir la información de GitHub (usuario y URL del repositorio de la práctica).

Usuario: jorgeYela
URL: https://github.com/jorgeYela/Practica02-Mi-Sitio-Web-CSS-.git

RESULTADO(S) OBTENIDO(S): Mediante esta práctica hemos podido conocer las pautas necesarias para definir el estilo y el aspecto de un archivo escrito en lenguaje de etiquetas, html. Empleando entonces mediante las hojas de estilo en cascada (css), estructura de cajas, colores, fuentes de texto, espacio entre los distintos elementos de la página, es decir, en definitiva, otorgar estilos a una pagina web.

CONCLUSIONES: Es importante conocer la estructura de las hojas de estilo en cascada (css), ya que es un pilar fundamental para el desarrollo web, dado que es la forma mediante la cual el programador le dice al cliente (navegador) como mostrar los distintos elementos del archivo html, consiguiendo entonces, mediante la conexión entre css y html, el flujo perfecto entre estilos y contenido. 

RECOMENDACIONES: 
Revisar el material facilitado por el docente .
Asistir a las horas de clases.  