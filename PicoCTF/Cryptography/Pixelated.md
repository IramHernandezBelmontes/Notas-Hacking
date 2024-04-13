## Descripción
I have these 2 images, can you make a flag out of them? [scrambled1.png](https://mercury.picoctf.net/static/9f2d081f12c05202359632c1989e7927/scrambled1.png) [scrambled2.png](https://mercury.picoctf.net/static/9f2d081f12c05202359632c1989e7927/scrambled2.png)
## Pistas 
[https://en.wikipedia.org/wiki/Visual_cryptography](https://en.wikipedia.org/wiki/Visual_cryptography)
Think of different ways you can "stack" images
## Solución
para este problema utilizaremos la herramienta de kali de nombre
"**ImageMagick**" esta herramienta nos permite combinar imagenes en este caso importantes ya que se tratan de 2 imagenes, el estilo de cryptografia es visual Cryptography, despues de usar algunos comandos el que funciono fe el siguiente

"convert  scrambled1.png scrambled2.png -compose Add -composite imagen_resultante.png"
 este te regresa la imagen con la flag

add suma los rojos, verdes y azules para dar la imagen resultante

![[scrambled.jpg]]
## Bandera

picoCTF{7188864c}
