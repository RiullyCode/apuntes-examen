# EJERCICIO TEMA 5 EXPLICADO:

## `title`
El elemento semántico de HTML title se utiliza para definir el título del documento en la pestaña del navegador y también como un título en los resultados de búsqueda.

Aquí te dejo un ejemplo de cómo se utiliza:
```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Titulo de la Página</title>
</head>
<body>
  <h1>Este es un título principal</h1>
  <p>Este es un párrafo de ejemplo.</p>
</body>
</html>
```
En este ejemplo, el título del documento se establece en "Titulo de la Página". Este título se mostrará en la pestaña del navegador y en los resultados de búsqueda.

<image src="https://cdn.discordapp.com/attachments/914613587715182622/1081977998175117423/image.png" alt="Descripción de la imagen">

## `Main`
El elemento semántico HTML <main> se utiliza para representar el contenido principal de una página web. Este elemento debe contener todo el contenido central de la página, como los artículos, secciones, contenido relevante, etc.

Un ejemplo de cómo se puede utilizar el elemento <main> en una página web sería el siguiente:
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi página web</title>
  </head>
  <body>
    <header>
      <h1>Encabezado de la página</h1>
      <nav>
        <ul>
          <li><a href="#">Inicio</a></li>
          <li><a href="#">Acerca de</a></li>
          <li><a href="#">Contacto</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <section>
        <h2>Sección de noticias</h2>
        <article>
          <h3>Título de la noticia 1</h3>
          <p>Contenido de la noticia 1...</p>
        </article>
        <article>
          <h3>Título de la noticia 2</h3>
          <p>Contenido de la noticia 2...</p>
        </article>
      </section>
      <section>
        <h2>Sección de productos</h2>
        <article>
          <h3>Producto 1</h3>
          <p>Descripción del producto 1...</p>
        </article>
        <article>
          <h3>Producto 2</h3>
          <p>Descripción del producto 2...</p>
        </article>
      </section>
    </main>
    <footer>
      <p>Derechos de autor &copy; 2023</p>
    </footer>
  </body>
</html>


```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi página web</title>
  </head>
  <body>
    <header>
      <h1>Encabezado de la página</h1>
      <nav>
        <ul>
          <li><a href="#">Inicio</a></li>
          <li><a href="#">Acerca de</a></li>
          <li><a href="#">Contacto</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <section>
        <h2>Sección de noticias</h2>
        <article>
          <h3>Título de la noticia 1</h3>
          <p>Contenido de la noticia 1...</p>
        </article>
        <article>
          <h3>Título de la noticia 2</h3>
          <p>Contenido de la noticia 2...</p>
        </article>
      </section>
      <section>
        <h2>Sección de productos</h2>
        <article>
          <h3>Producto 1</h3>
          <p>Descripción del producto 1...</p>
        </article>
        <article>
          <h3>Producto 2</h3>
          <p>Descripción del producto 2...</p>
        </article>
      </section>
    </main>
    <footer>
      <p>Derechos de autor &copy; 2023</p>
    </footer>
  </body>
</html>
```
En este ejemplo, se utiliza el elemento <main> para encerrar todo el contenido principal de la página, como las secciones de noticias y productos. De esta manera, se le da un significado semántico al contenido de la página, lo que hace que sea más fácil de entender para los motores de búsqueda y para los usuarios que utilizan tecnologías de asistencia.

## `Section`
El elemento semántico <section> en HTML se utiliza para agrupar contenido relacionado y crear secciones temáticas en una página web. Proporciona información sobre el significado y la estructura del contenido, lo que ayuda a los motores de búsqueda y a otros programas a comprender mejor la organización y el contexto de la información presentada.

Un ejemplo de uso de <section> sería en una página web de noticias, donde se puede utilizar para dividir el contenido en secciones como "Noticias de última hora", "Política", "Deportes", "Entretenimiento", etc. Cada sección tendría su propio encabezado y contenido relacionado, lo que facilitaría la navegación y la comprensión de la información para los usuarios. Aquí te muestro un ejemplo de código HTML:

<section>
  <h2>Noticias de última hora</h2>
  <p>Contenido de noticias de última hora...</p>
</section>

<section>
  <h2>Política</h2>
  <p>Contenido de política...</p>
</section>

<section>
  <h2>Deportes</h2>
  <p>Contenido de deportes...</p>
</section>

<section>
  <h2>Entretenimiento</h2>
  <p>Contenido de entretenimiento...</p>
</section>


