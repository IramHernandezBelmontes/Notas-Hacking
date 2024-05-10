## Descripción
Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Download the assembly dump [here](https://artifacts.picoctf.net/c/511/disassembler-dump0_d.txt).
## Pistas 
Don't tell anyone I told you this, but you can solve this problem without understanding the compare/jump relationship.

Of course, if you're really good, you'll only need one attempt to solve this problem.
## Solución
Un valor inicial de `0x9fe1a` (654874 en decimal) se asigna a una posición de memoria.

Se compara el valor asignado con `0x2710` (10000 en decimal).
Si el valor es menor o igual a `10000`, el código ejecuta una suma.
Si es mayor que `10000`, se realiza una resta.

Dado que el valor `0x9fe1a` (654874) es mayor que 0x2710, se resta 0x65 (101 en decimal).

- Después de la resta, el valor es 654874 - 101 = 654773.
- Este valor se almacena en el registro eax`.
`

El valor final en eax es 654773 en decimal, después de restar 101 de 654874.
## Bandera
picoCTF{654773}