# Práctica Cuadros de Velázquez
## Creación de entorno en local
Lo primero que hice fue crear la estructura de manera ==**LOCAL**==
Cree una carpeta llamada práctica 1 con los siguientes documentos:
1. Con cinco documentos HTML llamados:
   1.1 ``` index.html ```
   1.2 ``` venus.html ```
   1.3 ```meninas.html```
   1.4 ```vulcano.html```
   1.5 ```inocencio.html```
2. También un documento css llamado ```estilos.css```.
3. Un pequeño documento javascript llamado ```scripts.js```.
4. Un documento llamado ```README.md```, es el documento que visualizas actualmente y es donde explico como ejecuto la realización de la práctica.
5. También dentro ahí un directorio llamado **img** donde se almacenan las imágenes que utilizo en la página.
6. Por último, tendremos que crear el documento ```.gitignore```, con ello podremos hacer que archivos que se encuentran en el directorio y no queremos que se suban al repositorio de GitHub, por ejemplo ```.idea```.
   En la imagen siguiente se puede observar todos ellos:
   ![](img\archivos.png)
## Creación del entorno en GitHub
Después, lo que hice fue iniciar el repositorio de GitHub, a continuación voy a explicar los comandos en orden de ejecución desde PowerShell:
Lo primero que tengo que hacer es iniciar el repositorio, mediante el comando:
```git
 git init
```
Mientras en GitHub, crearemos un repositorio, y mediante los siguientes comandos, les conectaremos con local:
```git
git branch -M main
git remote add origin https://github.com/lauraamor/practica1.git
git push -f -u origin main
```
Con estos comandos lo que haremos es crear la rama ```main``` y añadirlo al repositorio remoto.
Cada vez que queramos subir algo al repositorio remos ejecutaremos estos comandos:
* ```git add .```  Para agregar la preparación de los ficheros a añadir
* ```git commit -m "comentario"``` Con el confirmaremos que todos los archivos agregados queremos que se suban, y con -m pondremos un pequeño comentario para diferenciarlos de todos.
* ```git push -u ``` Con este último les subiremos al repositorio remoto.
A continuación comentaré los aspectos más interesantes que me ha parecido en cada parte:
## HTML
En HTML las principales etiquetas principales que he utilizado son:
* ```<header>``` Con ella he hecho el encabezado de la página, donde he puesto el título
* ```<div>``` Con ella lo que he hecho es diferenciar las distintas partes del cuadro y de la información del cuadro.
* ```<nav>``` En ella he colocado dentro el menú lateral, ya que es un elemento de navegación.
*  ```<button>``` Con esta etiqueta he creado el botón de compra.
## CSS
En CSS con lo que ahí que practicar para que quede muy parecida es con las etiquetas: 
```CSS
position:;
overflow:;
```
Con la etiqueta ```position```, he utilizado las propiedades ```relative``` y ```absolute```, para las posiciones del menú lateral, de la imagen del cuadro, y de la información del cuadro.
Con la etiqueta ```overflow```, utilice la propiedad ```auto```, para que apareciese el scroll en el menú lateral.
Las anteriores son las etiquetas más importantes a la hora de maquetar.

La etiqueta que me ha parecido más interesante en **CSS**, ha sido la etiqueta ```filter: grayscale```, para poner en blanco y negro las imágenes del menú.

Después de esas etiquetas he contenido con las típicas como ````widht```` o ```heigt```, para conseguir un resultado parecido.
## JavaScript
En este documento lo único que he utilizado es para abrir la imagen en grande con el siguiente código:
```JavaScript
function grande_breda() {
    open("/img/breda.jpg");
}
```
Mientras en el **HTML** he añadido la función, para que así se ejecutase:
```JavaScript
onclick="grande_breda()"
```
# Posibles mejoras
Una de las mejoras que me gustaría haber implementado, es que los cuadros se cambien todos en la misma página, es decir solo existir el ````index.html````, y mediante JavaScript que se cambie.
También, es que la imagen en grande se abra y cierre con un clic en la misma ventana no en una nueva.
