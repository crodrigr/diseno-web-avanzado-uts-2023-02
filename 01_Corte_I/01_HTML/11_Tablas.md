# Tablas en Html

<br>
<br>

En HTML, una tabla es una estructura que permite organizar y mostrar datos en filas y columnas. Se utiliza la etiqueta `<table>` para crear la tabla, y dentro de esta etiqueta se utilizan las etiquetas `<tr>` (filas) para cada fila de la tabla, y las etiquetas `<th>` (encabezados) o `<td>` (celdas de datos) para cada celda en la fila.

Aquí tienes una representación básica de cómo se estructura una tabla en HTML:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Tabla HTML</title>
</head>
<body>

<table>
    <tr>
        <th>Encabezado de Columna 1</th>
        <th>Encabezado de Columna 2</th>
    </tr>
    <tr>
        <td>Celda 1,1</td>
        <td>Celda 1,2</td>
    </tr>
    <tr>
        <td>Celda 2,1</td>
        <td>Celda 2,2</td>
    </tr>
</table>

</body>
</html>
```

En este ejemplo:

- La etiqueta `<table>` define la tabla en sí.
- Las etiquetas `<tr>` definen las filas de la tabla.
- Las etiquetas `<th>` se utilizan para las celdas de encabezado (cabecera) de la tabla.
- Las etiquetas `<td>` se utilizan para las celdas de datos (contenido) de la tabla.

Esta estructura básica de tabla puede expandirse y personalizarse para mostrar cualquier tipo de información en filas y columnas. Puedes agregar más filas y celdas según sea necesario para tus datos específicos.

<br>
<br>
<br>


# Atributos Colsap y Rowspap

<br>
<br>


Los atributos `colspan` y `rowspan` se utilizan en las etiquetas `<td>` (celdas de datos) y `<th>` (encabezados de celda) en una tabla HTML para indicar cuántas columnas o filas debe ocupar una celda en particular. Estos atributos son muy útiles cuando deseas combinar celdas en varias columnas o filas, lo que te permite crear diseños más complejos en tu tabla.

Aquí tienes un ejemplo de cómo se utilizan los atributos `colspan` y `rowspan` en una tabla:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Atributos colspan y rowspan</title>
</head>
<body>

<table border="1">
    <tr>
        <th>Nombre</th>
        <th colspan="2">Detalles</th>
    </tr>
    <tr>
        <td rowspan="2">Producto A</td>
        <td>Precio</td>
        <td>$19.99</td>
    </tr>
    <tr>
        <td>Stock</td>
        <td>10 unidades</td>
    </tr>
    <tr>
        <td>Producto B</td>
        <td>Precio</td>
        <td>$29.99</td>
    </tr>
    <tr>
        <td>Producto C</td>
        <td>Precio</td>
        <td>$9.99</td>
    </tr>
</table>

</body>
</html>
```

En este ejemplo:

- Usamos `colspan="2"` en la segunda celda de encabezado para indicar que debe ocupar dos columnas.
- Usamos `rowspan="2"` en la primera celda de datos "Producto A" para indicar que debe ocupar dos filas.
- Esto crea una celda grande que se extiende por dos filas y dos columnas en la tabla.

Puedes experimentar con los valores de `colspan` y `rowspan` para crear diseños más complejos en tus tablas, como fusionar celdas en filas y columnas diferentes según tus necesidades.