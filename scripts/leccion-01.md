# Lección 1: ¿Qué es el desarrollo web?

## ¿De qué están hechos los sitios web?

Los sitios web están formados por una mezcla de archivos de texto, lenguajes de programación, imágenes, videos y otros elementos multimedia. También incluyen componentes de infraestructura que el navegador de tu computadora o teléfono utiliza para interpretar todo y mostrarte la página que ves.

Entre esos diversos lenguajes de programación, podemos resaltar tres:
* HTML (HyperText Markup Language): Es el esqueleto o la estructura de la página (textos, títulos, imágenes, botones y enlaces).
* CSS (Cascading Style Sheets): Es la capa de diseño y estilo; define los colores, tipografías, márgenes, tamaños y la adaptabilidad para celulares.
* JavaScript: Es el lenguaje que añade dinamismo e interactividad (animaciones, menús desplegables, formularios que se validan al instante o mapas interactivos).

Durante este curso, solo vamos a profundizar en HTML y CSS.

## ¿Por qué HTML y CSS son los componentes básicos?

HTML y CSS son los componentes básicos de la web porque dividen el trabajo de crear una página en dos partes esenciales: la estructura y la presentación.
* HTML (Lenguaje de Marcado de Hipertexto) es el esqueleto: Define qué es cada elemento de la página (títulos, párrafos, imágenes, enlaces o listas) mediante etiquetas. Sin HTML no hay contenido ni orden en el navegador.
* CSS (Hojas de Estilo en Cascada) es el revestimiento y diseño: Toma ese esqueleto de HTML y le da vida mediante colores, tipografías, márgenes, sombras y la capacidad de adaptarse a diferentes pantallas (celulares, tablets o computadoras).

## Ejemplo de un sitio web

Para empezar, ingrese a Code Sandbox: https://codesandbox.io/dashboard

Luego, asegurese que el archivo index.html este conectado con styles.css, en caso de no tener esa conexión, pegue esto en la parte final de `<head>`:

```html
<link rel="stylesheet" href="styles.css" />
```

Después, dentro de `<body>`, empieze a escribir lo que quiera, como por ejemplo esto:

```html
<h1>Hola vuelvo a casa</h1>
```

Finalmente, dentro de styles.css, empieze a definir el estilo de su página, como por ejemplo esto:

```css
h1 {
    text-decoration: underline;
    color: blue;
}
```

## Resultado esperado

Si hizo todo esto, la página mostrará un texto grande, de color azul subrayado, que dice "Hola vuelvo a casa".

# Puntos clave de esta lección

Como puntos clave de esta lección, podemos destacar que:
* El desarrollo web es la creación de sitios y aplicaciones para internet.
* HTML define el contenido de una página web.
* CSS define la apariencia visual de esa página.
* La fórmula es: Sitio Web = Contenido (HTML) + Estilo (CSS).
* Solo necesitas un navegador para comenzar.

## Conclusión

En conclusión, con los lenguajes HTML y CSS, puedes construir cualquier sitio web.

En las siguientes lecciones aprenderás paso a paso cómo escribir tu primer código HTML y darle estilo con CSS.
