## Descripción
Can you get the flag?Here's the [website](http://saturn.picoctf.net:64403/).We know that the website files live in `/usr/share/nginx/html/` and the flag is at `/flag.txt` but the website is filtering absolute file paths. Can you get past the filter to read the flag?
## Pistas 
none
## Solución
usamos la busqueda relativa de direcciones con 4 "../"
![[Forbiden paths.png]]
## Bandera
picoCTF{7h3_p47h_70_5ucc355_e5fe3d4d}