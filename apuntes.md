# Github

Esta es una documentacion basica sobre Github.

Github es un sistema de control de versiones, que nos ayuda a llevar un orden completo de las modificaciones y avances de un trabajo. Sirve para poder trabajar un proyecto en diferentes ordenadores y poder acceder a lo que has hecho anteriormente con muchas más opciones.

En Github podemos hacer muchas cosas pero las más significativas y importantes son las siguientes:

- Podemos hacer que podamos tirar hacia atrás en un trabajo subiendo commits por si ocurre algún problema y no sabemos qué hacer volvemos a como lo teníamos antes.
- Trabaja con ramas para poder editar cosas sin tener que tocar el trabajo principal.
- Se pueden crear clones de los repositorios para poder hacer trabajo simultáneo en diferentes ordenadores y después juntarlo todo.
- Puedes trabajar sin conexión a la red.
- Trabaja con plataformas de desarrollo colaborativo para poder tener los repositorios en la nube.
- Una vez instalado Github tendremos que configurar nuestro nombre de usuario y email con estos comandos en la consola.

git config--global user.name “Tu nombre”
git config--global user.email tugmail@gmail.com
Para crear un repositorio solo tendremos que darle al botón de "Nuevo" en "Crear un nuevo repositorio".

![Imagen1.png](img/Imagen1.png)

Una vez tenemos el repositorio creado tenemos que clonarlo en nuestra máquina local para poder trabajar y después subirlo a Github para hacer las pruebas fuera por si ocurre algo. Primero de todo tendremos que copiar la URL del repositorio.

![Imagen2.png](img/Imagen2.png)

Y después en nuestra consola en la raíz del repositorio tendremos que poner los siguientes comandos

1. -git clone URL del repositorio
2. -git init (para iniciarlo)
3. -git add “archivo” o git add . (para subir el archivo o todo)
4. -git commit-m “nombre del commit” (para saber que hemos subido por si tenemos que ir hacía atrás saber que es lo último que hemos hecho)
5. -git push origin main (para subirlo a la rama principal del repositorio)

Todo esto si ya tenemos el repositorio inicializado por el README si no hemos marcado esta opción tendremos que poner antes de lo anterior estos comandos

1. -git init
2. -git add README.md (para iniciar el repositorio en el local)
3. -git branch-M main (para asociarlo a una rama)-git commit-m "first commit”
4. -git remote add origin https://github.com/TuNombre/Prueba.git. (para asociar el local con el remoto)
5. -git push-u origin main

Y para sincronizarlo tendremos que poner los comandos de diferente forma git init

1. -git remote add origin https://github.com/TuNombre/Prueba.git.
2. -git branch-M main-git add .
3. -git commit-m "first commit"
4. -git push-u origin

Y por último para importar un repositorio ya creado solo tenemos que copiar la URL y a la hora de crear el nuevo repositorio nos dará la opción de importar un repositorio y tendremos que copiar la URL allí.

![Imagen3.png](img/Imagen3.png)

Si queremos utilizar Github Pages tendremos que ir al repositorio y en sus opciones de ajustes tendremos que ir al apartado de Pages y poner la rama principal y la carpeta root cuando hayamos hecho eso nos saldrá la URL del Pages y ya. Es muy importante que tengamos el index.html para que lo reconozca y podamos acceder

![Imagen4.png](img/Imagen4.png)


# Markdown

Markdown es un lenguaje de marcas usado por Github.

Tenemos etiquetas básicas para hacer según qué cosas como encabezados diferentes, estilos de letras, listas y más pero ahora veremos las más utilizadas y básicas.

Los encabezados se hacen con la etiqueta # y cuantas más almhodillas le pones más pequeño será.
# H1
## H2
### H3
#### H4
##### H5
###### H6

