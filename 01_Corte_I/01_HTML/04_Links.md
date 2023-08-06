# Links

<br>
<br>

En HTML, los enlaces se crean utilizando la etiqueta `<a>`, que significa "hipervínculo" (o "anchor" en inglés). Los enlaces permiten a los usuarios navegar de una página a otra página web, a un archivo o a una ubicación dentro de la misma página. Aquí tienes un ejemplo de cómo se utiliza la etiqueta `<a>` para crear un enlace:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Enlaces HTML</title>
</head>
<body>

<p>Visita mi <a href="https://www.ejemplo.com">sitio web</a> para obtener más información.</p>

<p>Descarga el <a href="documento.pdf">documento PDF</a> relacionado.</p>

</body>
</html>
```

En el ejemplo anterior:

- El texto "sitio web" está enlazado a la URL `https://www.ejemplo.com` utilizando el atributo `href`.
- El texto "documento PDF" está enlazado a un archivo llamado `documento.pdf` que se encuentra en el mismo directorio que la página HTML.

También puedes crear enlaces a ubicaciones dentro de la misma página utilizando anclajes. Por ejemplo, si tienes un encabezado de nivel 2 con el texto "Más Información", puedes enlazar a esa sección de la siguiente manera:

```html
<p>Salta a la <a href="#informacion">sección de Más Información</a>.</p>

<h2 id="informacion">Más Información</h2>
<p>Aquí encontrarás detalles adicionales sobre el tema.</p>
```

La parte `#informacion` en el atributo `href` se refiere al elemento con el atributo `id="informacion"`.

Los enlaces son una parte fundamental de la web y te permiten conectar tus páginas y recursos de manera efectiva, permitiendo a los usuarios navegar y acceder a diferentes contenidos.