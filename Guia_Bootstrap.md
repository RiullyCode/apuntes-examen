# Apuntes Bootstrap

## Link Boostrap
CSS: 
```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
```

Script:
```html
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js" integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
```

## `Sistema de columnas y contenedores de Bootstrap`
El sistema de columnas y contenedores de Bootstrap es una forma flexible y poderosa de crear diseños responsivos en una página web. Bootstrap es un marco de diseño front-end muy popular que proporciona una gran cantidad de herramientas y componentes para crear sitios web y aplicaciones web responsivas.

El sistema de columnas y contenedores de Bootstrap se basa en la idea de que una página web se divide en filas y columnas, y que cada columna puede contener elementos como texto, imágenes, formularios y otros componentes.

Para empezar a usar el sistema de columnas y contenedores de Bootstrap, es necesario agregar la biblioteca de Bootstrap a su sitio web. Puede hacer esto descargando la biblioteca de Bootstrap y agregando los archivos CSS y JavaScript a su sitio, o puede usar una CDN (Content Delivery Network) como la de Bootstrap para cargar los archivos desde un servidor externo.

Una vez que haya agregado la biblioteca de Bootstrap a su sitio web, puede comenzar a usar el sistema de columnas y contenedores. El sistema utiliza contenedores para envolver las filas y columnas de su sitio web. Los contenedores son simplemente elementos HTML que se usan para limitar el ancho del contenido de su sitio web.

Para crear una fila en Bootstrap, debe agregar un elemento HTML con la clase "row". Dentro de una fila, puede agregar una o varias columnas. Las columnas se definen usando clases como "col-md-4" o "col-lg-6". Estas clases indican el ancho de la columna en diferentes tamaños de pantalla. Por ejemplo, "col-md-4" significa que la columna ocupará 4 de las 12 columnas disponibles en pantallas medianas.

En resumen, el sistema de columnas y contenedores de Bootstrap le permite crear diseños responsivos en su sitio web de manera fácil y flexible. Simplemente use las clases proporcionadas por Bootstrap para definir filas y columnas, y ajuste los tamaños según sea necesario para adaptarse a diferentes tamaños de pantalla.
```html
<!DOCTYPE html>
<html>
<head>
  <title>Ejemplo de Bootstrap 5</title>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0/dist/css/bootstrap.min.css">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container">
  <h1>Mi sitio web</h1>
  <p>¡Bienvenido a mi sitio web! Aquí hay algunos ejemplos de cómo se ve el sistema de columnas y contenedores de Bootstrap 5:</p>
  
  <div class="row">
    <div class="col-md-6">
      <h2>Columna 1</h2>
      <p>Esta es la primera columna. En una pantalla mediana, ocupará 6 de las 12 columnas disponibles.</p>
    </div>
    <div class="col-md-6">
      <h2>Columna 2</h2>
      <p>Esta es la segunda columna. También ocupará 6 de las 12 columnas disponibles en una pantalla mediana.</p>
    </div>
  </div> 
</div>
</body>
</html>
```
La estructura básica es la misma, pero las clases para las columnas han cambiado ligeramente. En lugar de usar "col-md-4", ahora usamos "col-md-6" para que cada columna ocupe la mitad del ancho disponible en pantallas medianas.

