## Descripción
What does asm2(0x4,0x2d) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/ceac75672637589213b952abe32c84b3/test.S)
## Pistas 
assembly [conditions](https://www.tutorialspoint.com/assembly_programming/assembly_conditions.htm)
## Solución
para esta flag  se nos da la información de que  regresa 0x2e0

sabemos que 0x2e0 = ebp y a esp

al movernos a la linea  +3 este nos hara una condición en la que se comparara 
0x2e0 > 0x3fb

al ser false este se salta a la linea +12 para compararse con 0x280

0x2e0 >  0x280

al ser  true la line nos manda a la linea +29 donde el valor true ( 0x2e0) le suma 0x8 para convertirlo en eax

la siguiente instrucción eax,0xa nos pide una resta de los valores en hexadecimal la cual nos  regresa
(0x2e0 - 0xa)
0x2d6 la cual es nuestra flag


## Bandera
0x2d6