## Descripción
We found this weird message being passed around on the servers, we think we have a working decryption scheme.Download the message [here](https://artifacts.picoctf.net/c/128/message.txt).Take each number mod 37 and map it to the following character set: 0-25 is the alphabet (uppercase), 26-35 are the decimal digits, and 36 is an underscore.Wrap your decrypted message in the picoCTF flag format (i.e. `picoCTF{decrypted_message}`)
## Pistas 
Do you know what `mod 37` means?

`mod 37` means modulo 37. It gives the remainder of a number after being divided by 37.
## Solución
para este dato decifrado vamos a la pagina de https://www.dcode.fr/modulo-cipher donde pondremos en la opcion ModuloN 37 y este nos dara en uno de los resultados "R0UND N R0UND B6B25531" unicamente ponemos el formato de pico y tenemos la bandera
## Bandera
picoCTF{R0UND_N_R0UND_B6B25531}