```html
<section>
  <h2>Noticias de última hora</h2>
  <p>Contenido de noticias de última hora...</p>
</section>

<section>
  <h2>Política</h2>
  <p>Contenido de política...</p>
</section>

<section>
  <h2>Deportes</h2>
  <p>Contenido de deportes...</p>
</section>

<section>
  <h2>Entretenimiento</h2>
  <p>Contenido de entretenimiento...</p>
</section>

```
En este ejemplo, se utilizan las etiquetas `<section>` para agrupar el contenido relacionado bajo diferentes secciones temáticas, cada una con su propio encabezado `(<h2>)` y párrafo `(<p>)`.

## ``` Formulario de Login```
Un formulario de login en HTML se utiliza para permitir que los usuarios ingresen a un sitio web o aplicación mediante la autenticación de sus credenciales (por ejemplo, nombre de usuario y contraseña). Este formulario es una parte esencial de muchos sitios web y aplicaciones que requieren autenticación para acceder a ciertos contenidos o funcionalidades.

Aquí te muestro un ejemplo básico de un formulario de login en HTML:
<form>
  <label for="username">Nombre de usuario:</label>
  <input type="text" id="username" name="username" required>

  <label for="password">Contraseña:</label>
  <input type="password" id="password" name="password" required>

  <input type="submit" value="Ingresar">
</form>

```html
<form>
  <label for="username">Nombre de usuario:</label>
  <input type="text" id="username" name="username" required>

  <label for="password">Contraseña:</label>
  <input type="password" id="password" name="password" required>

  <input type="submit" value="Ingresar">
</form>
```
En este ejemplo, el formulario contiene dos campos de entrada: uno para el nombre de usuario y otro para la contraseña. Ambos campos son obligatorios (required) para asegurarse de que el usuario complete ambos campos antes de enviar el formulario.

El botón "Ingresar" <input type="submit" value="Ingresar"> es el elemento que envía el formulario al servidor para su procesamiento. Al hacer clic en el botón, los valores ingresados en los campos se envían al servidor a través del método HTTP POST o GET, según lo especificado en el atributo method del formulario.

Es importante tener en cuenta que este es solo un ejemplo básico de un formulario de login. En la práctica, los formularios de login suelen ser más complejos y pueden incluir características adicionales, como la verificación de captcha, recordar el usuario, recuperación de contraseña, entre otros. Además, el procesamiento de la autenticación en el servidor generalmente implica el uso de tecnologías como PHP, Node.js o Ruby on Rails, entre otros.

## `Aside`
El elemento semántico `<aside>` en HTML se utiliza para definir contenido relacionado o complementario al contenido principal de una página web. Este contenido puede estar ubicado en un lateral o sección adyacente al contenido principal. Se utiliza para agregar información complementaria que no es esencial para la comprensión del contenido principal, pero que aún así puede ser útil para el usuario.

Un ejemplo de uso de `<aside>` sería en una página de blog, donde se puede utilizar para agregar información relacionada con el contenido principal, como enlaces a publicaciones relacionadas, información del autor, anuncios o widgets de redes sociales. Aquí te muestro un ejemplo de código HTML:
<main>
  <article>
    <h2>Título del artículo</h2>
    <p>Contenido del artículo...</p>
  </article>
</main>

<aside>
  <h3>Enlaces relacionados</h3>
  <ul>
    <li><a href="#">Artículo relacionado 1</a></li>
    <li><a href="#">Artículo relacionado 2</a></li>
    <li><a href="#">Artículo relacionado 3</a></li>
  </ul>

  <h3>Redes sociales</h3>
  <ul>
    <li><a href="#">Facebook</a></li>
    <li><a href="#">Twitter</a></li>
    <li><a href="#">Instagram</a></li>
  </ul>
</aside>

```html
<main>
  <article>
    <h2>Título del artículo</h2>
    <p>Contenido del artículo...</p>
  </article>
</main>

<aside>
  <h3>Enlaces relacionados</h3>
  <ul>
    <li><a href="#">Artículo relacionado 1</a></li>
    <li><a href="#">Artículo relacionado 2</a></li>
    <li><a href="#">Artículo relacionado 3</a></li>
  </ul>

  <h3>Redes sociales</h3>
  <ul>
    <li><a href="#">Facebook</a></li>
    <li><a href="#">Twitter</a></li>
    <li><a href="#">Instagram</a></li>
  </ul>
</aside>

```
En este ejemplo, se utiliza la etiqueta `<aside>` para agrupar contenido relacionado o complementario al contenido principal. En este caso, el contenido principal está dentro de la etiqueta `<main>` y se refiere al artículo en sí, mientras que el `<aside>` contiene enlaces relacionados y enlaces a las redes sociales del sitio. Cada sección de contenido relacionado tiene su propio encabezado `(<h3>)` y contenido `(<ul>)`.

