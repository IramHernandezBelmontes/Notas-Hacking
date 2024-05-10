## Descripción
Can you figure out what is in the `eax` register at the end of the `main` function? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Debug [this](https://artifacts.picoctf.net/c/520/debugger0_b).
## Pistas 
You could calculate `eax` yourself, or you could set a breakpoint for after the calculcation and inspect `eax` to let the program do the heavy-lifting for you.
## Solución
al momento de ver la funcion main con  ghydra nos encontramos con una funcion for, 

donde:

local_c = 0x1e0da que su valor decimal seria: 123,098

local_10 va de 0 a 606 ya que este bucle termina cuando llega a 607, al final suma los 2 valores y esta suma seria nuestra flag

1e0da  en hexadecimal es igual a:
    1 * 16^4 = 1 * 65536 = 65536`
    e * 16^3 = 14 * 4096 = 57344`
    0 * 16^2 = 0`
    d * 16^1 = 13 * 16 = 208`
    a * 16^0 = 10 * 1 = 10
    
sumando su valor es 123098

despues vamos a hacer 606 * 607 el cual nos da 367,842, eso lo vamos a dividir entre 2 y nos da 183,921

por ultimo vamos a sumarlos 183,921 + 123,098 = 307019


## Bandera
picoCTF{307019}