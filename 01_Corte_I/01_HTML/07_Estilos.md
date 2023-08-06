# Estilos Css en Html

<br>
<br>

CSS (Cascading Style Sheets) es un lenguaje utilizado para describir la presentación y el estilo de una página web escrita en HTML. Permite controlar aspectos como el color, la fuente, el espaciado, la disposición y otros estilos visuales de los elementos en una página. Aquí te muestro cómo se aplica CSS a un documento HTML:

**Métodos para aplicar CSS:**

1. **CSS Interno:** Se agrega directamente en la sección `<style>` dentro del encabezado (`<head>`) del documento HTML. Aquí tienes un ejemplo:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de CSS Interno</title>
    <style>
        /* Definición de estilo para párrafos */
        p {
            color: blue;
            font-size: 18px;
        }
    </style>
</head>
<body>
    <p>Este es un párrafo con estilo CSS interno.</p>
</body>
</html>
```

2. **CSS Externo:** Se crea un archivo `.css` independiente que contiene las reglas de estilo y se vincula al documento HTML utilizando la etiqueta `<link>` en la sección `<head>`. Por ejemplo:

En `styles.css`:
```css
/* Definición de estilo para párrafos */
p {
    color: blue;
    font-size: 18px;
}
```

En el documento HTML:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de CSS Externo</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <p>Este es un párrafo con estilo CSS externo.</p>
</body>
</html>
```

3. **CSS en línea:** Se aplica directamente a un elemento en línea utilizando el atributo `style` dentro de la etiqueta HTML. Por ejemplo:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de CSS en Línea</title>
</head>
<body>
    <p style="color: blue; font-size: 18px;">Este es un párrafo con estilo CSS en línea.</p>
</body>
</html>
```

**Reglas de Estilo en CSS:**

En las reglas de estilo CSS, utilizas selectores para indicar a qué elementos se aplicará el estilo, y luego defines las propiedades y los valores de estilo. Por ejemplo:

```css
/* Selector de etiqueta */
p {
    color: blue;
    font-size: 18px;
}

/* Selector de clase */
.mi-clase {
    font-weight: bold;
}

/* Selector de ID */
#mi-id {
    text-decoration: underline;
}
```

Es importante recordar que CSS es muy versátil y permite estilizar prácticamente todos los elementos HTML. Puedes aplicar estilos a clases, IDs, elementos anidados y mucho más para lograr la apariencia visual deseada en tu página web.