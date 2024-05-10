## Descripción
I wonder what this really is... [enc](https://mercury.picoctf.net/static/e47483f88b12f2ab0c46315afc12f64d/enc) `''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])`
## Pistas 
You may find some decoders online
## Solución
para este problema convertiremos el texto a char y de char a hedump con cyberchef, el cual nos dara la bandera
## Bandera
picoCTF{16_bits_inst34d_of_8_e141a0f7}