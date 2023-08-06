# Lista en Html

<br>
<br>

En HTML, puedes crear tres tipos de listas: listas ordenadas, listas no ordenadas y listas de definición. Aquí tienes ejemplos de cómo crear cada tipo de lista:

**Lista Ordenada (`<ol>`):**
Una lista ordenada es una lista numerada en la que los elementos se presentan en un orden específico. Se utiliza la etiqueta `<ol>` para crear una lista ordenada y la etiqueta `<li>` para cada elemento de la lista.

```html
<ol>
    <li>Primer elemento</li>
    <li>Segundo elemento</li>
    <li>Tercer elemento</li>
</ol>
```

**Lista No Ordenada (`<ul>`):**
Una lista no ordenada es una lista en la que los elementos no siguen un orden específico y se presentan con viñetas. Se utiliza la etiqueta `<ul>` para crear una lista no ordenada y la etiqueta `<li>` para cada elemento de la lista.

```html
<ul>
    <li>Elemento A</li>
    <li>Elemento B</li>
    <li>Elemento C</li>
</ul>
```

**Lista de Definición (`<dl>`):**
Una lista de definición se utiliza para mostrar términos y sus definiciones. Se utiliza la etiqueta `<dl>` para crear una lista de definición, la etiqueta `<dt>` para los términos y la etiqueta `<dd>` para las definiciones.

```html
<dl>
    <dt>Término 1</dt>
    <dd>Definición 1</dd>
    
    <dt>Término 2</dt>
    <dd>Definición 2</dd>
    
    <dt>Término 3</dt>
    <dd>Definición 3</dd>
</dl>
```

Estos son ejemplos básicos de cómo crear listas en HTML. Puedes personalizar el contenido y el estilo de las listas utilizando CSS para adaptarlas al diseño de tu página web. Las listas son una forma efectiva de organizar y presentar información de manera estructurada.


## Ménu con listas sin css

Si deseas crear un menú de listas sin utilizar CSS para aplicar estilos, puedes usar la estructura de listas no ordenadas (`<ul>`) y listas de elementos (`<li>`) directamente en HTML. Aquí tienes un ejemplo simple:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Menú de Listas HTML sin CSS</title>
</head>
<body>

<ul>
    <li><a href="#inicio">Inicio</a></li>
    <li><a href="#nosotros">Nosotros</a></li>
    <li><a href="#servicios">Servicios</a></li>
    <li><a href="#contacto">Contacto</a></li>
</ul>

</body>
</html>
```

En este ejemplo, hemos creado una lista no ordenada (`<ul>`) y hemos añadido elementos de lista (`<li>`) para cada enlace del menú. Cada enlace se crea con la etiqueta `<a>` y utiliza el atributo `href` para especificar la URL de destino.

Ten en cuenta que, sin estilos CSS, el menú tendrá la apariencia por defecto del navegador, que generalmente incluye viñetas y colores estándar. Si deseas personalizar el estilo del menú, deberás agregar estilos CSS correspondientes en la sección `<style>` dentro de la etiqueta `<head>`.