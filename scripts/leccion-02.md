# Lección 2: Introducción a HTML

En esta lección aprenderás a reconocer la estructura básica de un documento HTML y a utilizar etiquetas para agregar títulos y párrafos. También crearás un proyecto nuevo en CodeSandbox y comprobarás cómo el navegador interpreta el código.

## ¿Qué es una etiqueta HTML?

HTML utiliza etiquetas para identificar y organizar los elementos de una página web. Muchas etiquetas tienen una etiqueta de apertura y otra de cierre. El cierre se reconoce porque incluye una barra diagonal (`/`) antes del nombre.

Por ejemplo:

```html
<h1>Mi primer título</h1>
<p>Este es mi primer párrafo.</p>
```

En este ejemplo:

- `<h1>` abre un título principal y `</h1>` lo cierra.
- `<p>` abre un párrafo y `</p>` lo cierra.
- El texto que se encuentra entre ambas etiquetas es el contenido del elemento.

## ¿Cómo se organiza un documento HTML?

Un documento HTML tiene una estructura básica que permite al navegador interpretar su contenido.

- `<!DOCTYPE html>` indica que el documento utiliza HTML5.
- `<html>` es el elemento raíz y contiene el documento.
- `<head>` reúne información y configuraciones del documento que no forman parte del contenido principal visible.
- `<title>` define el nombre que aparece en la pestaña del navegador.
- `<body>` contiene el contenido que se muestra dentro de la página, como títulos y párrafos.

## Etiquetas básicas: títulos y párrafos

En esta lección utilizaremos principalmente dos etiquetas:

- **`<h1>`:** representa el título principal del contenido.
- **`<p>`:** representa un párrafo de texto.

Ejemplo:

```html
<h1>Mi primera página</h1>
<p>Estoy aprendiendo a crear páginas web con HTML.</p>
```

El navegador interpreta las etiquetas y muestra el título y el párrafo con su formato predeterminado.

## Crear un proyecto en CodeSandbox

1. Ingresa a [CodeSandbox](https://codesandbox.io/dashboard) e inicia sesión.
2. Selecciona **Create**.
3. Elige la plantilla **HTML + CSS**.
4. Asigna un nombre al proyecto, por ejemplo: `Mi primera página HTML`.
5. Crea el proyecto y espera a que aparezca el editor.
6. En el explorador de archivos, abre `index.html`.
7. Mantén visible el panel **Preview** para observar el resultado.

El proyecto incluye `index.html` para el contenido HTML y `styles.css` para los estilos CSS. En esta lección trabajaremos principalmente en `index.html`.

## Ejemplo práctico: nuestra primera página

Dentro de `index.html`, utiliza la estructura completa del archivo que aparece en `starter_files/index.html`. En la sección `<body>`, agrega un título y un párrafo:

```html
<h1>¡Hola, mundo!</h1>
<p>Estoy aprendiendo HTML.</p>
```

El archivo `index.html` debe contener la estructura del documento, incluyendo las secciones `<head>` y `<body>`. La conexión con `styles.css` se deja preparada, aunque en esta lección no será necesario modificar los estilos.

## Resultado esperado

Al guardar o actualizar el proyecto, el panel **Preview** debe mostrar:

- Un título principal que dice **¡Hola, mundo!**.
- Un párrafo debajo que dice **Estoy aprendiendo HTML.**.

En la pestaña del navegador debe aparecer el título **Mi primera página HTML**.

## Actividad práctica

Modifica únicamente el texto que se encuentra dentro de las etiquetas:

```html
<h1>Mis canciones favoritas</h1>
<p>Esta página reúne mis canciones favoritas.</p>
```

Después observa cómo cambia el contenido en **Preview**. No elimines las etiquetas de apertura ni las de cierre.

## Puntos clave de esta lección

- Las etiquetas HTML identifican y organizan los elementos del documento.
- Muchas etiquetas tienen apertura y cierre.
- `<html>` contiene el documento HTML.
- `<head>` contiene información y configuraciones del documento.
- `<body>` contiene el contenido visible de la página.
- `<h1>` permite crear un título principal.
- `<p>` permite escribir párrafos.

## Conclusión

En esta lección aprendiste a reconocer las partes de una etiqueta HTML, identificaste la estructura básica de un documento y creaste tu primera página con un título y un párrafo.

En las siguientes lecciones incorporarás más elementos para construir páginas web cada vez más completas.
