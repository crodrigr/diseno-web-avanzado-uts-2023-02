# Formularios en Html

<br>
<br>

Los formularios en HTML son elementos esenciales que permiten a los usuarios enviar datos al servidor web para su procesamiento. Aquí tienes un ejemplo básico de cómo crear un formulario en HTML:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Formulario HTML</title>
</head>
<body>

<h2>Formulario de Contacto</h2>

<form action="/procesar.php" method="post">
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre" required>
    <br>
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
    <br>
    
    <label for="mensaje">Mensaje:</label>
    <textarea id="mensaje" name="mensaje" rows="4" required></textarea>
    <br>
    
    <input type="submit" value="Enviar">
</form>

</body>
</html>
```

En este ejemplo:

- Utilizamos la etiqueta `<form>` para crear el formulario. El atributo `action` especifica la URL a la que se enviarán los datos del formulario, y el atributo `method` define el método de envío (en este caso, `post`).
- Utilizamos etiquetas `<label>` para etiquetar cada campo de entrada (`<input>`) y `<textarea>`.
- Los elementos de entrada del usuario se crean utilizando etiquetas `<input>` y `<textarea>`, con diferentes tipos de atributos como `type`, `id`, `name` y `required`.
- El botón de envío se crea con `<input type="submit">`.

Este es un formulario de contacto simple. Al enviar el formulario, los datos se enviarían al servidor web para su procesamiento. Puedes ajustar y personalizar este formulario según tus necesidades, y procesar los datos utilizando tecnologías del lado del servidor, como PHP, Python, Node.js, etc.


## Validación de formularios

<br>

La validación de formularios en HTML se refiere a asegurarse de que los datos ingresados por el usuario cumplan con ciertos requisitos antes de enviarlos al servidor para su procesamiento. Puedes utilizar la validación tanto del lado del cliente (en el navegador del usuario) como del lado del servidor (en el servidor web que recibe los datos).

**Validación del Lado del Cliente:**

La validación del lado del cliente se realiza utilizando atributos HTML y JavaScript. Aquí hay algunos ejemplos de validación de formularios en HTML:

1. **Atributos `required`, `type` y `pattern`:** Puedes utilizar el atributo `required` en campos de entrada para hacer que sean obligatorios. El atributo `type` permite definir el tipo de entrada (por ejemplo, `email`, `number`, `date`) y `pattern` permite especificar una expresión regular para validar el formato.

```html
<input type="email" id="email" name="email" required>
<input type="number" id="edad" name="edad" min="18" max="99">
<input type="text" id="codigo" name="codigo" pattern="[A-Za-z0-9]{6}">
```

2. **Atributos `min` y `max`:** Puedes usar estos atributos para definir rangos numéricos o fechas permitidas en campos de entrada numéricos o de fecha.

3. **Validación Personalizada con JavaScript:** Puedes utilizar JavaScript para realizar validaciones personalizadas y mostrar mensajes de error. Aquí hay un ejemplo simple:

```html
<form onsubmit="return validarFormulario()">
    <input type="text" id="nombre" required>
    <input type="submit" value="Enviar">
</form>

<script>
function validarFormulario() {
    var nombre = document.getElementById("nombre").value;
    if (nombre === "") {
        alert("Por favor, ingresa tu nombre.");
        return false;
    }
    return true;
}
</script>
```

**Validación del Lado del Servidor:**

La validación del lado del servidor es esencial, ya que la validación del lado del cliente puede ser evitada o manipulada. Debes realizar una validación exhaustiva en tu servidor para garantizar que los datos ingresados sean seguros y cumplan con los requisitos.

Utilizar una combinación de validación del lado del cliente y del servidor es la mejor práctica para asegurarte de que los datos ingresados sean correctos y seguros antes de ser procesados.


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

Estos son solo algunos ejemplos de los tipos de datos que puedes recopilar a través de formularios HTML. Cada tipo de campo de entrada tiene su propio propósito y es útil para diferentes tipos de datos. Puedes combinar estos tipos de campos para crear formularios completos y funcionales

## Practica

![image](https://github.com/crodrigr/diseno-web-avanzado-uts-2023-02/assets/31961588/a8654924-afa7-4a74-befc-369e690dea09)
