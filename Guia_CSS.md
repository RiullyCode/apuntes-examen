# Guía CSS básico y avanzado

## `Como centrar contenido en el navegador`
Para centrar un div en el centro de la página, puedes utilizar la propiedad margin junto con la propiedad display en CSS. Aquí te muestro un ejemplo:
```html
<div class="centrado">
  <h1>Contenido centrado</h1>
  <p>Este es el contenido que deseamos centrar.</p>
</div>
```
```css
.centrado {
  width: 50%; /* Ancho del div */
  height: 50%; /* Altura del div */
  margin: auto; /* Centra el div horizontalmente y verticalmente */
  display: flex; /* Crea un contenedor flexible */
  justify-content: center; /* Centra el contenido horizontalmente */
  align-items: center; /* Centra el contenido verticalmente */
}
```
En este ejemplo, width y height definen el tamaño del div. La propiedad margin con valor auto centra el div horizontalmente y verticalmente. La propiedad display con valor flex crea un contenedor flexible que te permite centrar el contenido dentro del div. La propiedad justify-content con valor center centra el contenido horizontalmente, mientras que la propiedad align-items con valor center centra el contenido verticalmente.

Es importante tener en cuenta que, al utilizar la propiedad display: flex, algunos navegadores pueden requerir la propiedad display: -webkit-flex; para asegurarse de que se muestre correctamente.

## `Como hacer que una web sea responsive en cuanto al navegador`
Para hacer que una web sea responsive en cuanto al navegador, debes utilizar técnicas de diseño responsivo en CSS. A continuación, te mostraré algunas técnicas básicas y avanzadas que puedes utilizar para hacer que tu web sea responsive:

Utiliza unidades de medida relativas:
En lugar de utilizar unidades de medida fijas como píxeles, utiliza unidades de medida relativas como porcentajes, ems o rems. Por ejemplo:

```css
.contenedor {
  width: 80%; /* Ancho del contenedor en porcentaje */
  font-size: 1em; /* Tamaño de fuente en ems */
}
```
Esto asegura que la web se adapte al tamaño del navegador y se ajuste automáticamente al tamaño de la pantalla.

Utiliza la propiedad max-width para limitar el ancho de los elementos:
Puedes utilizar la propiedad max-width para limitar el ancho de los elementos. Por ejemplo:

```css
.imagen {
  max-width: 100%; /* Ancho máximo de la imagen */
  height: auto; /* Altura automática de la imagen */
}
```
Utiliza Flexbox o Grid para un diseño más avanzado:
Flexbox y Grid son técnicas avanzadas de diseño responsivo que te permiten crear diseños complejos y adaptables a diferentes tamaños de pantalla. Por ejemplo:
```css
.contenedor {
  display: flex; /* Crea un contenedor flexible */
  flex-wrap: wrap; /* Ajusta el contenido a la pantalla */
  justify-content: space-between; /* Espacio entre los elementos */
  align-items: center; /* Centra verticalmente los elementos */
}

.item {
  flex: 1 0 calc(33.333% - 20px); /* Ancho del item */
  margin-bottom: 20px; /* Margen inferior del item */
}
```
En este ejemplo, el contenedor utiliza Flexbox para ajustar el contenido a la pantalla, mientras que los elementos utilizan una fórmula de ancho flexible para adaptarse a diferentes tamaños de pantalla.

En resumen, para hacer que una web sea responsive en cuanto al navegador, debes utilizar unidades de medida relativas, limitar el ancho de los elementos, utilizar media queries y técnicas avanzadas de diseño responsivo como Flexbox o Grid.

## `Como Utilizar fuentes de texto personalizadas`

Si quieres aplicar por ejemplo una fuente genérica como sans-serif a tu sitio web, simplemente debes utilizar la propiedad font-family en tus estilos CSS. Por ejemplo, para aplicar sans-serif al cuerpo de tu sitio, puedes hacer lo siguiente:
```css
body {
  font-family: sans-serif;
}
```
Esta propiedad establece la fuente genérica sans-serif como la fuente predeterminada para todo el contenido dentro del elemento body. Ten en cuenta que sans-serif es una fuente genérica que se utiliza como un respaldo en caso de que la fuente principal no se cargue correctamente. Si deseas utilizar una fuente personalizada en su lugar, debes seguir los pasos que mencioné anteriormente para cargar y utilizar una fuente personalizada en tu sitio web.