![Descripción de la imagen](https://cdn.discordapp.com/attachments/914613587715182622/1082053938875998338/image.png)

### Tipos de contenedores
En Bootstrap hay tres tipos de contenedores: .`container`, .`container-fluid`, y `.container-xxl.` Cada uno de ellos tiene una finalidad específica y se adapta a diferentes necesidades de diseño.

`.container`: este es el contenedor predeterminado en Bootstrap. Es un contenedor con un ancho máximo fijo y centrado en la página. Se adapta a diferentes anchos de pantalla utilizando un sistema de cuadrícula de columnas que se ajusta automáticamente en función del tamaño de la pantalla. Es adecuado para la mayoría de los diseños web y se utiliza comúnmente para la mayoría de los proyectos.

.`container-fluid`: este es un contenedor de ancho completo que se extiende hasta el borde de la ventana del navegador. Es útil cuando se desea un diseño sin márgenes. No tiene un ancho máximo fijo y se adapta a diferentes anchuras de pantalla mediante un sistema de cuadrícula de columnas. Es ideal para diseños que requieren imágenes o elementos que se extienden a lo ancho de la pantalla.

.`container-xxl`: este es un contenedor más ancho que .container y está diseñado para pantallas grandes. Es similar a .container-fluid, pero tiene un ancho máximo específico (1400px) en lugar de extenderse completamente. Este contenedor es útil cuando se requiere un ancho máximo específico para diseños en pantallas grandes.

Estos tres tipos de contenedores ofrecen una gran flexibilidad para adaptarse a diferentes necesidades de diseño. Seleccionar el tipo de contenedor adecuado es importante para crear un diseño limpio y legible.

### `Funcionamiento sistema de rejilla dependiendo de la pantalla`

La rejilla de Bootstrap es un sistema de columnas que se utiliza para crear diseños responsivos en la página web. La rejilla está compuesta por filas y columnas, y cada columna está dividida en 12 partes iguales, independientemente del tamaño de la pantalla.

Bootstrap utiliza clases CSS específicas para definir el tamaño de las columnas en función del tamaño de la pantalla. Hay cinco tamaños diferentes de pantalla que se utilizan en Bootstrap:

`Extra pequeño (XS)` para pantallas pequeñas (menos de 576 píxeles).

`Pequeño (SM)` para pantallas medianas (entre 576 y 768 píxeles).

`Mediano (MD)` para pantallas grandes (entre 768 y 992 píxeles).

`Grande (LG)` para pantallas extra grandes (entre 992 y 1200 píxeles).

`Extra grande (XL)` para pantallas muy grandes (más de 1200 píxeles).

Para especificar el tamaño de una columna en función del tamaño de la pantalla, se utiliza la sintaxis col-{tamaño}-{número de columnas}, donde {tamaño} es el tamaño de la pantalla y {número de columnas} es el número de columnas que la columna ocupará en la fila.

Por ejemplo, para crear dos columnas de igual ancho en una pantalla mediana, podemos usar las clases col-md-6 en ambas columnas. Esto significa que cada columna ocupará 6 de las 12 columnas disponibles en una pantalla mediana.

Bootstrap también tiene clases específicas para tamaños de pantalla más grandes o más pequeños, lo que permite personalizar el diseño para adaptarse a diferentes tamaños de pantalla. Por ejemplo, para hacer que una columna ocupe todo el ancho disponible en una pantalla extra pequeña, podemos usar la clase col-xs-12.

```html
<div class="container">
  <div class="row">
    <div class="col-sm-6 col-md-4 col-lg-3">
      <p>Columna 1</p>
    </div>
    <div class="col-sm-6 col-md-4 col-lg-3">
      <p>Columna 2</p>
    </div>
    <div class="col-sm-6 col-md-4 col-lg-3">
      <p>Columna 3</p>
    </div>
    <div class="col-sm-6 col-md-4 col-lg-3">
      <p>Columna 4</p>
    </div>
  </div>
</div>
```

En resumen, la rejilla de Bootstrap utiliza un sistema de columnas flexibles y clases CSS específicas para crear diseños responsivos que se adapten a diferentes tamaños de pantalla. Esto permite a los diseñadores crear páginas web que se vean bien en cualquier dispositivo, desde teléfonos móviles hasta pantallas de escritorio grandes.

## `d-none`
La clase CSS .d-none en Bootstrap se utiliza para ocultar elementos en la página web. Es una clase de utilidad que se utiliza comúnmente en diseños responsivos para ocultar elementos en diferentes tamaños de pantalla.

La clase .d-none se utiliza junto con otras clases que definen el tamaño de la pantalla en la que se debe ocultar el elemento. Por ejemplo, si queremos ocultar un elemento en pantallas pequeñas y medianas, podemos utilizar la clase .d-none junto con la clase .d-md-block. En este caso, el elemento se ocultará en pantallas pequeñas y medianas, pero se mostrará en pantallas grandes y extra grandes.

Además de la clase .d-none, Bootstrap también proporciona otras clases de utilidad para ocultar elementos en diferentes tamaños de pantalla. Algunas de estas clases incluyen:

`.d-sm-none`: oculta el elemento en pantallas pequeñas y más grandes.

`.d-md-none`: oculta el elemento en pantallas medianas y más grandes.

`.d-lg-none`: oculta el elemento en pantallas grandes y más grandes.

`.d-xl-none`: oculta el elemento solo en pantallas extra grandes.

Estas clases son útiles para crear diseños responsivos que se adapten a diferentes tamaños de pantalla. Al ocultar elementos en pantallas más pequeñas, se puede reducir el desorden en la página y mejorar la legibilidad en dispositivos móviles y otros tamaños de pantalla pequeños.

En resumen, la clase .d-none en Bootstrap se utiliza para ocultar elementos en la página web. Junto con otras clases de utilidad, como .d-sm-none y .d-md-none, se puede crear un diseño responsivo que se adapte a diferentes tamaños de pantalla.

Supongamos que tenemos un elemento div con la clase texto que queremos ocultar en pantallas pequeñas:

```html
<div class="texto d-none d-sm-block">
  <p>Este texto solo se mostrará en pantallas medianas y grandes.</p>
</div>
```
En este ejemplo, se utiliza la clase .d-none para ocultar el elemento div en pantallas pequeñas. Luego, se utiliza la clase .d-sm-block para mostrar el elemento en pantallas medianas y más grandes.

En este caso, el texto dentro del elemento div solo se mostrará en pantallas medianas y grandes. En pantallas pequeñas, el elemento div se ocultará y el contenido no se mostrará.

Puedes ajustar las clases utilizadas en función de tus necesidades. Por ejemplo, si deseas ocultar el elemento en pantallas grandes en lugar de pantallas pequeñas, puedes cambiar la clase .d-sm-block por .d-lg-none.

En resumen, la clase .d-none se utiliza para ocultar elementos en la página web, y se puede combinar con otras clases de utilidad para adaptar el diseño a diferentes tamaños de pantalla.

## `Texto, tipografía y colores de bootstrap:`

### `Estilos de encabezado `

Estilos de los encabezados `<h1>` – `<h6>`
Los encabezados `<h1>` – `<h6>` disponen de estilos predefinidos:

• h1 Bootstrap (2.5rem = 40px)

• h2 Bootstrap (2rem = 32px)

• h3 Bootstrap (1.75rem = 28px)

• h4 Bootstrap (1.5rem = 24px)

• h5 Bootstrap (1.25rem = 20px)

• h6 Bootstrap (1rem = 16px)

### `Clase display-x`
Bootstrap nos ofrece diferentes clases para crear encabezados de mayor tamaño. Hay cuatro
clases:
.display-1 , .display-2 , .display-3 , .display-4
Ejemplo: 

<h1 class="display-1">Encabezado Display-1</h1>

```html
<h1 class="display-1">Encabezado Display-1</h1>

```
### `Etiqueta <small>`
Gracias a la etiqueta `<small>` podemos crear un texto secundario más claro en cualquier encabezado:

<h1>h1 Encabezado <small>texto secundario</small></h1>

```html
<h1>h1 Encabezado <small>texto secundario</small></h1>
```
### `Etiqueta <mark>`
La etiqueta `<mark>` es representada con un color de fondo amarillo y algo de relleno:
<p>Párrafo con <mark>etiqueta de marcado</mark> en un texto.</p>

```html
<p>Párrafo con <mark>etiqueta de marcado</mark> en un texto.</p>
```
### `Etiqueta <abbr>`
La etiqueta `<abbr>` es representada mediante un borde inferior punteado, por ejemplo:
<p>Esto es una etiqueta <abbr title="La etiqueta abbr se representa con un borde inferior
punteado">abbr</abbr> en Bootstrap.</p>

```html
<p>Esto es una etiqueta <abbr title="La etiqueta abbr se representa con un borde inferior
punteado">abbr</abbr> en Bootstrap.</p>
```

### `Etiqueta <blockquote>`
Agregando la clase .blockquote `<blockquote>` obtenemos un estilo personalizado, aquí un ejemplo:
<blockquote class="blockquote">
<p>Un buen desarrollador de software trabaja con disciplina y constancia desde el primer día.</p>
<footer class="blockquote-footer">Omar Bradley</footer>
</blockquote>

Como podemos ver aplica un estilo especial.

```html
Ejemplo:
<blockquote class="blockquote">
<p>Un buen desarrollador de software trabaja con disciplina y constancia desde el primer día.</p>
<footer class="blockquote-footer">Omar Bradley</footer>
</blockquote>
```

### `Clases de bootstrap 4:`
Las siguientes clases de Bootstrap 4 se pueden agregar a los elementos HTML de estilo:

• .`font-weight-bold` Negrita

• .`font-weight-normal` Normal

• .`font-weight-light` Fina

• .`font-italic` Itálica

• .`lead` Destaca un párrafo

• .`small` Más pequeño (85% del tamaño del padre)

• .`text-left` Alineado izquierda

• .`text-center` Alineado centro

• .`text-right` Alineado derecha

• .`text-justify` Justificado

• .`text-nowrap` Texto nowrap

• .`text-lowercase` Texto en minúsculas

• .`text-uppercase` Texto en mayúsculas.text-capitalize Texto capitalizado

• .`initialism` Muestra el texto en un elemento `<abbr>` con tamaño más pequeño

• .`list-unstyled` Quita el list-style y margin-left en elementos de lista (funciona en `<ul>` y `<ol>`).

• .`list-inline` Coloca todos los elementos de una lista en una única línea.

### Colores de texto
Las clases para los colores del texto son: 
`.text-primary` `.text-secondary`, .`text-muted`, .`textsuccess`, .`text-danger`, .`text-warning`, `.text-info,` .`text-white`, .`text-dark` y .`text-light`.

Las clases de colores de fondo son: .`bg-primary` , .`bg-success` , .`bg-info` , .`bg-warning` , .`bgdanger` , .`bg-secondary` , .`bg-dark` y .`bg-light`

## `Tablas en Bootstrap`
### `Tabla básica`
Una tabla básica Bootstrap 4 tiene un relleno y
divisiones horizontales. Mediante la clase .table le
agregamos un estilo básico a nuestra tabla:

![Descripción de la imagen](https://cdn.discordapp.com/attachments/914613587715182622/1082068861152661524/image.png)

```html
<table class="table">
```
### `Tabla con filas en colores alternos`
Con la clase .table-striped agregamos filas con
colores alternos:

![Descripción de la imagen](https://media.discordapp.net/attachments/914613587715182622/1082069085594062929/image.png)
```html
<table class="table table-striped">
```
### `Tabla con bordes`
La clase .table-bordered agrega bordes en todos
los lados de la tabla y celdas:

![Descripción de la imagen](https://cdn.discordapp.com/attachments/914613587715182622/1082069296391409724/image.png)
```html
<table class="table table-striped table-bordered">
```

### `Tabla con efecto hover`
La clase .table-hover agrega un efecto al hacer
:hover con el ratón en las filas de la tabla:

![Descripción de la imagen](https://media.discordapp.net/attachments/914613587715182622/1082069915223203972/image.png)
En el caso de la imagen, estamos pasando el raton por encima de Larry
```html
<table class="table table-striped table-bordered
table-hover">
```

### `Tabla negra / oscura`
La clase .table-dark agrega un fondo negro a la tabla:

![Descripción de la imagen](https://cdn.discordapp.com/attachments/914613587715182622/1082070365284614174/image.png)

<table class="table table-striped table-bordered table-hover table-dark">

## `Clases contextuales`
Las clases contextuales se pueden usar para colorear toda la tabla  `<table>` , las filas de la tabla `<tr>` o las celdas de la
tabla `<td>`.

Las clases contextuales que se pueden usar son:

• .`table-primary` Azul: indica una acción importante.

• .`table-success` Verde: Indica una acción exitosa o positiva.

• .`table-danger` Rojo: indica una acción peligrosa o potencialmente negativa.

• .`table-info` Azul claro: indica un cambio informativo neutral o acción.

• .`table-warning` Naranja: indica una advertencia que podría necesitar atención.

• .`table-active` Gris: aplica el color de desplazamiento a la fila de la tabla o celda de la tabla.

• .`table-secondary` Gris: Indica una acción menos importante.

• .`table-light` Fondo gris claro.

• .`table-dark` Fondo Gris oscuro.

### `Colores del encabezado de la tabla`
Colores del encabezado de la tabla
La clase .thead-dark agrega un fondo negro a los encabezados de la tabla, y la clase .`theadlight` agrega un fondo gris a los encabezados de la tabla.


### Imágenes en bootstrap
### `Imagen responsive`:
Bootstrap 4 nos ofrece la clase .`img-fluid` para que las imágenes se adapten correctamente a
los distintos dispositivos.
Ejemplo:

```html
<img src="eniun.jpg" class="img-fluid" alt="Eniun">
```

### `Imagen con esquinas redondeadas`
La clase .`rounded` agrega esquinas redondeadas a una imagen:
Ejemplo:
```html
<img src="eniun.jpg" class="rounded" alt="Eniun">
```

### `Imagen con forma de círculo`
La clase .rounded-circle da forma de círculo a la imagen:
Ejemplo:
```html
<img src="eniun.jpg" class="rounded-circle" alt="Eniun">
```

### `Imagen tipo miniatura`
La clase .img-thumbnail da forma de miniatura a la imagen:
Ejemplo:
```html
<img src="eniun.jpg" class="img-thumbnail" alt="Eniun">
```

### `Alineación de imágenes`
Desplace una imagen hacia la derecha con la clase .float-right o hacia la izquierda con .floatleft:
Ejemplo:
```html
<img src="eniun.jpg" class="float-left" alt="Eniun">
<img src="eniun.jpg" class="float-right" alt="Eniun">
```
## `Botones de bootstrap`

Bootstrap 4 nos ofrece diferentes clases para darle estilo a nuestros botones: `btn`, `btn-primary`,
`btn-secondary`, `btn-success`, `btn-info`, `btn-warning`, `btn-danger`, `btn-dark`, `btn-light` y `btn btnlink`.

En primer lugar debemos incluir la clase btn y después podemos combinarla con el resto de
clases. Las clases de botón se pueden usar sobre enlaces, botones o inputs.

![Descripción de la imagen](https://cdn.discordapp.com/attachments/914613587715182622/1082072784223608882/image.png)

### `Botones con contorno`
Tenemos también clases para darle contorno a los botones: `btn-outline-primary`, `btn-outlinesecondary`, `btn-outline-success`, `btn-outline-info`, `btn-outline-warning`, `btn-outline-danger`, `btnoutline-dark` y `btn-outline-light`.

![Descripción de la imagen](https://cdn.discordapp.com/attachments/914613587715182622/1082073145835524167/image.png)

### `Botones y sus tamaños`
Disponemos de diferentes clases para definir el tamaño de los botones: `btn-sm`, `btn-lg` y `btnblock`.

![Descripción de la imagen](https://media.discordapp.net/attachments/914613587715182622/1082073337599107203/image.png)

### `Botones activados y desactivados`
Para que un botón aparezca activado o desactivado utilizamos las siguientes clases: .`active` y
.`disabled`. Se pueden usar para botones, inputs y enlaces.

![Descripción de la imagen](https://cdn.discordapp.com/attachments/914613587715182622/1082073590599532604/image.png)

### `Grupos de botones`
Para hacer grupos de botones de forma horizontal utilizamos la clase .`btn-group` y de forma
vertical utilizamos la clase .`btn-group-vertical`.

![Descripción de la imagen](https://cdn.discordapp.com/attachments/914613587715182622/1082073759785156778/image.png)

### `Dropdown`

Botones desplegables o dropdown
Podemos hacer botones desplegables utilizando la etiqueta `<button>`, las clases anteriormente
vistas e incluyendo nuevos componentes.

```html
<div class="dropdown">
  <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Dropdown button
  </button>
  <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
    <a class="dropdown-item" href="#">Action</a>
    <a class="dropdown-item" href="#">Another action</a>
    <a class="dropdown-item" href="#">Something else here</a>
  </div>
</div>
```

![Descripción de la imagen](https://cdn.shopify.com/s/files/1/2570/3194/files/bootstrap-4-multilevel-dropdown-menu-on-mouse-hover.jpg?v=1513838883)

## `Barra de navegacion`
Con Bootstrap, una barra de navegación puede extenderse o contraerse, dependiendo del
tamaño de la pantalla.
Se crea una barra de navegación estándar con la clase .navbar, seguida de una clase de colapso
sensible: .`navbar-expand-xl` | `lg` | `md` | `sm` (apila la barra de navegación verticalmente en
pantallas extra grandes, grandes, medianas o pequeñas).
Para agregar enlaces dentro de la barra de navegación, usa un elemento `<ul>` con `class =
"navbar-nav`". Luego agrega elementos `<li>` con una clase .`nav-item` seguido de un elemento
`<a>` con una clase .`nav-link`.

<nav class="navbar navbar-expand-sm bg-light">
<ul class="navbar-nav">
<li class="nav-item">
<a class="nav-link" href="#">Link 1</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link 2</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link 3</a>
</li>
</ul>
</nav>
<br>

```html
<nav class="navbar navbar-expand-sm bg-light">
<ul class="navbar-nav">
<li class="nav-item">
<a class="nav-link" href="#">Link 1</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link 2</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link 3</a>
</li>
</ul>
</nav>
<br>
```
### `Barra de navegación vertical`
Elimina la clase .`navbar-expandxl` | `lg` | `md` | `sm` para crear una
barra de navegación vertical.
<!-- A vertical navbar -->
<nav class="navbar bg-light">
<!-- Links -->
<ul class="navbar-nav">
<li class="nav-item">
<a class="nav-link" href="#">Link 1</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link 2</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link 3</a>
</li>
</ul>
</nav>

```html
<!-- A vertical navbar -->
<nav class="navbar bg-light">
<!-- Links -->
<ul class="navbar-nav">
<li class="nav-item">
<a class="nav-link" href="#">Link 1</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link 2</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link 3</a>
</li>
</ul>
</nav>
```

### `Barra de navegación centrada`

Agrega la clase .`justify-content-center` para centrar la barra de navegación.
El siguiente ejemplo centrará la barra de navegación en pantallas medianas, grandes y extra
grandes. En pantallas pequeñas, se mostrará verticalmente y alineado a la izquierda (debido a
la clase .`navbar-expand-sm`).
```html
<nav class="navbar navbar-expand-sm bg-light justify-content-center">
```
### `Barra de navegación coloreada`
Utilice cualquiera de las clases .bg-color para cambiar el color de fondo de la barra de
navegación:

.`bg-primary`

.`bg-success`

.`bg-info`

.`bg-warning`

.`bg-danger`

.`bg-secondary`

.`bg-dark`

.`bg-light`

Consejo: Agrega un color de texto
blanco a todos los enlaces en la barra de
navegación con la clase .navbar-dark, o
usa la clase .navbar-light para agregar
un color de texto negro.

```html
<!-- Grey with black text -->
<nav class="navbar navbar-expand-sm bg-light navbar-light">
<ul class="navbar-nav">
<li class="nav-item active">
<a class="nav-link" href="#">Active</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link</a>
</li>
<li class="nav-item">
<a class="nav-link disabled" href="#">Disabled</a>
</li>
</ul>
</nav>
```
## `Brand Logo (Logotipo)`
La clase .navbar-brand se utiliza para resaltar el nombre de marca / logotipo / proyecto de su
página:
```html
<nav class="navbar navbar-expand-sm bg-dark navbar-dark">
<a class="navbar-brand" href="#">Logo</a>
...
</nav>
```
Al usar la clase .`navbar-brand` en las imágenes, Bootstrap aplicará un estilo automático a la
imagen para que se ajuste verticalmente a la barra de navegación.

## `Colapsando el menú de navegación`
Muy a menudo, especialmente en pantallas pequeñas, deseas ocultar los enlaces de
navegación y reemplazarlos con un botón que debería revelarlos al hacer clic en ellos.

Para crear una barra de navegación plegable, usa un botón con `class = "navbar-toggler"`, `datatoggle = "collapse"` y `data-target = "# thetarget"`. Luego, envuelve el contenido de la barra de
navegación (enlaces, etc.) dentro de un elemento div con class = "`collapse navbar-collapse`",
seguido de una identificación que coincida con el objetivo de datos del botón: "`thetarget`".

```html
<nav class="navbar navbar-expand-md bg-dark navbar-dark">
<a class="navbar-brand" href="#">Navbar</a>
<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#collapsibleNavbar">
<span class="navbar-toggler-icon"></span>
</button>
<div class="collapse navbar-collapse" id="collapsibleNavbar">
<ul class="navbar-nav">
<li class="nav-item">
<a class="nav-link" href="#">Link</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link</a>
</li>
</ul>
</div>
</nav>
```
### `Barra de navegación con menú desplegable`
Las barras de navegación también pueden contener menús desplegables.
```html
<nav class="navbar navbar-expand-sm bg-dark navbar-dark">
<!-- Brand -->
<a class="navbar-brand" href="#">Logo</a>
<!-- Links -->
<ul class="navbar-nav">
<li class="nav-item"> <a class="nav-link" href="#">Link 1</a> </li>
<li class="nav-item“> <a class="nav-link" href="#">Link 2</a> </li>
<!-- Dropdown -->
<li class="nav-item dropdown">
<a class="nav-link dropdown-toggle" href="#" id="navbardrop" data-toggle="dropdown"> Dropdown link </a>
<div class="dropdown-menu">
<a class="dropdown-item" href="#">Link 1</a>
<a class="dropdown-item" href="#">Link 2</a>
<a class="dropdown-item" href="#">Link 3</a>
</div>
</li>
</ul>
</nav>
```

### `Formas y botones de la barra de navegación`
Agrega un elemento `<form>` con class = "`form-inline`" para agrupar entradas y botones de
lado a lado.
<nav class="navbar navbar-expand-sm bg-dark navbar-dark">
<form class="form-inline" action="/action_page.php">
<input class="form-control mr-sm-2" type="text" placeholder="Search">
<button class="btn btn-success" type="submit">Search</button>
</form>
</nav>

```html
<nav class="navbar navbar-expand-sm bg-dark navbar-dark">
<form class="form-inline" action="/action_page.php">
<input class="form-control mr-sm-2" type="text" placeholder="Search">
<button class="btn btn-success" type="submit">Search</button>
</form>
</nav>
```

## `Texto de barra de navegación`
Use la clase .navbar-text para alinear verticalmente cualquier elemento dentro de la barra de
navegación que no sea un enlace (garantiza el relleno y el color de texto adecuados)

```html
<nav class="navbar navbar-expand-sm bg-dark navbar-dark">
<!-- Links -->
<ul class="navbar-nav">
<li class="nav-item">
<a class="nav-link" href="#">Link 1</a>
</li>
<li class="nav-item">
<a class="nav-link" href="#">Link 2</a>
</li>
</ul>
<!-- Navbar text-->
<span class="navbar-text">
Navbar text
</span>
</nav>
```

## `Barra de navegación fija`
La barra de navegación puede mostrarse fija en el top o bottom de la página (arriba o abajo).
Una barra de navegación fija permanece visible en una posición fija (superior o inferior)
independiente del desplazamiento de la página.
La clase .`fixed-top` hace que la barra de navegación esté fija en la parte superior.

```html
<nav class="navbar navbar-expand-sm bg-dark navbar-dark fixed-top">
...
</nav>
```
Usa la clase .`fixed-bottom` para hacer que la barra de navegación permanezca en la parte
inferior de la página.
```html
<nav class="navbar navbar-expand-sm bg-dark navbar-dark fixed-bottom">
...
</nav>
```
Usa la clase .`sticky-top` para hacer que la barra de navegación sea fija / permanezca en la parte
superior de la página cuando se desplace. Nota: Esta clase no funciona en IE11 y versiones
anteriores (la tratará como position: relative).
```html
<nav class="navbar navbar-expand-sm bg-dark navbar-dark sticky-top">
...
</nav>
```

## Componentes en Bootstrap
Como hemos visto en los puntos anteriores, Bootstrap nos ofrece diferentes clases muy fáciles
de aprender y que podemos utilizar en nuestros proyectos para aplicar diferentes estilos a
nuestros contenedores y a nuestras etiquetas.
Además, Bootstrap nos da la posibilidad de utilizar diferentes componentes, que no son más
que pedazos de código ya programados que podemos insertar en nuestros proyectos. Por
ejemplo: menús de navegación, carousels y tablas de precios, entre otros.

### Componentes utiles para nuestros desarrollos
Algunos de los componentes que nos van a servir para nuestros desarrollos son los siguientes:

• `Modal`

```html
<!-- Button to Open Modal -->
<button type="button" class="btn btn-primary" data-toggle="modal" data-target="#myModal">
  Open Modal
</button>

<!-- The Modal -->
<div class="modal" id="myModal">
  <div class="modal-dialog">
    <div class="modal-content">

      <!-- Modal Header -->
      <div class="modal-header">
        <h4 class="modal-title">Modal Heading</h4>
        <button type="button" class="close" data-dismiss="modal">&times;</button>
      </div>

      <!-- Modal body -->
      <div class="modal-body">
        Modal body text goes here.
      </div>

      <!-- Modal footer -->
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save Changes</button>
      </div>

    </div>
  </div>
</div>
```
En este ejemplo, el botón "Open Modal" tiene los atributos "data-toggle" y "data-target" establecidos en "modal" y "#myModal" respectivamente. Esto indica que cuando se haga clic en el botón, se abrirá un modal con el ID "myModal". El modal tiene un encabezado, un cuerpo y un pie de página, cada uno con su propia clase de Bootstrap. El botón "Close" tiene el atributo "data-dismiss" establecido en "modal", lo que indica que al hacer clic en el botón, se cerrará el modal.

• `Carousel`
```html
<div id="myCarousel" class="carousel slide" data-ride="carousel">

  <!-- Indicators -->
  <ul class="carousel-indicators">
    <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
    <li data-target="#myCarousel" data-slide-to="1"></li>
    <li data-target="#myCarousel" data-slide-to="2"></li>
  </ul>

  <!-- The slideshow -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="img1.jpg" alt="Image 1">
    </div>
    <div class="carousel-item">
      <img src="img2.jpg" alt="Image 2">
    </div>
    <div class="carousel-item">
      <img src="img3.jpg" alt="Image 3">
    </div>
  </div>

  <!-- Left and right controls -->
  <a class="carousel-control-prev" href="#myCarousel" data-slide="prev">
    <span class="carousel-control-prev-icon"></span>
  </a>
  <a class="carousel-control-next" href="#myCarousel" data-slide="next">
    <span class="carousel-control-next-icon"></span>
  </a>

</div>
```
En este ejemplo, se utiliza la clase "carousel" para crear el contenedor del carousel. Dentro de este contenedor, se establecen los indicadores y las imágenes a través de las clases "carousel-indicators" y "carousel-item". Además, se agregan los controles izquierdo y derecho a través de las clases "carousel-control-prev" y "carousel-control-next". El atributo "data-slide" se utiliza para desplazar las imágenes hacia la izquierda o hacia la derecha.

• `Navs`
```html
<ul class="nav nav-tabs">
  <li class="nav-item">
    <a class="nav-link active" href="#home">Home</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#about">About</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#services">Services</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#contact">Contact</a>
  </li>
</ul>
```
En este ejemplo, se utiliza la clase "nav" para crear la barra de navegación. Dentro de la barra de navegación, se establecen las pestañas mediante la clase "nav-tabs". Cada pestaña se crea utilizando la clase "nav-item" y un enlace que se crea utilizando la clase "nav-link". La pestaña activa se identifica mediante la clase "active".

• `Breadcrumbs`
```html
<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item"><a href="#">Library</a></li>
    <li class="breadcrumb-item active" aria-current="page">Data</li>
  </ol>
</nav>
```
En este ejemplo, se utiliza la clase "breadcrumb" para crear el breadcrumb. Dentro del breadcrumb, se establecen los enlaces a través de la clase "breadcrumb-item". El último ítem del breadcrumb se identifica mediante la clase "active" y se establece mediante el atributo "aria-current". La navegación es accesible para lectores de pantalla gracias al atributo "aria-label".

• `Pagination`
```html
<nav aria-label="Page navigation example">
  <ul class="pagination">
    <li class="page-item disabled">
      <a class="page-link" href="#" tabindex="-1" aria-disabled="true">Previous</a>
    </li>
    <li class="page-item"><a class="page-link" href="#">1</a></li>
    <li class="page-item"><a class="page-link" href="#">2</a></li>
    <li class="page-item"><a class="page-link" href="#">3</a></li>
    <li class="page-item">
      <a class="page-link" href="#">Next</a>
    </li>
  </ul>
</nav>
```
En este ejemplo, se utiliza la clase "pagination" para crear la paginación. Dentro de la paginación, se establecen los botones de página utilizando la clase "page-item" y los enlaces a través de la clase "page-link". El botón de página activa se identifica mediante la clase "active". El botón de "Previous" se deshabilita mediante la clase "disabled" y el atributo "aria-disabled". El atributo "aria-label" se utiliza para hacer la navegación accesible para lectores de pantalla.

• `Tooltips`
```html
<button type="button" class="btn btn-secondary" data-toggle="tooltip" data-placement="top" title="Tooltip on top">
  Tooltip on top
</button>
```
En este ejemplo, se utiliza la clase "btn" para crear un botón. El tooltip se establece utilizando los atributos "data-toggle", "data-placement" y "title". El atributo "data-toggle" establece que el elemento es un tooltip. El atributo "data-placement" establece la posición del tooltip (arriba, abajo, izquierda o derecha). El atributo "title" establece el texto del tooltip.

• `Formularios`
```html
<form>
  <div class="form-group">
    <label for="exampleFormControlInput1">Email address</label>
    <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="name@example.com">
  </div>
  <div class="form-group">
    <label for="exampleFormControlSelect1">Example select</label>
    <select class="form-control" id="exampleFormControlSelect1">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
  </div>
  <div class="form-group">
    <label for="exampleFormControlTextarea1">Example textarea</label>
    <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
  </div>
</form>
```
En este ejemplo, se utiliza la clase "form-group" para agrupar los elementos del formulario. Se utiliza la etiqueta "label" para establecer las etiquetas de los elementos del formulario. Los elementos del formulario se crean utilizando la clase "form-control". En este ejemplo, se utiliza un campo de correo electrónico, un campo de selección y un campo de texto.

• `Cards`
```html
<div class="card" style="width: 18rem;">
  <img src="..." class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```
En este ejemplo, se utiliza la clase "card" para crear la card. La imagen se establece mediante la clase "card-img-top". El contenido de la card se establece dentro de la clase "card-body". En este ejemplo, se establece un título de la card, texto y un botón. El tamaño de la card se establece mediante la clase "style".
