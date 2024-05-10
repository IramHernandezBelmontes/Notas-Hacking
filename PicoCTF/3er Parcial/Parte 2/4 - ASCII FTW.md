## Descripción
#### Description

This program has constructed the flag using hex ascii values. Identify the flag text by disassembling the program.You can download the file from [here](https://artifacts.picoctf.net/c/508/asciiftw).
## Pistas 
The combined range of hex-ascii for English alphabets and numerical digits is from 30 to 7A.

Online hex-ascii converters can be helpful.
## Solución
para este codigo utilizaremos ghidra para   realziar reversing, donde   al momento de explorar la funcion main esta nos  dice que  la flag inicia con 0x70  que en ASCII represeta una   P

al momento de indagar no mucho en el programa podemos apreciar lo siguitente

![[ASCCI FTW.png]]

inicia con 0x70, al momento de pasar cada valor hexadecimal a  una calculadora esta es la flag

![[ASCCI FTW222.png]]
## Bandera

picoCTF{ASCII_IS_EASY_8960F0AF}