## `Como hacer 3 media querys para que el tamaño cambie en función del tamaño del navegador (por ejemplo más 1000px, entre 600px y 1000px y menos de 600px.` 
Para crear 3 media queries para que el tamaño cambie en función del tamaño del navegador, puedes utilizar las siguientes reglas CSS:
```css
/* Media query para pantallas grandes de más de 1000px */
@media (min-width: 1000px) {
  /* Aquí puedes agregar los estilos que deseas aplicar a la página cuando el ancho de la pantalla sea mayor a 1000px */
}

/* Media query para pantallas medianas entre 600px y 1000px */
@media (min-width: 600px) and (max-width: 999px) {
  /* Aquí puedes agregar los estilos que deseas aplicar a la página cuando el ancho de la pantalla esté entre 600px y 999px */
}

/* Media query para pantallas pequeñas de menos de 600px */
@media (max-width: 599px) {
  /* Aquí puedes agregar los estilos que deseas aplicar a la página cuando el ancho de la pantalla sea menor a 600px */
}
```
Cada media query utiliza la propiedad @media para definir un conjunto de estilos CSS que se aplicarán solo si se cumple la condición especificada en la regla. En este caso, se especifica el ancho mínimo o máximo de la pantalla utilizando las propiedades min-width y max-width en píxeles.

Dentro de cada media query, puedes agregar los estilos CSS que deseas aplicar a la página cuando se cumple la condición especificada. Por ejemplo, puedes cambiar el tamaño de la fuente, el ancho de los elementos o la disposición de los elementos en función del tamaño de la pantalla.

Al utilizar estos tres media queries, podrás crear un sitio web responsive que se adapte a diferentes tamaños de pantalla.

## `Como poner una imagen fija y que cubra todo el fondo del navegador.`
Puedes establecer una imagen de fondo que cubra todo el fondo del navegador utilizando la propiedad background de CSS. Para hacer esto, sigue estos pasos:

Agrega una imagen a tu sitio web, ya sea utilizando la etiqueta img en tu HTML o utilizando una URL en tus estilos CSS. Por ejemplo:
```css
body {
  background-image: url("mi-imagen.jpg");
}
```
Asegúrate de que la imagen sea lo suficientemente grande para cubrir todo el fondo del navegador. Puedes utilizar una imagen de alta resolución o ajustar la imagen con un editor de imágenes.

Utiliza la propiedad background-size para hacer que la imagen se ajuste al tamaño de la pantalla. Establece el valor a cover para hacer que la imagen cubra todo el fondo.

Utiliza la propiedad background-attachment para fijar la imagen en su lugar. Establece el valor a fixed para que la imagen permanezca en su lugar mientras se desplaza por la página.

El siguiente ejemplo muestra cómo puedes utilizar estas propiedades para establecer una imagen de fondo fija que cubra todo el fondo del navegador:

```css
body {
  background-image: url("mi-imagen.jpg");
  background-size: cover;
  background-attachment: fixed;
}
```

Con estas propiedades CSS, la imagen de fondo se ajustará automáticamente al tamaño de la pantalla y se fijará en su lugar, creando un efecto de imagen fija que cubre todo el fondo del navegador.

## `Como hacer una transición en css`
Para crear una transición en CSS, sigue estos pasos:

Selecciona el elemento al que deseas agregar la transición. Puede ser cualquier elemento, como un botón, un enlace, una imagen o un cuadro de texto.

Agrega la propiedad transition a tu CSS. Esta propiedad especifica qué propiedad CSS se animará y cuánto tiempo durará la animación. Por ejemplo, puedes utilizar la propiedad transition para animar el color de fondo de un botón durante 0.5 segundos:
```css
button {
  background-color: red;
  transition: background-color 0.5s;
}
```
En este ejemplo, la propiedad transition se utiliza para animar la propiedad background-color durante 0.5 segundos.

