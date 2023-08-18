## Taller

### 1. Formato

A continuación haz que tenga un formato según la imagen adjunta. Para eso copia el código propuesto. 

![image](https://github.com/crodrigr/diseno-web-avanzado-uts-2023-02/assets/31961588/ab2224ff-8bbe-417d-9708-0f4b523f7cf3)


<details><summary>Mostrar código</summary>

<p>
  
```html
<!DOCTYPE html>
<html>
<head>
	<title>Ejercicio html etiquetas de texto básicas</title>
	<meta charset="utf-8"/>
</head>
<body>

Berners-Lee trabajó en el CERN desde junio hasta diciembre de 1980. Durante ese tiempo, propuso un proyecto basado en el hipertexto para facilitar la forma de compartir y la puesta al día de la información entre investigadores. En este periodo también construyó un programa llamado ENQUIRE que no llegó a ver la luz.1​

Después de dejar el CERN, en 1980, se fue a trabajar a la empresa de John Poole Image Computer Systems Ltd., pero regresó al CERN otra vez en 1984.

En 1989, el CERN era el nodo de Internet más grande de Europa y Berners-Lee vio la oportunidad de unir Internet y el hipertexto (HTTP y HTML), de lo que surgiría la World Wide Web. Desarrolló su primera propuesta de la Web el 12 de marzo de 1989,2​ pero no tuvo mucho eco, por lo que en 1990 y con la ayuda de Robert Cailliau, hicieron una revisión que fue aceptada por su gerente, Mike Sendall. Usó ideas similares a las que había usado en el sistema Enquire, para crear la World Wide Web, para esto diseñó y construyó el primer navegador (llamado WorldWideWeb y desarrollado con NEXTSTEP) y el primer servidor Web al que llamó httpd (HyperText Transfer Protocol daemon).

El primer servidor Web se encontraba en el CERN y fue puesto en línea el 6 de agosto de 1991. Esto proporcionó una explicación sobre lo que era el World Wide Web, cómo uno podría tener un navegador y cómo establecer un servidor Web. Este fue también el primer directorio Web del mundo, ya que Berners-Lee mantuvo una lista de otros sitios Web aparte del suyo. Debido a que tanto el software del servidor como del cliente fue liberado de forma gratuita desde el CERN, el corazón de Internet Europeo en esa época, su difusión fue muy rápida. El número de servidores Web pasó de veintiséis en 1992 a doscientos en octubre de 1995 lo que refleja cual fue la velocidad de la difusión de internet.

En 1994 entró en el Laboratorio de Ciencias de la Computación e Inteligencia Artificial del Massachusetts Institute of Technology. Se trasladó a EE. UU. y puso en marcha el W3C, que dirige actualmente. El W3C es un organismo internacional de estandarización de tecnologías Web dirigido conjuntamente por el Instituto Tecnológico de Massachusetts, el ERCIM francés y la Universidad de Keiō en Japón. Este organismo decidió que todos sus estándares fuesen libres, es decir, que los pudiese utilizar todo el mundo libremente sin coste alguno, lo que sin lugar a dudas fue una de las grandes razones para que la Web haya llegado a tener la importancia que tiene hoy en día.

En su libro Tejiendo la red, publicado en 1999, Berners-Lee explica por qué la tecnología web es libre y gratis. Se considera al mismo tiempo el inventor y el protector de la web.

</body>
</html>

```
</p>
</details> 

<br>
<br>

### 2 Lista ordenadas y no ordenadas


![image](https://github.com/crodrigr/diseno-web-avanzado-uts-2023-02/assets/31961588/a2786c4f-31a3-4e40-82d3-61c4651566e7)

<details><summary>Solución lista ordenanda</summary>

<p>

```html
<h2>Listas ordenadas</h2>

<ol type="a" start="4">
    <li>Elemento 1</li>		
    <li>Elemento 2</li>
    <li>Elemento 3</li>
    <li>Elemento 4</li>
</ol>

<ol start="100" reversed="reversed">
    <li>Elemento 1</li>		
    <li>Elemento 2</li>
    <li>Elemento 3</li>
    <li>Elemento 4</li>
</ol>

<ol type="i" start="999">
    <li>Elemento 1</li>		
    <li>Elemento 2</li>
    <li>Elemento 3</li>
    <li>Elemento 4</li>
</ol>

```

</p>
</details>



<details><summary>Solución lista no ordenanda</summary>

<p>

```html
<h2>Listas no ordenadas</h2>

<ul type="disc">
    <li>Elemento 1</li>		
    <li>Elemento 2</li>
    <li>Elemento 3</li>
    <li>Elemento 4</li>
</ul>

<ul type="circle">
    <li>Elemento 1</li>		
    <li>Elemento 2</li>
    <li>Elemento 3</li>
    <li>Elemento 4</li>
</ul>

<ul type="square">
    <li>Elemento 1</li>		
    <li>Elemento 2</li>
    <li>Elemento 3</li>
    <li>Elemento 4</li>
</ul>

```

</p>
</details> 