## `Table`

El elemento semántico `<table>` en HTML se utiliza para crear una tabla de datos. Las tablas se utilizan a menudo para organizar y mostrar datos de una manera clara y fácil de entender. El contenido de una tabla se divide en filas `<tr>` y columnas `<td>`, y puede incluir encabezados de columna `<th>`.

Aquí te muestro un ejemplo básico de cómo se crea una tabla en HTML:
<table>
  <thead>
    <tr>
      <th>Nombre</th>
      <th>Edad</th>
      <th>País</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Juan</td>
      <td>32</td>
      <td>Argentina</td>
    </tr>
    <tr>
      <td>María</td>
      <td>27</td>
      <td>México</td>
    </tr>
    <tr>
      <td>Pedro</td>
      <td>45</td>
      <td>Chile</td>
    </tr>
  </tbody>
</table>

 ```html
<table>
  <thead>
    <tr>
      <th>Nombre</th>
      <th>Edad</th>
      <th>País</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Juan</td>
      <td>32</td>
      <td>Argentina</td>
    </tr>
    <tr>
      <td>María</td>
      <td>27</td>
      <td>México</td>
    </tr>
    <tr>
      <td>Pedro</td>
      <td>45</td>
      <td>Chile</td>
    </tr>
  </tbody>
</table>

 ```
En este ejemplo, se crea una tabla con tres columnas: Nombre, Edad y País. La primera fila de la tabla se utiliza como encabezado de columna `<thead>`, mientras que el resto de las filas se encuentran en el cuerpo de la tabla `<tbody>`. Cada fila de la tabla `<tr>` contiene tres celdas `<td>`, una para cada columna.

Es importante tener en cuenta que el uso de tablas para diseñar el diseño visual de un sitio web se considera una mala práctica. Las tablas deben utilizarse solo para presentar datos de una manera organizada y semántica. Si se desea crear diseños más complejos, se recomienda utilizar otras técnicas de diseño, como CSS.

## `Mark`
El elemento semántico `<mark>` en HTML se utiliza para resaltar o marcar un fragmento de texto dentro de un documento web. Es útil para señalar partes importantes de un texto o para resaltar información específica para el usuario.

Aquí te muestro un ejemplo de cómo se utiliza el elemento `<mark>` en HTML:
<p>La <mark>luna</mark> es el único satélite natural de la Tierra.</p>

```html
<p>La <mark>luna</mark> es el único satélite natural de la Tierra.</p>

```
En este ejemplo, el texto "luna" se marca o resalta utilizando la etiqueta `<mark>`. Esto hace que el texto se destaque del resto del contenido, lo que puede ayudar a que el lector se centre en la información más importante o relevante.

También es posible utilizar el elemento `<mark>` para resaltar varias palabras o frases dentro de un mismo párrafo o sección de texto:
<p>El <mark>clima</mark> en esta región es <mark>cálido</mark> y <mark>húmedo</mark> durante la mayor parte del año.</p>

```html
<p>El <mark>clima</mark> en esta región es <mark>cálido</mark> y <mark>húmedo</mark> durante la mayor parte del año.</p>
```
En este ejemplo, se resaltan tres palabras diferentes utilizando la etiqueta `<mark>`. Cada palabra se destaca de forma individual, lo que puede ayudar al lector a identificar rápidamente los aspectos más importantes de la descripción del clima en esta región.

## `Video`
El elemento `<video>` en HTML se utiliza para insertar un archivo de vídeo en una página web. El uso de vídeos en HTML es una forma efectiva de añadir contenido multimedia a un sitio web, lo que puede mejorar la experiencia del usuario y aumentar el interés y la participación del visitante.

La sintaxis básica del elemento `<video>` es la siguiente:
<video src="https://www.youtube.com/watch?v=GuZzuQvv7uc&ab_channel=chayanneVEVO" controls>
  Tu navegador no admite la reproducción de videos.
</video>

```html
<video src="https://www.youtube.com/watch?v=GuZzuQvv7uc&ab_channel=chayanneVEVO" controls>
  Tu navegador no admite la reproducción de videos.
</video>
```
En este ejemplo, se utiliza la etiqueta `<video>` para insertar un archivo de vídeo en la página web. El atributo src se utiliza para especificar la ruta o URL del archivo de vídeo que se desea mostrar. El atributo controls se utiliza para mostrar los controles de reproducción estándar del navegador web, como el botón de reproducción, pausa y volumen.

