## Descripción
The one time pad can be cryptographically secure, but not when you know the key. Can you solve this? We've given you the encrypted flag, key, and a table to help `UFJKXQZQUNB` with the key of `SOLVECRYPTO`. Can you use this [table](https://jupiter.challenges.picoctf.org/static/1fd21547c154c678d2dab145c29f1d79/table.txt) to solve it?.
## Pistas 
Submit your answer in our flag format. For example, if your answer was 'hello', you would submit 'picoCTF{HELLO}' as the flag.

Please use all caps for the message.
## Solución
al analizar el contenido del archivo podemos apreciar un cifrado de Vigenère un algoritmo evolucionado del cifrado de Cesar, por lo que usaremos la herramienta de la pagina https://es.planetcalc.com/2468/ la cual al colocar el texto cifrado y la llave este nos regresa la flag

![[easy  1.png]]
## Bandera
picoCTF{cryptoisfun}