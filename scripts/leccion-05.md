# Lección 5: Crear una página web sencilla

## Combinar HTML y CSS para crear un perfil personal

HTML y CSS son dos herramientas fundamentales para construir una página web. HTML permite organizar el contenido, como los títulos, párrafos, listas y enlaces. CSS permite cambiar su apariencia, por ejemplo, los colores, tamaños de texto, espacios, bordes y alineación.

En esta lección combinaremos lo aprendido anteriormente para crear una página de perfil personal que incluya una presentación, una lista de hobbies y una lista de metas.

## Ejemplo del funcionamiento de HTML y CSS

Para empezar, ingrese a CodeSandbox: https://codesandbox.io/dashboard

Luego, cree un proyecto con la plantilla **HTML + CSS** o abra los archivos iniciales de esta lección. Trabajaremos con dos archivos: `index.html`, donde colocaremos el contenido, y `styles.css`, donde definiremos los estilos.

Primero, dentro de la etiqueta `<head>` del archivo `index.html`, verifique que el título de la pestaña y la hoja de estilos estén configurados de esta manera:

```html
<title>Mi perfil personal</title>
<link rel="stylesheet" href="styles.css" />
```

Después, dentro de `<body>`, cree un contenedor principal y un encabezado con su nombre, como en el siguiente ejemplo:

```html
<div class="page">
    <header class="site-header">
        <p>MI ESPACIO EN LA WEB</p>
        <h1>¡Hola! Soy Alex</h1>
        <p>Estudiante y amante de la creatividad</p>
    </header>
</div>
```

La etiqueta `<header>` agrupa el contenido introductorio de la página. La etiqueta `<h1>` define el título principal y `<p>` permite escribir párrafos. El atributo `class` asigna un nombre que luego podremos utilizar para aplicar estilos con CSS.

A continuación, dentro del contenedor, agregue una sección para presentarse. Incluya un subtítulo, una breve descripción y un enlace que lleve a la sección de hobbies:

```html
<main>
    <section class="profile-card">
        <h2>Sobre mí</h2>
        <p>Me gusta aprender cosas nuevas y crear proyectos.</p>
        <a class="profile-link" href="#hobbies">Conoce mis hobbies</a>
    </section>
</main>
```

La etiqueta `<main>` identifica el contenido principal de la página, mientras que `<section>` agrupa contenido relacionado. La etiqueta `<h2>` crea un subtítulo y `<a>` permite crear un enlace. En este caso, `href="#hobbies"` indica que el enlace llevará al elemento que tenga `id="hobbies"`.

Ahora, debajo de la tarjeta de presentación, cree la sección de hobbies con una lista desordenada y una sección de metas con una lista ordenada:

```html
<section class="content-section" id="hobbies">
    <h2>Mis hobbies</h2>
    <ul>
        <li>Dibujar</li>
        <li>Jugar videojuegos</li>
        <li>Escuchar música</li>
    </ul>
</section>

<section class="content-section">
    <h2>Mis metas</h2>
    <ol>
        <li>Aprender a crear páginas web.</li>
        <li>Practicar HTML y CSS.</li>
        <li>Compartir mis proyectos.</li>
    </ol>
</section>
```

La etiqueta `<ul>` crea una lista con viñetas, mientras que `<ol>` crea una lista numerada. Cada elemento de ambas listas se coloca dentro de `<li>`. Observa también que la sección de hobbies tiene `id="hobbies"`, que coincide con el destino del enlace anterior.

Finalmente, antes de cerrar el contenedor principal, agregue un pie de página:

```html
<footer class="site-footer">
    <p>Hecho por Alex | Mi primera página personal</p>
</footer>
```

La etiqueta `<footer>` contiene información final, como el autor o una nota sobre la página. Con esto, la estructura HTML estará lista.

## Agregar estilos con CSS

Ahora, abra el archivo `styles.css`. Para comenzar, podemos definir el tipo de letra, el color del texto y el fondo general de la página:

```css
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background-color: #f1f5f9;
    color: #253047;
    line-height: 1.6;
}
```

La propiedad `background-color` cambia el fondo, `font-family` define la tipografía y `line-height` controla la separación entre líneas. La propiedad `margin: 0` elimina el margen predeterminado del navegador.

Luego, utilice las clases que agregó al HTML para diseñar el encabezado y las secciones:

```css
.page {
    width: 90%;
    max-width: 850px;
    margin: 0 auto;
    padding: 32px 0;
}

.site-header {
    background-color: #dbeafe;
    text-align: center;
    padding: 32px 20px;
    border-radius: 16px;
    margin-bottom: 24px;
}

.profile-card,
.content-section {
    background-color: #ffffff;
    padding: 24px;
    border-radius: 14px;
    margin-bottom: 20px;
}

h1,
h2 {
    color: #1e3a8a;
}
```

El selector `.page` permite centrar y limitar el ancho del contenido. El punto delante de `site-header` o `profile-card` indica que se trata de una clase CSS. Las propiedades `padding`, `margin-bottom` y `border-radius` agregan espacio interno, separación entre elementos y esquinas redondeadas, respectivamente.

Para que el enlace destaque, agregue la siguiente regla:

```css
.profile-link {
    display: inline-block;
    background-color: #2563eb;
    color: #ffffff;
    text-decoration: none;
    padding: 10px 16px;
    border-radius: 8px;
}
```

Por último, centre el pie de página y utilice un color de texto más suave:

```css
.site-footer {
    text-align: center;
    color: #64748b;
    font-size: 14px;
    padding: 10px;
}
```

Estas reglas muestran cómo una misma página puede organizarse primero con HTML y después personalizarse con CSS. En los archivos de ejemplo resueltos de esta lección encontrará el código completo del perfil personal, incluidos los estilos adicionales.

## Resultado esperado

Si hizo todo esto, la página mostrará un perfil personal con un encabezado azul claro y un título principal, una sección de presentación con un enlace, una lista de hobbies con viñetas, una lista numerada de metas y un pie de página. El contenido estará centrado y tendrá fondos claros, espacios y esquinas redondeadas.

Al seleccionar el enlace **Conoce mis hobbies**, el navegador deberá desplazarse hasta la lista de hobbies.

## Actividad práctica

Personalice el perfil siguiendo estos pasos:

1. Cambie el nombre “Alex” por su propio nombre.
2. Modifique el párrafo de presentación.
3. Reemplace los hobbies y las metas por ejemplos propios.
4. Cambie el color de fondo del encabezado y observe el resultado.
5. Compruebe que el enlace lleva a la sección de hobbies.

## Puntos clave

Como puntos clave de esta lección, podemos destacar que:

- HTML permite organizar el contenido de una página mediante encabezados, párrafos, secciones, listas y enlaces.
- CSS permite personalizar la apariencia usando colores, tipografías, márgenes, espacios internos y bordes.
- El atributo `class` conecta elementos HTML con reglas CSS que comienzan con un punto, como `.site-header`.
- Las listas `<ul>` muestran viñetas y las listas `<ol>` muestran una secuencia numerada; sus elementos se definen con `<li>`.
- Un enlace con `href="#hobbies"` puede llevar a una sección de la misma página que tenga `id="hobbies"`.

## Conclusión

En conclusión, en esta lección aprendimos a combinar HTML y CSS para crear una página de perfil personal. Con HTML organizamos la información en secciones, títulos, párrafos y listas; con CSS mejoramos la presentación mediante colores, espacios, alineación y bordes.

Al combinar ambos lenguajes podemos construir páginas web más claras, ordenadas y atractivas. Como práctica final, se recomienda personalizar el perfil con información propia y comprobar que todos sus enlaces funcionen correctamente.
