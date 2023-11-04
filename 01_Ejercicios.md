Claro, aquí tienes un ejercicio más complejo que utiliza callbacks para filtrar y transformar un array de objetos que representan productos. El enunciado es el siguiente:

**Enunciado del ejercicio:**

Supongamos que tienes un array de objetos que representan productos. Cada objeto tiene propiedades como `nombre`, `precio` y `stock`. Escribe dos funciones:

1. `filtrarProductos(array, callback)`: Esta función toma un array de productos y un callback como argumentos. El callback debe ser una función que acepte un producto y devuelva `true` si el producto cumple con ciertos criterios, o `false` en caso contrario. La función `filtrarProductos` debe utilizar el callback para filtrar los productos que cumplen con los criterios y devolver un nuevo array con esos productos.

2. `calcularTotal(array)`: Esta función toma un array de productos y calcula el precio total de los productos en ese array.



// Mostramos los productos filtrados y el precio total
console.log("Productos filtrados:", productosFiltrados);
console.log("Precio total:", precioTotal);
```

En este ejercicio, hemos definido un array de objetos que representan productos y dos funciones: `filtrarProductos` y `calcularTotal`. La función `filtrarProductos` toma un array de productos y un callback que filtra los productos que cumplan con ciertos criterios (en este caso, aquellos con un precio mayor o igual a 20). Luego, la función `calcularTotal` calcula el precio total de los productos filtrados. Finalmente, se muestra en la consola el resultado de los productos filtrados y el precio total.
