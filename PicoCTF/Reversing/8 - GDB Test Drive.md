## Descripción
Can you get the flag?Download this [binary](https://artifacts.picoctf.net/c/85/gdbme).Here's the test drive instructions:

- `$ chmod +x gdbme`
- `$ gdb gdbme`
- `(gdb) layout asm`
- `(gdb) break *(main+99)`
- `(gdb) run`
- `(gdb) jump *(main+104)`
## Pistas 
none
## Solución
para este problema vamos a descargar un programa que se llama gdb el cual nos permite leer código assembly, seguimos las instrucciones y nos dará la flag
## Bandera

picoCTF{d3bugg3r_dr1v3_197c378a}