Los estilos de letra que podemos utilizar son los siguientes:
- Para poner letra en itálica o cursiva tendremos que poner el texto entre asterisco o entre barras bajas.
*texto* o _texto_
- Para ponerlo en negrita tendremos que hacer lo mismo pero en vez de poner uno pondremos dos.
** texto ** o __ texto __
- Para tachar el texto lo pondremos entre ~
~texto~
- También podemos hacer listas ordenadas y desordenadas
Para hacer una lista ordenada solo tendremos que poner un numero delante
1.Primer cosa
2.Segunda cosa
3.Tercer cosa
- Y para hacerla desordenada solo tendremos que poner uno de los siguientes símbolos
/*/-/+/
● Cosa
-Cosa
+Cosa
- Para crear párrafos tendremos que introducir lineas en blanco entre el texto
  
texto
  
- El código se ha de incluir entre acentos graves (`). Si en el código aparece un acento grave, se ha de introducir el carácter dos veces al principio de la sección del código.
``Todo esto es `código`.``
- También se puede marcar el área correspondiente al código insertando tres acentos graves al principio y al final. Junto a los tres iniciales se puede indicar el lenguaje (HTML, JavaScript) para que incluso se muestre con los colores adecuados:
```html
<html>
<head>
</head>
</html>
```
- Para poder hacer links tendremos que poner entre corchetes el nombre del link y después el link entre paréntesis.
[Texto del link]0(https://ejemplo.com/ "Título opcional del enlace")

- Para introducir imágenes se puede hacer de dos formas diferentes

1. Desde una URL
![Logo de GitHub](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png "GitHub Logo")

2. Desde un archivo
![Mi imagen](imagenes/foto.png "Mi foto")

- Para hacer una tabla y configurarla tendremos que hacer esto y podemos hacer esto.
a. Los dos puntos se usan para alinear las columnas (izquierda , derecha o centrado).
b. No es necesario que estén alineadas verticalmente. Solo a nivel visual para claridad del código.
c. Se han de poner al menos tres guiones para separar cada encabezado.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

- Para poner una nota al pie de la página tendremos que poner entre corchetes un cono y un 1.
Texto con enlace al pie de página [^1]

- Y por último para hacer listas de verificación tendremos que dejar un espacio en blanco entre los corchetes que no estén marcadas
A-[x]
B-[ ]
C-[ ]


# HTML

HTML es un lenguaje de marcas para hacer páginas web en navegadores y actualmente el más utilizado. Las normas de este lenguaje las define el World Wide Web (W3C) y por esto todas las páginas web están hechas de forma similar.

Historia del HTML

En el año 1993 Tim Bernes-Lee describe el lenguaje HTML en un primer borrador que no se convirtió en estándar. Posteriormente, Dave Raggett propone el HTML+, que tampoco funciona bien. La IETF crea un grupo de trabajo para desarrollar un estándar basado en los borradores anteriores. Entonces surge el HTML 2.0 en 1996, el desarrollo pasa al W3C. A partir de ahí se ha ido mejorando el lenguaje hasta llegar al HTML 5 el utilizado actualmente donde nos da muchísimas más opciones.

HTML significa HyperText Markup Language

HyperText es el texto que enlaza con otros recursos como la base de la web donde se realiza.
Markup son las etiquetas que estructuran y dan forma a la página web.
Language es el lenguaje con reglas y estructuras.
En este lenguaje de marcas hay muchas opciones para poder hacer tu página web mejor y ordenada a forma de programación. Para poder realizar todo esto tendremos que saber las etiquetas básicas y sus funciones.

Para empezar una página web hay una etiqueta que define en que html queremos empezar a escribir donde te da cierta información importante como el idioma predeterminado, el título y más cosas.

Ahora veremos un ejemplo de código HTML y lo que hace cada etiqueta que contiene.

<!DOCTYPE html> Aquí nos dice el tipo de documento que es.
<html lang="es"> Aquí podemos ver el idioma y la etiqueta de HTML se abre con todo lo que contendrá la página.
<head> Aquí se encuentra lo que no se verá en la página web pero está configurado y información adicional.
<meta charset="UTF-8"> Aquí podemos ver los caracteres que utilizará.
<meta name="viewport" content="width=device-width, initial-scale=1.0">Información adicional
<title>Primera Página ASIX </title> Aquí podemos ver el título de la página.
</head>

Como podemos ver las etiquetas siempre se abren y se cierran con <etiqueta> Texto </etiqueta>
También se puede observar que dentro de las etiquetas podemos poner atributos para que hagan cosas más concretas y fáciles de entender.
<etiqueta> atributo Texto </etiqueta>
También existen etiquetas sin contenido como una imagen y se les llama elementos vacíos o al contrario si tienen más de un elemento juntos se les llama anidamiento.

Aqui tenemos otro ejemplo donde hay muchas más etiqueta muy utilizadas
<body> Esta etiqueta encierra todo el contenido que mostrará la página web
<h1>Primer Título </h1> En esta etiqueta se muestra el titulo del articulo que va abajo y el número indica la grandaria e importancia.
<hr> Esta etiqueta mete una línea horizontal para separar información.
<h2>Índice de contenidos</h2> Una etiqueta igual pero con el título menor
<!--ol y li es una lista ordenada--> Esta etiqueta es un comentario que sirve para guiar al programador para saber la estructura, no sale en la página web.
<ol> Esta etiqueta hace una lista ordenada
<li>Introducción </li> Y esta etiqueta ordena la lista por números
<li>Quienes somos</li>
<ul>Software</ul> Esta etiqueta hace una lista desordenada
<ul>Hardware</ul>
<li>Nuestras listas de negocios</li>
</ol>
<ul>
<li>Intro</li>
<li>Quienes somos</li>
<li>Nuestra lista</li>
</ul>
<p> Esta etiqueta hace un párrafo y lo mueve a una línea nueva y ocupa todo el ancho de la página
<strong>Lorem ipsum</strong> Esta etiqueta resalta la letra en negrita.
dolor sit, amet consectetur adipiscing elit. <span>Optio, quas! Quas, omnis vel quaerat eum dolorem fugit ab inventore veritatis</span> Esta etiqueta sirve para seleccionar un trozo de texto, quia cupiditate
recusandae ipsum eos ipsam quibusdam repudiandae, sed cumque. </p>
<br> Esta etiqueta sirve para hacer un salto de línea
<em>Lorem ipsum</em> esta etiqueta sirve para dar un énfasis
</body> Cierre de la etiqueta de body
</html> Cierre de la etiqueta de html

Las rutas se usan para enlazar archivos (como imágenes, CSS o scripts) y hay dos tipos que son las siguientes:

Relativas: dependen de la ubicación actual del archivo.
  ```<img src="img/logo.png" alt="Logo">```

Absolutas: incluyen toda la dirección desde el servidor.

```<img src="C:/img/logo.png" alt="Logo">```

Una herramienta muy útil que hemos visto son los validadores de códigos HTML ya que nos permiten ver si hay algún fallo en nuestro código HTML de forma rápida y segura. Funciona de manera simple, subes tu archivo y el validador solo lo revisa y te pone los fallos y donde están.

![validador1](img/validador1.png)
![validador2](img/validador2.png)

Los formularios permiten al usuario enviar datos a una página diferente.
<form>
  <label for="nombre">Nombre:</label>
  <input type="text" id="nombre" name="nombre">
  
  <label for="email">Correo:</label>
  <input type="email" id="email" name="email">
  
  <input type="submit" value="Enviar">
</form>
Hay atributos en las etiquetas que son muy utilizados como pueden ser el for, name, value, id y más.
Suelen ser para identificar la información o darle algún trabajo.

Para hacer nuestra página web más fácil de ver y mejor distribuida hay etiquetas semánticas que se usan mucho por las razones que he dicho
<header>: cabecera de la página.
<nav>: menú de navegación.
<main>: contenido principal.
<section>: una sección del contenido.
<footer>: pie de página.

En la etiqueta de body hay dos elementos diferentes que son:
Elementos de bloques y elementos de línea.
Los elementos de bloques son grandes estructuras de etiquetas que normalmente los navegadores los muestran como bloques independientes y los separa como por ejemplos los títulos, párrafos, lista o tablas.
Y los elementos de línea son pequeñas estructuras que representan o describen pequeños trozos de texto o datos y el navegador los suele mostrar en línea uno tras otro dentro del bloque que los contiene. Son un ejemplo los hiperenlaces, las citas o las imágenes.
Ahora explicaré una etiqueta que no salen en el ejemplo.
Los enlaces son la etiqueta a a href="https://www.mozilla.org/es-AR/about/manifesto/">Manifesto Mozilla /a

Y estos son las etiquetas más utilizadas y la historia del HTML.

# CSS

Anteriormente las páginas web eran muy sencillas y planas y para cambiar esto se ideo el CSS que hace que las páginas web se ven muchisimo mejor con más colores, formas, tamaños y cosas inpensables que se podían hacer con CSS. 
CSS es Cascading Style Sheets, entonces HTML se ocupa de hacer la página web y CSS se ocupa de enlazar las cosas del HTML y darles efectos visuales que se plasman en la página en el navegador que utilices.

Esto tiene ventajas e inconvenientes que ahora veremos:

- Ventajas
1. Posibilidad de mantener el código
2. CSS es más potente que HTML en diseños de etiquetas 
3. CSS es un lenguaje sencillo de utilizar y entender
4. Se pueden definir más de una página CSS para una o más páginas webs

- Inconvenientes 
1. El único inconveniente es que no todos los navegadores funcionan ni se comportan igual entonces esto provoca que a veces haya que cambiar las hojas de estilos según el navegador porque no cumple los estandares mínimos del navegador.

- Ubicaciones del CSS
El CSS se puede implementar en diferentes lugares del código 

1. En la etiqueta se llama estilo inline y se hace con el atributo style. 
    - ```<p style="text-align:center; color:red">Paràgraf centrat vermell</p>```
2. En la cabecera del documento que es nombrado estilo interno que funciona de manera que dentro de la etiqueta que pongamos en el head pondremos las caracteristicas de las etiquetas que queremos que cambien.
    - ``` <head>
               <style> 
                  p { 
                    text-align:center; 
                    color:red 
                  } 
                </style>
         </head>```
3. Y por último es el estilo externo que es hacer un archivo CSS aparte y enlazarlo en el head del documento, esta es la mejor manera y más sencilla y dentro del CSS pondremos todos los estilos a las etiquetas que queramos como hacemos en el estilo interno 
    -  ```<link rel="stylesheet" href="estils.css" type="text/css" />```

- Estructura básica 

1. Cada regla de CSS esta compuesta por un selector y unas declaraciones. El selector indica a que elementos se implementaran los estilos y las declaraciones son las propiedades y valores que ponemos dentro. 
p -> Selector 
{
  font-size: 10pt; ->Declaracion
  background-color: gray;->Declaracion
}

2. Comentarios 
Los comentarios sirven para dar informacion a las personas que vean el codigo de primeras y no entiendan algo que puedan conseguir entenderlo y se ponen de esta manera 
/*
Comentarios
*/

