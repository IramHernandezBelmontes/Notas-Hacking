## Descripción
Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Download the assembly dump [here](https://artifacts.picoctf.net/c/510/disassembler-dump0_b.txt).
## Pistas 
`PTR`'s or 'pointers', reference a location in memory where values can be stored.
## Solución
al momento de ver el registro eax este nos manda a  DWORD PTR [rbp-0x4],0x9fe1a

0x9fe1a lo tenemos que convertir a decimal, donde

A(10 en decimal) x 16^0 = 10
 1  1 × 16^1 = 16`
 E (14 en decimal): 14 × 16^2 = 3584`
 F (15 en decimal): 15 × 16^3 = 61440`
9: 9 × 16^4 = 589824`

sumamos 10 + 16 +3584 + 61440 + 589824 =  654874

la bandera es 654874
## Bandera
picoCTF{654874}