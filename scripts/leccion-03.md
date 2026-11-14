# Lección 3: Añadir más elementos HTML

## Etiquetas ul, img y a

Las etiquetas `<ul>`, `<img>` y `<a>` son fundamentales para agregar listas, imágenes y enlaces para que una página sea interactiva.

* Etiqueta `<ul>`: Esta etiqueta se utiliza para crear listas desordenadas. Al mismo tiempo, cada elemento de la lista se define con la etiqueta `<li>`.
* Etiqueta `<img>`: Esta etiqueta, como su nombre lo indica, se utiliza para insertar imágenes en la página web. Se debe especificar la ruta de la imagen mediante el atributo `src` y se puede agregar un texto alternativo con el atributo `alt`.
* Etiqueta `<a>`: Esta etiqueta se utiliza para crear enlaces a otras páginas web o recursos. Se debe especificar la URL de destino mediante el atributo `href`. Además, se puede definir si el enlace se abrirá en la misma ventana o en una nueva utilizando el atributo `target`.

## Ejemplo del funcionamiento de las etiquetas

Para empezar, ingrese a Code Sandbox: https://codesandbox.io/dashboard

Luego, con la etiqueta `<ul>`, empieze a definir la lista desordenada, como en este ejemplo:

```html
<ul class="clase1">
</ul>
```

Después, dentro de la etiqueta `<ul>`, agregue los elementos de la lista con la etiqueta `<li>`:

```html
<ul class="clase1">
    <li>Pelé</li>
    <li>Maradona</li>
    <li>Messi</li>
</ul>
```

Finalmente, con las etiquetas `<a>` e `<img>`, cree un hipervínculo o un enlace, al mismo tiempo que añade una imagen dentro de la etiqueta `<a>`, como en el siguiente ejemplo:

```html
<a href="" class="logo">
    <img height="200" width="150" src="img/descarga.png" alt="" />
</a>
```

## Resultado esperado

Si hizo todo esto, la página mostrará una lista con los nombres de tres futbolistas y un hipervínculo que contiene una imagen.

## Puntos clave de esta lección

Como puntos clave de esta lección, podemos destacar que:
* La etiqueta `<ul>` en HTML sirve para crear una lista desordenada (unordered list), cuyos elementos se muestran por defecto con viñetas o puntos y no siguen una secuencia numérica o jerárquica obligatoria.
* La etiqueta `<a>` (conocida como etiqueta de ancla) se utiliza en HTML para crear hipervínculos o enlaces.
* La etiqueta `<img>` en HTML se utiliza para incrustar imágenes (como fotografías, ilustraciones o gráficos) directamente en una página web.

## Conclusión

En conclusión, en esta lección aprendimos la importancia y el funcionamiento de las etiquetas HTML `<ul>`, `<img>` y `<a>`, las cuales permiten mejorar la estructura y presentación de una página web.

Con la etiqueta `<ul>` podemos organizar información mediante listas desordenadas, con `<img>` podemos insertar imágenes y con `<a>` podemos crear enlaces a otras páginas o recursos.

En conjunto, estas etiquetas nos ayudan a desarrollar páginas web más completas, visuales e interactivas, fortaleciendo nuestros conocimientos básicos de HTML.