3. Si tenemos dos etiquetas diferentes que queremos que tengan el mismo estilo para no tener que repetir dos veces las declaraciones podemos agruparlas y ponerlo una sola vez 

h1,p {color: red}

4. Tipos de Selectores 
    - Selector de elementos: Esto afecta a todos los elementos de la página que tengan la etiqueta que pongamos 
    /* All <a> elements. */
    a {
    color: red;
    }
    
    - Selector de clase: Estos solo afectaran a los que en la etiqueta tengan el atributo llamado igual que el id
            example {
            property: value;
            property2: value2;
                    }
        Afectaría a los siguientes elementos HTML:
            <p class="example">
            <li class="example">
            <div class="example">

    - Selectores Avanzados

        - Selector Universal: Sirven para hacer que afecten a todas las etiquetas de la página y se ponen con un *
            Toda la página tendrá un borde de 1 píxel negro 
            *  {
             border: 1px solid #000000;
             }

        - Selector de Atributos: Permiten seleccionar elementos de una función que hemos puesto en el código 
            Afecta a todas las imagenes que tengan alt 
            img[alt] {
                border: 1px solid #000000;
            }

        - Selector de Hijos: Esto afecta a atributos que vengan de una etiqueta que este por encima suya 
            Aqui solo los elementos strong que vengan de un h3 se pondran azul
            h3>strong {
            color: blue;
            }

        - Selectores Descendientes: Son iguales que los hijos pero aqui afectan a todos los que esten por debajo


        - Selectores de Hermanos Adyecentes: Permiten seleccionar un elemento concreto que esta justo después del otro elemento al mismo nivel
            <h1>Encabezado 1 </h1>
            <h2>Encabezado 2 (hermano adyacente) </h2>
            <h2>Encabezado 2 (hermano no adyacente) </h2>