Cambia el valor de la propiedad CSS que deseas animar. Por ejemplo, puedes cambiar el color de fondo de un botón al pasar el cursor sobre él:
```css
button:hover {
  background-color: blue;
}
```
En este ejemplo, la propiedad :hover se utiliza para cambiar el color de fondo del botón cuando se pasa el cursor sobre él.

Con estos pasos, tendrás una transición suave que anima el color de fondo del botón durante 0.5 segundos cuando el usuario pasa el cursor sobre él. Puedes ajustar la duración de la transición y la propiedad CSS que se animará para crear diferentes efectos de animación.

También puedes utilizar otras propiedades de la transición, como transition-delay para especificar un retraso antes de que la transición comience o transition-timing-function para especificar una función de temporización para la transición.

## `como hacer en css selectores de tipo etiqueta, clase, identificador, descendiente y de tipo hijo.`
Los selectores en CSS son patrones que se utilizan para seleccionar los elementos HTML que se desean estilizar. Aquí te explico algunos de los selectores más comunes en CSS:

`Selector de tipo etiqueta`: Selecciona todos los elementos con un tipo de etiqueta específico. Por ejemplo, p selecciona todos los párrafos.

`Selector de clase:` Selecciona todos los elementos que tienen un atributo class específico. El selector de clase comienza con un punto (.) seguido del nombre de la clase. Por ejemplo, .boton selecciona todos los elementos que tienen la clase "boton".