El texto "Tu navegador no admite la reproducción de videos." se mostrará en el caso de que el navegador del usuario no admita la reproducción de videos HTML5.

Además del atributo src y controls, existen otros atributos que se pueden utilizar con el elemento `<video>`, como autoplay para reproducir el video automáticamente cuando se carga la página, loop para hacer que el video se repita continuamente y poster para mostrar una imagen de portada antes de que se inicie la reproducción del video.

También se pueden especificar varios formatos de archivo de vídeo en el atributo src para garantizar la compatibilidad con diferentes navegadores web. Por ejemplo:

<video controls>
  <source src="ruta-del-archivo.mp4" type="video/mp4">
  <source src="ruta-del-archivo.webm" type="video/webm">
  Tu navegador no admite la reproducción de videos.
</video>

```html
<video controls>
  <source src="ruta-del-archivo.mp4" type="video/mp4">
  <source src="ruta-del-archivo.webm" type="video/webm">
  Tu navegador no admite la reproducción de videos.
</video>
```
En este ejemplo, se utiliza la etiqueta <source> para especificar dos formatos diferentes de archivo de video: MP4 y WebM. El navegador del usuario seleccionará automáticamente el formato que mejor se adapte a su dispositivo y software. Si el navegador no admite la reproducción de videos HTML5, se mostrará el texto de reemplazo "Tu navegador no admite la reproducción de videos."

## `Mapa`
Para insertar un mapa en una página web HTML, entras en google maps y buscas una ubicación.

Le das a `compartir` -> `insertar en un mapa` y `copiar html`
```html
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d46405.723452683116!2d-5.883677172536517!3d43.36954390222433!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xd368c9a60ac1c67%3A0x3134440ecc5e6224!2sOviedo%2C%20Asturias!5e0!3m2!1ses!2ses!4v1678035713683!5m2!1ses!2ses" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
```

## `footer`
En HTML, un "footer" es una sección que se coloca al final del contenido de una página web, que generalmente contiene información adicional como enlaces importantes, información de contacto, derechos de autor, etc. El footer es una parte importante de una página web, ya que proporciona información relevante y útil para los visitantes del sitio web.

Aquí te proporciono un ejemplo básico de cómo crear un footer en HTML:
<footer>
  <div class="container">
    <div class="row">
      <div class="col-sm-6">
        <h4>Información de contacto</h4>
        <p>Dirección: 1234 Calle Principal, Ciudad, País</p>
        <p>Teléfono: +1 234 567 890</p>
        <p>Email: info@ejemplo.com</p>
      </div>
      <div class="col-sm-6">
        <h4>Enlaces útiles</h4>
        <ul>
          <li><a href="#">Inicio</a></li>
          <li><a href="#">Acerca de nosotros</a></li>
          <li><a href="#">Servicios</a></li>
          <li><a href="#">Contacto</a></li>
        </ul>
      </div>
    </div>
    <hr>
    <p class="text-center">Derechos de autor &copy; 2023 Ejemplo.com</p>
  </div>
</footer>

 ```html
<footer>
  <div class="container">
    <div class="row">
      <div class="col-sm-6">
        <h4>Información de contacto</h4>
        <p>Dirección: 1234 Calle Principal, Ciudad, País</p>
        <p>Teléfono: +1 234 567 890</p>
        <p>Email: info@ejemplo.com</p>
      </div>
      <div class="col-sm-6">
        <h4>Enlaces útiles</h4>
        <ul>
          <li><a href="#">Inicio</a></li>
          <li><a href="#">Acerca de nosotros</a></li>
          <li><a href="#">Servicios</a></li>
          <li><a href="#">Contacto</a></li>
        </ul>
      </div>
    </div>
    <hr>
    <p class="text-center">Derechos de autor &copy; 2023 Ejemplo.com</p>
  </div>
</footer>
 ```
 En este ejemplo, se crea un footer que contiene dos secciones: una sección de información de contacto y una sección de enlaces útiles. La información de contacto incluye la dirección, el teléfono y el correo electrónico de la empresa. Los enlaces útiles incluyen los enlaces a las secciones importantes del sitio web. Al final del footer, se muestra un texto con los derechos de autor del sitio web.

El footer se crea utilizando la etiqueta <footer>, y se divide en dos secciones utilizando las clases de Bootstrap "col-sm-6". También se agrega un borde horizontal utilizando la etiqueta <hr>. En la última línea del footer, se muestra un texto con los derechos de autor utilizando la etiqueta <p> y la clase de Bootstrap "text-center".
