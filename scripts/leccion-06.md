# Lección 6: Consejos y Próximos Pasos

## Revisar y mejorar nuestra página web

Durante las lecciones anteriores aprendimos a crear la estructura de una página con HTML, añadir elementos como imágenes, listas y enlaces, aplicar estilos con CSS y combinar estos recursos para construir un perfil personal.

En esta última lección vamos a revisar ese proyecto y aprender algunas prácticas que nos ayudarán a mantener nuestro código ordenado, reconocer errores frecuentes y comprobar que nuestro HTML y CSS estén bien escritos. También conoceremos recursos para continuar aprendiendo y veremos cómo compartir nuestro trabajo.

Para realizar los ejemplos, utilizaremos el proyecto de perfil personal de la Lección 5. No es necesario crear una página nueva.

## Buenas prácticas al trabajar con HTML y CSS

Antes de compartir una página web, es recomendable revisar algunos hábitos que facilitan su lectura y mantenimiento:

* **Mantener el código ordenado:** utiliza sangrías y separa los bloques con saltos de línea. Así será más sencillo identificar dónde comienza y termina cada sección.
* **Usar etiquetas según su propósito:** organiza el contenido con elementos como `<header>`, `<main>`, `<section>` y `<footer>`. Utiliza encabezados para los títulos, párrafos para el texto y listas cuando presentes varios elementos.
* **Cerrar y anidar correctamente las etiquetas:** comprueba que cada elemento tenga su cierre cuando corresponda y que los elementos estén dentro del contenedor adecuado.
* **Usar nombres claros y consistentes:** si en HTML escribes `class="profile-link"`, el selector CSS debe llamarse `.profile-link`. Recuerda que el punto identifica una clase en CSS.
* **Separar el contenido de los estilos:** mantén la estructura en `index.html` y las reglas visuales en `styles.css`. Verifica que ambos archivos estén conectados correctamente.
* **Revisar enlaces e imágenes:** comprueba que los enlaces lleven al destino esperado. Cuando agregues imágenes, utiliza el atributo `alt` para proporcionar una descripción textual apropiada.
* **Probar distintos tamaños de pantalla:** revisa que el contenido se pueda leer y utilizar tanto en una computadora como en un celular.

Estas prácticas no solo ayudan a que la página se vea correctamente; también hacen que el proyecto sea más fácil de entender y modificar.

## Errores comunes y cómo reconocerlos

Al trabajar con HTML y CSS podemos cometer errores pequeños que cambian el resultado de la página. Estos son algunos de los más frecuentes:

### 1. Nombres de clases diferentes

En HTML podemos tener:

```html
<a class="profile-link" href="#hobbies">Conoce mis hobbies</a>
```

El selector correspondiente en CSS debe ser:

```css
.profile-link {
    background-color: #2563eb;
    color: #ffffff;
}
```

Si escribimos `.profile-lnik` en CSS, el nombre ya no coincide con la clase del HTML y esas reglas no se aplicarán al enlace.

### 2. Enlaces internos sin un destino coincidente

En el perfil personal, el enlace utiliza `href="#hobbies"`. Para que funcione, debe existir una sección con el identificador correspondiente:

```html
<a class="profile-link" href="#hobbies">Conoce mis hobbies</a>

<section class="content-section" id="hobbies">
    <h2>Mis hobbies</h2>
</section>
```

El valor de `href` y el de `id` deben coincidir. Si uno se llama `hobbies` y el otro `pasatiempos`, el enlace no llevará a esa sección.

### 3. Etiquetas sin cerrar o mal anidadas

Revisa que las etiquetas estén correctamente anidadas. Por ejemplo, si abres una sección, organiza su contenido dentro de ella y ciérrala antes de terminar el contenedor que la incluye.

### 4. Archivo CSS o ruta incorrectos

En el `<head>` del documento debe aparecer el enlace al archivo de estilos:

```html
<link rel="stylesheet" href="styles.css">
```

Comprueba que el archivo se llame exactamente `styles.css` y que se encuentre en la ruta indicada. Si está dentro de otra carpeta, la ruta debe reflejar esa ubicación.

### 5. Errores de escritura en CSS

Una propiedad mal escrita, una llave faltante o un punto y coma omitido pueden impedir que una regla se interprete como esperas. Revisa la sintaxis de cada bloque:

```css
.profile-link {
    background-color: #2563eb;
    color: #ffffff;
}
```

Cuando algo no se vea como esperas, revisa primero el nombre del selector, después la propiedad y finalmente las llaves y los signos de puntuación.

## Ejemplo: revisar nuestro perfil personal

Para empezar, ingrese a CodeSandbox y abra el proyecto de perfil personal trabajado en la Lección 5:

https://codesandbox.io/p/sandbox/web-dev-course-97kkrh

Trabajaremos con dos archivos: `index.html`, donde se encuentra la estructura, y `styles.css`, donde se encuentran los estilos.

Primero, revise el archivo `index.html` y compruebe lo siguiente:

1. Que el documento tenga la estructura principal y que las etiquetas estén correctamente cerradas.
2. Que el contenido esté organizado en secciones claras, como presentación, hobbies y metas.
3. Que el enlace **Conoce mis hobbies** utilice `href="#hobbies"` y que la sección de hobbies tenga `id="hobbies"`.
4. Que las clases utilizadas en HTML tengan sus selectores correspondientes en CSS.