`Selector de identificador:` Selecciona un elemento específico que tiene un atributo id. El selector de identificador comienza con un signo de numeral (#) seguido del nombre del identificador. Por ejemplo, #encabezado selecciona el elemento con el identificador "encabezado".

`Selector descendiente:` Selecciona un elemento que es descendiente de otro elemento específico. El selector descendiente utiliza un espacio para separar los nombres de las etiquetas. Por ejemplo, div p selecciona todos los párrafos que son descendientes de un elemento div.

`Selector de tipo hijo:` Selecciona un elemento que es un hijo directo de otro elemento específico. El selector de tipo hijo utiliza el símbolo > para separar los nombres de las etiquetas. Por ejemplo, div > p selecciona todos los párrafos que son hijos directos de un elemento div.

A continuación, te muestro un ejemplo de cómo se utiliza cada uno de estos selectores:

```css
/* Selector de tipo etiqueta */
p {
  color: red;
}

/* Selector de clase */
.boton {
  background-color: blue;
}

/* Selector de identificador */
#encabezado {
  font-size: 24px;
}

/* Selector descendiente */
div p {
  font-style: italic;
}

/* Selector de tipo hijo */
div > p {
  font-weight: bold;
}
```

## `Como usar pseudoclases`
Las pseudoclases en CSS se utilizan para aplicar estilos a elementos HTML en diferentes estados o situaciones específicas. A continuación, te muestro algunos ejemplos de pseudoclases comunes y cómo utilizarlos en CSS:

Pseudoclase `:hover:` Se utiliza para aplicar un estilo a un elemento cuando se pasa el cursor sobre él. Por ejemplo:
```css
button:hover {
  background-color: red;
}
```

Pseudoclase `:focus:` Se utiliza para aplicar un estilo a un elemento cuando está siendo enfocado, como cuando se selecciona un campo de entrada de texto. Por ejemplo:
```css
input:focus {
  border: 2px solid blue;
}
```

Pseudoclase `:active:` Se utiliza para aplicar un estilo a un elemento cuando se hace clic sobre él. Por ejemplo:
```css
button:active {
  background-color: green;
}
```

Pseudoclase `:first-child:` Se utiliza para aplicar un estilo al primer elemento hijo de otro elemento. Por ejemplo:
```css
ul li:first-child {
  font-weight: bold;
}
```

Pseudoclase `:last-child:` Se utiliza para aplicar un estilo al último elemento hijo de otro elemento. Por ejemplo:
```css
ul li:last-child {
  color: gray;
}
```

Pseudoclase `:nth-child():` Se utiliza para aplicar un estilo a elementos específicos en una lista. Por ejemplo, el siguiente código selecciona el primer, segundo y tercer elemento en una lista:

```css
ul li:nth-child(1),
ul li:nth-child(2),
ul li:nth-child(3) {
  font-size: 20px;
}
```
Pseudoclase `:nth-of-type():` Se utiliza para aplicar un estilo a elementos específicos de un tipo de elemento específico. Por ejemplo, el siguiente código selecciona el primer y segundo párrafo de una página:
```css
p:nth-of-type(1),
p:nth-of-type(2) {
  color: blue;
}
```
Estas son solo algunas de las pseudoclases disponibles en CSS. Puedes utilizar pseudoclases para crear estilos únicos para diferentes estados y situaciones específicas en tu sitio web.

## `Como hacer que el menú debe cambiar de vertical a horizontal, vertical en pantalla pequeña y horizontal en pantalla grande.`

Para hacer que el menú cambie de vertical a horizontal en función del tamaño de la pantalla, puedes utilizar media queries y flexbox en CSS. El siguiente ejemplo muestra cómo hacerlo:
```html
<nav>
  <ul>
    <li><a href="#">Inicio</a></li>
    <li><a href="#">Nosotros</a></li>
    <li><a href="#">Servicios</a></li>
    <li><a href="#">Contacto</a></li>
  </ul>
</nav>
```
```css
/* Estilos para el menú */
nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

nav li {
  display: block;
}

nav a {
  display: block;
  padding: 10px;
  color: #fff;
  background-color: #333;
  text-decoration: none;
}

/* Media queries para cambiar el menú de vertical a horizontal */
@media screen and (min-width: 600px) {
  nav {
    display: flex;
    justify-content: center;
  }

  nav ul {
    flex-direction: row;
  }

  nav li {
    display: inline-block;
    margin: 0 10px;
  }
}
```
En este ejemplo, el menú se muestra en formato vertical en pantallas más pequeñas y en formato horizontal en pantallas más grandes. Los estilos iniciales se aplican a los elementos ul, li y a del menú. Luego, utilizamos media queries para aplicar estilos adicionales en pantallas más grandes.

En la media query, configuramos el nav para que se muestre como un contenedor flexible (display: flex) y centrado horizontalmente (justify-content: center). A continuación, establecemos flex-direction: row en ul para cambiar la dirección de los elementos hijos de vertical a horizontal. Finalmente, establecemos los elementos li como elementos inline-block y agregamos un margen de 10px para que se separen entre sí. Con estos estilos, el menú se mostrará horizontalmente en pantallas más grandes y verticalmente en pantallas más pequeñas.

## `Como hacer que en las secciones que tengamos dos noticias se posicionen en vertical en dispositivos pequeños y en paralelo en dispositivos grandes.`

Para hacer que las secciones con dos noticias se posicionen en vertical en dispositivos pequeños y en paralelo en dispositivos grandes, podemos utilizar media queries y flexbox en CSS. El siguiente ejemplo muestra cómo hacerlo:
```html
<section class="news-section">
  <div class="news-item">
    <h2>Noticia 1</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
  </div>
  <div class="news-item">
    <h2>Noticia 2</h2>
    <p>Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
  </div>
</section>
```
```css
/* Estilos para la sección de noticias */
.news-section {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.news-item {
  width: 48%;
  padding: 10px;
  background-color: #f9f9f9;
  border: 1px solid #ccc;
}

.news-item h2 {
  margin-top: 0;
}

/* Media queries para cambiar la posición de las noticias */
@media screen and (max-width: 600px) {
  .news-section {
    flex-direction: column;
  }

  .news-item {
    width: 100%;
    margin-bottom: 20px;
  }
}
```
En este ejemplo, se utiliza flexbox para mostrar las noticias en paralelo en pantallas más grandes y en vertical en pantallas más pequeñas. Los estilos iniciales se aplican a los elementos .news-section y .news-item. Luego, utilizamos media queries para aplicar estilos adicionales en pantallas más pequeñas.

En la media query, configuramos .news-section para que se muestre en una columna (flex-direction: column) en pantallas más pequeñas. A continuación, establecemos el ancho de .news-item en 100% para que ocupe todo el ancho de la pantalla y agregamos un margen inferior de 20px para separar las noticias. Con estos estilos, las noticias se mostrarán en vertical en pantallas más pequeñas y en paralelo en pantallas más grandes.





