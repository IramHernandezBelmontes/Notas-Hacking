## Descripción
What does asm2(0x4,0x2d) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/ceac75672637589213b952abe32c84b3/test.S)
## Pistas 
assembly [conditions](https://www.tutorialspoint.com/assembly_programming/assembly_conditions.htm)
## Solución
para esta solucion vamos  a meter los 2 valores a ebp = 0xc  y ebp = ox8 a estos valores les vamos a sumar los valores que nos de en la linea 20 y 24, estro va a generar un ciclo el cual nos pedira llegar  al  valor de la ounea 24, para eso vamos a tomar ebp + 0xc y lo vamos a dividir entre lo que nos da la linea 31 y esa  va a ser nuestra flag
## Bandera

0xa3