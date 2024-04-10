## Descripción
We made a lot of substitutions to encrypt this. Can you decrypt it? Connect with `nc jupiter.challenges.picoctf.org 13758`.
## Pistas 
Flag is not in the usual flag format
## Solución
al momento de ejecutar el comando nos regresa un texto encriptado el cual no conocemos en un principio de que es
![[waves o lamba 1.png]]
utilizamos la pagina web  https://www.dcode.fr/identificador-cifrado para  detectar ante que cifrado nos encontramos el cual nos arroja varios resultados
![[lambda 2.png]]

utilizamos el cifrado de vingere el cual no nos arroja nada, decidimos utilizar el cifrado mono-alphabetic Sustitution y decriptamos automaticamente el cual nos regresa este resultado 

![[lambda 3.png]]

aqui podemos ver que el texto esta mal escrito, solamente acomodamos las letras para que tenga sentido el texto y queda asi

![[lambda 4.png]]
## Bandera
FREQUENCY_IS_C_OVER_LAMBDA_DNVTFRTAYU