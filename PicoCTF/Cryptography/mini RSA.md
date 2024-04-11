## Descripción
Let's decrypt this: [ciphertext](https://jupiter.challenges.picoctf.org/static/ee7e2388b45f521b285334abb5a63771/ciphertext)? Something seems a bit small.
## Pistas 
RSA [tutorial](https://en.wikipedia.org/wiki/RSA_(cryptosystem))

How could having too small an e affect the security of this 2048 bit key?

Make sure you don't lose precision, the numbers are pretty big (besides the e value)
## Solución
para solucionar este reto tendremos que investigar que es ciframiento RSA, una vez comrpendido vamos a utilizar la pagina https://www.dcode.fr/rsa-cipher donde ingresaremos las los datos de las letras correspondientes y esto nos dara la flag

![[mini RSA.png]]
## Bandera
picoCTF{n33d_a_lArg3r_e_606ce004}