- Pseudoclases y Pseudoelementos 

    - Pseudoclases: Son para definir acciones que hacen según lo que haga el usuario. 
        :link: El estado normal por defecto de los enlaces. Tal y como se ven por primera vez.
        :visited: Enlaces que ya se han visitado con el navegador que se está utilizando.
        :focus: Enlaces (o campos de formularios, o cualquier otra cosa) que tienen en ese momento el cursor en su interior.
        :hover: Enlaces que tienen en este momento el puntero del ratón sobre ellos.

    - Psuedoelementos: Es lo mismo que las pseudoclases pero si solo queremos afectar a una cosa en concreto de la linea
         selector::pseudo-elemento { propiedad: valor; }
            /* Selecciona la primera línea de un <p> */
            p::first-line {
                color: red;
            }


4. Composición 

Algunas etiquetas ocupan todo el ancho de la página y eso se puede modificar con márgenes, bordes y rellenos.

- Los márgenes funcionan con margin y podemos hacer que este orientado hacia un lado o otro, hacia arriba o hacia abajo (margin-top, margin-right, margin-bottom, margin-left ) controlandolo con unidades como píxeles, porcentajes o de forma automática. 

- Los bordes funcionan con border y podemos editar el grosor , estilo, ubicación y color de estos. Con border-width, border-style, border-color

