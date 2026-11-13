# Lección 4: Introducción a CSS

## ¿Qué es CSS?

CSS (*Cascading Style Sheets*, hojas de estilo en cascada) es el lenguaje que se usa para darle estilo a una página HTML: colores, fuentes, tamaños y diseño.

Una forma sencilla de verlo: **HTML es el esqueleto** de la página (el contenido) y **CSS es la ropa** (cómo se ve ese contenido).

## Cómo vincular CSS a un HTML

Para que el HTML use los estilos, se crea un archivo con extensión `.css` en la misma carpeta y se conecta con la etiqueta `link` dentro del `head`.

### Ejemplo de vinculación:

```html
<head>
  <meta charset="UTF-8">
  <title>Mi primera página con estilo</title>
  <link rel="stylesheet" href="estilos.css">
</head>
```

* `rel="stylesheet"`: le indica al browser que el archivo es una hoja de estilos.
* `href="estilos.css"`: es el nombre (y la ruta) del archivo CSS.

## Estructura de una regla CSS

Una regla CSS tiene tres partes: el **selector**, la **propiedad** y el **valor**.

```css
selector {
  propiedad: valor;
}
```

* **Selector:** indica a qué elemento HTML se le aplica el estilo (por ejemplo `body`, `h1` o `p`).
* **Propiedad:** es lo que se quiere cambiar (por ejemplo `color` o `font-size`).
* **Valor:** es el cambio que se quiere hacer (por ejemplo `blue` o `20px`).
* Cada declaración termina con punto y coma `;` y todo va dentro de llaves `{ }`.

### Ejemplo de una regla:

```css
body {
  background-color: lightblue;
}
```

Esta regla cambia el color de fondo de toda la página a celeste.

## Propiedades básicas

| Propiedad | ¿Qué hace? | Ejemplo |
|---|---|---|
| `color` | Cambia el color del texto | `color: darkblue;` |
| `background-color` | Cambia el color de fondo | `background-color: yellow;` |
| `font-family` | Cambia el tipo de letra | `font-family: Arial, sans-serif;` |
| `font-size` | Cambia el tamaño del texto | `font-size: 20px;` |
| `text-align` | Alinea el texto | `text-align: center;` |
| `padding` | Espacio interno de un elemento | `padding: 10px;` |
| `border` | Agrega un borde | `border: 2px solid black;` |

## Clases e IDs

A veces se quiere darle estilo a **un solo elemento** y no a todos los de su tipo. Para eso existen las clases y los IDs.

### Clases (class):

Una clase se define en el HTML con el atributo `class` y en el CSS se llama con un **punto** (`.`). Una misma clase puede usarse en muchos elementos.

```html
<p class="destacado">Este párrafo tiene estilo especial.</p>
```

```css
.destacado {
  background-color: yellow;
}
```

### IDs (id):

Un ID se define en el HTML con el atributo `id` y en el CSS se llama con un **numeral** (`#`). Un ID debe usarse una sola vez en la página.

```html
<p id="aviso">Este es un aviso único.</p>
```

```css
#aviso {
  border: 2px solid black;
}
```

### Diferencias:

Las clases (`.`) se pueden reutilizar en varios elementos, mientras que los IDs (`#`) identifican a un único elemento de la página.

## Ejemplo práctico:

**index.html**

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Mi primera página con estilo</title>
  <link rel="stylesheet" href="estilos.css">
</head>
<body>
  <h1>Mi Página Personal</h1>
  <p class="destacado">¡Hola! Me llamo Ana y estoy aprendiendo CSS.</p>

  <h2>Mis hobbies</h2>
  <ul>
    <li>Jugar videojuegos</li>
    <li>Escuchar música</li>
    <li>Dibujar</li>
  </ul>

  <p id="aviso">Esta página fue hecha en la clase de CSS.</p>
</body>
</html>
```

**estilos.css**

```css
body {
  background-color: lightblue;
  font-family: Arial, sans-serif;
  margin: 30px;
}

h1 {
  color: darkblue;
  text-align: center;
}

h2 {
  color: purple;
}

.destacado {
  font-size: 20px;
  background-color: yellow;
  padding: 10px;
}

li {
  color: darkgreen;
}

#aviso {
  border: 2px solid black;
  padding: 8px;
  text-align: center;
}
```

## Resultado esperado:

La página mostrará:
* Un fondo celeste con letra Arial.
* Un título azul oscuro centrado.
* Un párrafo con fondo amarillo y letra más grande (por la clase `destacado`).
* Un subtítulo morado y una lista de hobbies en verde oscuro.
* Un párrafo final con borde negro y texto centrado (por el ID `aviso`).

## Consejos clave:

* Los archivos `index.html` y `estilos.css` deben estar en la misma carpeta; si no, hay que ajustar la ruta en `href`.
* Revisar que el nombre del archivo CSS esté bien escrito, incluida la extensión.
* No olvidar el punto y coma `;` al final de cada propiedad ni cerrar las llaves `}`.
* Después de guardar, actualizar el navegador para ver los cambios.

## Práctica:

Abre el enlace de CodePen que aparece en la descripción del video (no es necesario registrarse) y prueba lo siguiente:

1. Cambia el color de fondo del `body`.
2. Cambia el color y la alineación del `h1`.
3. Crea tu propia clase y aplícala a un párrafo.

## Conclusión:

Recordemos que CSS se encarga del aspecto de la página y se vincula al HTML con la etiqueta `link`. Cada regla se compone de un selector, una propiedad y un valor, y para darle estilo a elementos específicos podemos usar clases (con punto) o IDs (con numeral).