## Descripción
We have recovered a [binary](https://jupiter.challenges.picoctf.org/static/7aa5f383ec616fe9d72c2ffe1fabd0d9/rev) and a [text file](https://jupiter.challenges.picoctf.org/static/7aa5f383ec616fe9d72c2ffe1fabd0d9/rev_this). Can you reverse the flag.
## Pistas 
objdump and Gihdra are some tools that could assist with this
## Solución
vamos a descargar la herramienta ghidra para ver el contenido del archivo, vamos a buscar la funcion main en donde podemos ver como se ejecuta el archivo, lo que nos interesa es como mueve los valores de la lafg por lo que extraemos los valores de operaciones, haciendo unas adaptaciones al codigo utilziamos el siguiente codigo

flag = "picoCTF{w1{1wq84fb<1>49}"


flagrev = ''


for i in range(8, len(flag)):

    if (i & 1) == 0:
        flagrev += chr(ord(flag[i]) - 5)  
    else:
        flagrev += chr(ord(flag[i]) + 2)  


print("Resultado:", flagrev) 

## Bandera

picoCTF{r3v3rs36ad73964}