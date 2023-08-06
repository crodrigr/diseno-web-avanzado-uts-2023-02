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

<br>
<br>

## Get y Post


En HTML, los formularios pueden enviar datos al servidor utilizando dos métodos principales: GET y POST. Estos métodos determinan cómo se transmiten los datos del formulario al servidor para su procesamiento.

**Método GET:**
Cuando se utiliza el método GET, los datos del formulario se adjuntan a la URL como parámetros de consulta. Esto significa que los datos son visibles en la URL y se pueden ver en la barra de direcciones del navegador. Es adecuado para formularios que realizan búsquedas o solicitan datos del servidor, pero no se recomienda para formularios que envíen datos sensibles, ya que los datos son visibles en la URL.

```html
<form action="/procesar.php" method="get">
    <input type="text" name="nombre">
    <input type="submit" value="Enviar">
</form>
```

En este ejemplo, si el usuario ingresa "Juan" en el campo de nombre y envía el formulario, la URL resultante podría ser: `/procesar.php?nombre=Juan`

**Método POST:**
Cuando se utiliza el método POST, los datos del formulario se envían en el cuerpo de la solicitud HTTP, en lugar de adjuntarse a la URL. Los datos no son visibles en la URL y se considera más seguro para el envío de datos sensibles, como contraseñas. Es el método preferido para enviar datos que pueden modificar el estado del servidor.

```html
<form action="/procesar.php" method="post">
    <input type="text" name="nombre">
    <input type="submit" value="Enviar">
</form>
```

En este caso, los datos no serían visibles en la URL, y se enviarían en el cuerpo de la solicitud al archivo `procesar.php`.

En ambos casos, el atributo `action` de la etiqueta `<form>` especifica la URL a la que se enviarán los datos, y el atributo `method` define el método de envío (`get` o `post`).

Recuerda que, independientemente del método que elijas, siempre debes realizar una validación adecuada tanto en el lado del cliente (usando HTML y JavaScript) como en el lado del servidor (usando un lenguaje de servidor como PHP, Python, etc.) para garantizar la seguridad y la integridad de los datos.

<br>
<br>

## Tipos de datos

<br>
<br>


En un formulario HTML, existen varios tipos de datos que se pueden recopilar a través de los diferentes tipos de campos de entrada. Aquí tienes algunos de los tipos de datos más comunes que se pueden capturar en un formulario:

1. **Texto (`text`):** Se utiliza para recopilar cadenas de texto, como nombres, direcciones o comentarios.

```html
<input type="text" name="nombre">
```

2. **Contraseña (`password`):** Similar al campo de texto, pero el texto ingresado se oculta con asteriscos o puntos, generalmente utilizado para contraseñas.

```html
<input type="password" name="contraseña">
```

3. **Número (`number`):** Se utiliza para recopilar valores numéricos.

```html
<input type="number" name="edad">
```

4. **Correo Electrónico (`email`):** Se utiliza para recopilar direcciones de correo electrónico y realiza automáticamente una validación básica del formato del correo electrónico.

```html
<input type="email" name="correo">
```

5. **Fecha (`date`):** Permite a los usuarios seleccionar una fecha de un calendario emergente.

```html
<input type="date" name="fecha_nacimiento">
```

6. **Selección de Opciones (`select` y `option`):** Se utiliza para crear listas desplegables o menús de selección.

```html
<select name="pais">
    <option value="us">Estados Unidos</option>
    <option value="ca">Canadá</option>
    <option value="mx">México</option>
</select>
```

7. **Botones de Radio (`radio`):** Se utiliza para recopilar una selección única de varias opciones.

```html
<input type="radio" name="genero" value="masculino"> Masculino
<input type="radio" name="genero" value="femenino"> Femenino
```

8. **Casillas de Verificación (`checkbox`):** Se utiliza para recopilar opciones múltiples.

```html
<input type="checkbox" name="intereses[]" value="deporte"> Deporte
<input type="checkbox" name="intereses[]" value="musica"> Música
<input type="checkbox" name="intereses[]" value="lectura"> Lectura
```

9. **Área de Texto (`textarea`):** Se utiliza para recopilar texto más largo, como comentarios o descripciones.

```html
<textarea name="comentario" rows="4" cols="50"></textarea>
```

Estos son solo algunos ejemplos de los tipos de datos que puedes recopilar a través de formularios HTML. Cada tipo de campo de entrada tiene su propio propósito y es útil para diferentes tipos de datos. Puedes combinar estos tipos de campos para crear formularios completos y funcionales.