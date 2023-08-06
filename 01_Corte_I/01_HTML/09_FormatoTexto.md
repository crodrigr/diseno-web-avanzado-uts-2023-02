# Formato a texto en Html

<br>
<br>

En HTML, puedes aplicar formato al texto utilizando diversas etiquetas y propiedades CSS para lograr efectos visuales específicos. Aquí hay algunos ejemplos de cómo puedes formatear el texto en tu página web:

1. **Negrita (`<strong>` o `<b>`):** Se utiliza para enfatizar un texto y hacerlo más destacado visualmente.

```html
<p>Este es un texto <strong>importante</strong>.</p>
```

2. **Cursiva (`<em>` o `<i>`):** Se utiliza para indicar énfasis o un tono diferente en el texto.

```html
<p>Esto es <em>cursiva</em>.</p>
```

3. **Subrayado (`<u>`):** Se utiliza para subrayar el texto.

```html
<p>Este es un <u>texto subrayado</u>.</p>
```

4. **Tachado (`<s>` o `<del>`):** Se utiliza para mostrar el texto con una línea horizontal a través de él.

```html
<p>Este es un <s>texto tachado</s>.</p>
```

5. **Texto con formato predefinido (`<pre>`):** Mantiene el formato original del texto, incluyendo espacios y saltos de línea.

```html
<pre>
    Este es
    un texto
    con
    formato predefinido.
</pre>
```

6. **Cambio de tamaño de fuente (`<span>` y CSS):** Puedes utilizar la etiqueta `<span>` junto con CSS para cambiar el tamaño de fuente.

```html
<p>Este es un <span style="font-size: 24px;">texto más grande</span> de lo normal.</p>
```

7. **Fuente personalizada (`<span>` y CSS con `@font-face`):** Puedes cargar y aplicar fuentes personalizadas utilizando CSS.

```html
<style>
@font-face {
    font-family: MiFuentePersonalizada;
    src: url('ruta-de-la-fuente.ttf');
}

.fuente-personalizada {
    font-family: MiFuentePersonalizada, sans-serif;
}
</style>

<p>Este es un <span class="fuente-personalizada">texto con fuente personalizada</span>.</p>
```

8. **Color de texto (`<span>` y CSS):** Puedes cambiar el color del texto utilizando CSS.

```html
<p>Este es un <span style="color: red;">texto de color rojo</span>.</p>
```

Estos son solo algunos ejemplos de cómo puedes aplicar formato al texto en HTML. La combinación de etiquetas HTML y propiedades CSS te permite lograr una amplia variedad de efectos visuales para adaptarse al diseño de tu página web.