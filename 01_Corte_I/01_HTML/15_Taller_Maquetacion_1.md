# Taller de maquetación

Con base en el siguiente diseño realice la maqueta en **html**

<br>

![image](https://github.com/crodrigr/diseno-web-avanzado-uts-2023-02/assets/31961588/94b67cc7-6424-42d0-b6e1-bbad9c6ecaae)

En HTML, la etiqueta `<div>` es una etiqueta de división que se utiliza para crear un contenedor genérico y flexible en el cual se pueden agrupar y organizar otros elementos HTML, como texto, imágenes, enlaces, formularios y otros elementos. El término "div" es una abreviatura de "división" y se usa comúnmente para dividir o estructurar el contenido de una página web en secciones lógicas o para aplicar estilos y efectos a grupos específicos de elementos.

Aquí hay un ejemplo de cómo se usa la etiqueta `<div>` en HTML:

```html
<div id="contenedor">
    <h1>Título</h1>
    <p>Este es un párrafo dentro del contenedor.</p>
    <img src="imagen.jpg" alt="Imagen">
</div>
```

<br>

En este ejemplo, `<div id="contenedor">` crea un contenedor alrededor de un título (`<h1>`), un párrafo (`<p>`) y una imagen (`<img>`). Puedes aplicar estilos CSS al contenedor para darle un formato específico o manipularlo con JavaScript utilizando su identificador (`id`) como referencia.

Los `<div>` se utilizan principalmente para organizar y estructurar el contenido, permitiendo un diseño más flexible y una separación clara entre diferentes partes de una página web. También se utilizan para implementar diseños sensibles (responsive) y para aplicar estilos específicos a secciones del contenido.

### Solución 

```html

<!DOCTYPE html>
<html>
<head>
	<title>Ejercicio html etiquetas de texto básicas</title>
	<meta charset="utf-8"/>
	<style>
		div{
		   border: 1px solid #000000;	
		   padding: 5px  10px;
		}
		#main{
			display:flex;
		}
		#footer {
			display: flex;
			flex-wrap: wrap;
		}

		#footer > div {
			flex: 1;
			min-width: 0; /* Para evitar que el contenido fuerce el tamaño de la sección */
		}

		#nav{
			margin-top: 5px;
		}

	</style>
</head>
<body>
     <div id="wrapper">
           <div id="header">
               <img width="50px" height="50px"  src="https://www.zarla.com/images/zarla-redata-1x1-2400x2400-20211214-qcmpq7w86rx4wybrffy9.png?crop=1:1,smart&width=250&dpr=2" alt="logotipo"/>
			   <a href="tel:975757575" title="Llámemos">975757575</a>
			   <div id="nav">
				   <ul>
					   <li><a href="">Servicios</a></li>
					   <li><a href="">Blog</a></li>
					   <li><a href="">Contacto</a></li>
				   </ul>
			   </div>
		   </div>
	
	 <div id="container">
          <div id="main">
              <div id="section1" >
                    <h1>Un titulo muy representativo</h1>
					 <p>Lorem Ipsum es simplemente el texto de relleno de las imprentas y archivos de texto. Lorem Ipsum ha sido el texto de relleno estándar de las industrias desde el año 1500, cuando un impresor (N. del T. persona que se dedica a la imprenta) desconocido usó una galería de textos y los mezcló de tal manera que logró hacer un libro de textos especimen. No sólo sobrevivió 500 años, sino que tambien ingresó como texto de relleno en documentos electrónicos, quedando esencialmente igual al original. Fue popularizado en los 60s con la creación de las hojas "Letraset", las cuales contenian pasajes de Lorem Ipsum, y más recientemente con software de autoedición, como por ejemplo Aldus PageMaker, el cual incluye versiones de Lorem Ipsum.</p>
					 <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
			  </div>
			  <div id="section2">
				    <video controls src="https://www.youtube.com/watch?v=grScJAcO45g"></video>
					<div id="article1">
						<h2>Un section 2</h2>
						<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
						<a href="" title="ir a...">Saber más</a>
					</div>
			  </div>
			  <div id="section3">
				  <div id="article2">
					  <h2>Un section 3</h2>
					  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
					  <a href="" title="ir a...">Saber más</a>
				  </div>
				  <audio controls src=""></audio>
			  </div>
		  </div>
	 </div>
	 <div id="footer">
		  <div id="section4">
                <h3>Sobre mi</h3>			   
				<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
					tempor incididunt.</p>
				<a href="#header">Subir</a>
		  </div>
		  <div id="section5">
               <h3>Horarios</h3>
			   <p>Mañanas:9.00-13.00<br/>Tardes:16.00-19.00<br/>Domingo cerrado.</p>
		  </div>
		  <div id="section6">
			<img src="" alt="ISO9001"/>
			<img src="" alt="ISO14001"/>
		</div>
		 
	 </div>
</body>
</html>



```


## Taller en clase 

![image](https://github.com/crodrigr/diseno-web-avanzado-uts-2023-02/assets/31961588/9b8fc6cf-b1b3-4938-837e-e3bd00729148)