Después, abra `styles.css` y compruebe que las reglas estén organizadas y que los nombres de los selectores coincidan con las clases del documento HTML.

Finalmente, observe la vista previa. Pruebe el enlace **Conoce mis hobbies**, revise que los estilos se apliquen y cambie el ancho de la vista para comprobar cómo se distribuye el contenido en una pantalla más pequeña.

## Validar nuestro código

Además de revisar el proyecto manualmente, podemos utilizar herramientas de validación. Estas herramientas ayudan a detectar problemas de sintaxis y de estructura.

### Validar HTML con Nu HTML Checker

Para revisar el HTML, ingrese a:

https://validator.w3.org/nu/

Luego:

1. Abra el archivo `index.html` en CodeSandbox.
2. Copie su contenido completo.
3. En Nu HTML Checker, utilice la opción de entrada de código para pegar el HTML o indique una URL pública del documento si dispone de ella.
4. Ejecute la comprobación.
5. Revise los mensajes que aparezcan, localice la línea indicada y corrija los problemas encontrados.
6. Vuelva a realizar la comprobación después de los cambios.

El Nu HTML Checker revisa documentos HTML y muestra mensajes que ayudan a identificar errores. Es una herramienta de revisión, no una certificación que garantice por sí sola que una página sea perfecta.

### Validar CSS

Para revisar la hoja de estilos, también podemos utilizar el servicio de validación de CSS del W3C:

https://jigsaw.w3.org/css-validator/

Podemos introducir el contenido de `styles.css` directamente o utilizar una de las otras modalidades disponibles en el servicio. Después, revisamos los mensajes y corregimos las reglas que tengan problemas.

Recuerda que un validador no reemplaza la revisión visual. También debemos probar los enlaces, comprobar que los estilos se vean correctamente y revisar la página en diferentes tamaños de pantalla.

## Dónde aprender más

Aprender desarrollo web requiere práctica y consulta constante. Una fuente recomendada para continuar es **MDN Web Docs**, que ofrece guías y documentación para personas que están comenzando.

Puede ingresar a:

https://developer.mozilla.org/es/docs/Learn_web_development

En MDN encontrará recursos para profundizar en:

* **HTML:** estructura del contenido, etiquetas, enlaces, listas e imágenes.
* **CSS:** selectores, colores, tipografías, espaciado y diseño.
* **Accesibilidad:** recomendaciones para que el contenido pueda ser utilizado por más personas.
* **Herramientas y pruebas:** recursos para revisar y mejorar los proyectos web.

Una buena forma de aprender es elegir un tema, leer su explicación, probar un ejemplo en CodeSandbox y observar cómo cambia el resultado.

## Compartir nuestro trabajo

Cuando termine de revisar su perfil personal, compruebe que la vista previa funcione y que los enlaces y estilos se comporten como espera.

Después, utilice la opción de compartir de CodeSandbox para obtener el enlace de su proyecto. Envíe ese enlace mediante el espacio o canal indicado por el docente para que otras personas puedan revisar su creación.

Antes de compartir, asegúrese de que el proyecto no dependa de archivos que estén fuera del sandbox y que el enlace permita acceder al trabajo.

## Actividad práctica

Revise el perfil personal que construyó en la Lección 5 y complete los siguientes pasos:

1. Compruebe que el HTML esté ordenado y que las etiquetas estén correctamente cerradas.
2. Verifique que el enlace **Conoce mis hobbies** lleve a la sección correcta.
3. Compruebe que las clases de `index.html` coincidan con los selectores de `styles.css`.
4. Revise el HTML con Nu HTML Checker.
5. Revise el CSS con el validador del W3C.
6. Pruebe la página en una vista de computadora y otra más estrecha, como la de un celular.
7. Copie el enlace de CodeSandbox y compártalo según las indicaciones del curso.

## Puntos clave de esta lección

Como puntos clave de esta lección, podemos destacar que:

* Mantener el código ordenado facilita su lectura y mantenimiento.
* Las etiquetas HTML deben utilizarse de acuerdo con su propósito y estar correctamente anidadas.
* Los nombres de clases en HTML deben coincidir con los selectores correspondientes en CSS.
* Los enlaces internos necesitan un destino que coincida con su atributo `href`.
* Los validadores de HTML y CSS ayudan a detectar problemas, pero no sustituyen las pruebas visuales y funcionales.
* MDN Web Docs es un recurso para continuar aprendiendo HTML, CSS y otras tecnologías web.
* Antes de compartir un proyecto, es importante revisar su funcionamiento y comprobar que el enlace permita acceder a él.

## Conclusión

En conclusión, en esta lección aprendimos que crear una página web no consiste solamente en escribir HTML y CSS. También debemos revisar nuestro código, mantenerlo ordenado, corregir errores y comprobar que el resultado funcione como esperamos.

Con herramientas como los validadores y recursos como MDN podemos seguir mejorando nuestros proyectos y ampliar nuestros conocimientos.

Con esto terminamos el curso de Fundamentos de Desarrollo Web. Ahora puedes continuar practicando, personalizar tus propias páginas y compartir tus creaciones. ¡Gracias por aprender con NutriStartup!
