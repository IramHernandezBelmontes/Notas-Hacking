## Descripción
How about we take you on an adventure on exploring certificate signing requestsTake a look at this CSR file [here](https://artifacts.picoctf.net/c/421/readmycert.csr).
## Pistas 
Download the certificate signing request and try to read it.
## Solución
al descargar el archivo certificado le cambiamos su valor a txt, al ver el contenido podemos darnos cuenta que parece ser una llave SSH, pero al ver el signo de igual "=" sabemos que es base64, decriptamos el archivo y salen valores incongruentes pero al principio sale la flag junto con un "cftPlayer"

![[ReadMyCert.png]]
## Bandera
picoCTF{read_mycert_3aa80090}