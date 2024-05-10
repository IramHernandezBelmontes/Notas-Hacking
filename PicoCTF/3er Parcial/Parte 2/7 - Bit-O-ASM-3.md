
## Descripción
Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Download the assembly dump [here](https://artifacts.picoctf.net/c/530/disassembler-dump0_c.txt).
## Pistas 
Not everything in this disassembly listing is optimal.
## Solución
se almacena el valor de 0x9fe1a y 4 los cuales se multiplican,  se suma 0x1f5 al resultado de la multiplicación y su resultado es nuestra flag (eax)

El valor final almacenado en eax será (0x9fe1a × 4) + 0x1f5. Convirtiendo 0x9fe1a a decimal, tenemos 654874. M ultiplicando por 4, obtenemos 2619496. Al sumar 501, obtenemos 2619997`.
## Bandera
picoCTF{2619997}