- Y por último podemos editar el relleno de las cosas con el padding que es un espacio transparente que se usa para que las cosas no esten juntas y se pueden modificar hacia los lados y hacia arriba y abajo (padding-top, padding-right, padding-bottom, padding-left).

5. Google Fonts

Esto se utiliza para cambiar la fuente de la letra de nuestra página web de forma muy sencilla. 
Tendremos que elegir primero la fuente que queremos y arriba a la derecha nos saldra un símbolo de +. Una vez dado ahí nos saldrán dos opciones para copiar y pondremos el link que podemos copiar en el head de nuestra página con la etiqueta link y ya estaría.
  <link rel="preconnect" href="https://fonts.googleapis.com">


# Diseño Responsive, Media Query y Bootstrap

- El diseño responsive es una tecnica que sirve para que las páginas web se adapten a la pantalla que el usuario disponga o le vaya de mejor manera y la página no pierda nada de información y sea mejor de leer y ver según sea más grande o pequeña. 

- El media query es una técnica que es de CSS que es para que cuando hagamos el diseño responsive coloquemos las cosas de manera diferente al agrado del programador ya sea cambiando las cosas de color o de ubicación, que se utiliza con el @media.
    
    En este caso como podemos ver si la pantalla no supera los 600 píxeles se verá de esa manera, si no se verá como esta en nuestro codigo HTML 
    @media only screen and (max-width: 600px) {
    /* column-2 pasará de tener 50% a 100% */
    .column-2{
        width: 100%;
    }
    /* column-3 pasará de tener 33.33% a 100% */
    .column-3{
        width: 100%;
    }
    /* column-4 pasará de tener 25% a 50% */
    .column-4{
        width: 50%;
    }
}
- Tambien existen operadores para hacer más sencillo y rápido el media query como el and, not, only y or. 

    @media only screen and (min-width:320px) and (max-width:480px){
        <!—- Aquí van todos los estilos CSS -->
    }

- Ahora veremos los párametros que más se utilizan en el media query 
    1. width: anchura de la ventana del navegador.
    2. height: altura de la ventana del navegador.
    3. device-width: anchura de la resolución de pantalla.
    4. device-height: altura de la resolución de pantalla.
    5. orientation (portrait/landscape): dispositivo en horizontal o en vertical.
    6. resolution: densidad de píxeles.

- Si ponemos los atributos para el tamaño de la pantalla,la etiqueta Viewport es necesaria. Va implementada en el bloque <head> del documento HTML.

<meta name="viewport" content="width=device-width, initial-scale=1.0">

Aquí se especifica que el ancho de la web sea la anchura de la resolución de la pantalla y que no se escale inicialmente. 

- Bootstrap

Bootstrap es un framework CSS (con algo de JavaScript) diseñado para facilitar el desarrollo de sitios web responsivos, es decir, que se adaptan automáticamente a diferentes tamaños de pantalla (móvil, tablet, escritorio, etc.).

- Ventajas del Bootstrap:
    1. Permite aplicar estilos fácilmente asignando clases HTML sin necesidad de escribir mucho CSS.
    2. Facilita el diseño responsive con su sistema de columnas y media queries predefinidas.
    3. Sigue la filosofía Mobile First (primero diseñar para móviles porque actualmente se hacen más páginas para móviles que para ordenadores), lo cual es ideal para la experiencia de usuario.

- Bootstrap usa una plantilla de una tabla de 12 columnas, que permite distribuir los elementos del diseño fácilmente.

    Se adapta al tamaño de pantalla usando clases como:
    1. col-12 (pantallas muy pequeñas)
    2. col-sm-6 (pequeñas)
    3. col-md-4 (medianas)
    4. col-lg-3 (grandes)
    5. col-xl-2 (muy grandes)

- Se implenta en nuetra página de forma sencilla como el css o el google fonts, primero tendremos que copiar el link de bootstrap que se encuentra en la paágina principal y copiar la etiqueta link y el script y pegarla en el bloque head del HTML, una vez hecho eso solo queda escoger los componentes que quieres meter y copiar el codigo de la página de bootstrap oficial y implementarlo en la tuya modificando las cosas predeterminadas por las tuyas a tu convenencia. 

- Hay componentes muy utilizados como los sliders, las barrras de navegación, tablas con estilos y la fácil distribución de los espacios que hay en la página usando todo tipo de etiquetas flex, entre muchas más cosas. 