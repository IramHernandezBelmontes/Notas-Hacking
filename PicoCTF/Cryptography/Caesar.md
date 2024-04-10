## Descripción
Decrypt this [message](https://jupiter.challenges.picoctf.org/static/49f31c8f17817dc2d367428c9e5ab0bc/ciphertext).
## Pistas 
caesar cipher [tutorial](https://learncryptography.com/classical-encryption/caesar-cipher)
## Solución
primero aplicamos file al archivo para ver que tipo es, este archivo resulta ser un archivo sumamente grande que el editor no pude abrir por lo que para sacar el contenido  utilizaremos un grep "picoCTF{.*} ciphertext" es este nos devolvera la flag 

![[caesar 1.png]]
pero podemos apreciar que el contenido dentro de los corchetes esta cifrado por lo quedó debemos descifrarlo, en mi caso usare la pagina de https://caesarcipher.net/ el cual nos solicitara el código de texto y una llave en la cual basarse, utilice la llave 4 y este me arrojo el contenido des encriptado de la flag

![[caesar 2.png]]
## Bandera 
picoCTF{crossingtherubiconvfhsjkou}