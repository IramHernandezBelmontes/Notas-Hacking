## Descripción
This vault uses ASCII encoding for the password. The source code for this vault is here: [VaultDoor4.java](https://jupiter.challenges.picoctf.org/static/c695ee23309d453a3ef369c34cc1bccb/VaultDoor4.java)
## Pistas 
Use a search engine to find an "ASCII table".

You will also need to know the difference between octal, decimal, and hexadecimal numbers.
## Solución
para esta solucion podemos ver que la clave viene en partes de distintos tipos de formato, concretamente en, ASCII, Hexadecimales y octales, la ultima parte corresponde a la clave unica de la flag

usamos cyber chef para cada  parte con su respectivo formato y este nos devolvera la flag en partes
## Bandera
picoCTF{jU5t_4_bunCh_0f_bYt3s_8f4a6cbf3b}