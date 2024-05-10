## Descripción
Can you figure out what is in the `eax` register at the end of the `main` function? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Disassemble [this](https://artifacts.picoctf.net/c/512/debugger0_a).
## Pistas 
gdb is a very good debugger to use for this problem and many others!

`main` is actually a recognized symbol that can be used with gdb commands.
## Solución
para este reto utilizaremos la herramienta ghydra para realizarle ingenieria inversa al programa de linux, una vez que estemos dentro del programa buscaremos la funcion main, donde encontraremos 

undefined8 main(void)

{
  return 0x86342;
}

ese 0x86342 lo convertiremos a decimal el cual es 549698 y esa es nuestra flag


![[gdb1.png]]

## Bandera
picoCTF{549698}