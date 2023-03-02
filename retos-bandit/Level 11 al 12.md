### Bandit Level 11 → Level 12

## Objetivo
The password for the next level is stored in the file **data.txt**, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions.

## Datos de acceso al nivel
bandit11
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

## Solución
Forma 1
bandit11@bandit:~$ ls 
data.txt 
bandit11@bandit:~$ cat data.txt 
Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi bandit11@bandit:~$ cat data.txt | tr [a-zA-Z] [n-za-mN-ZA-M] 
The password is JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv bandit11@bandit:~$

Forma 2 
bandit11@bandit:~$ ls 
data.txt 
bandit11@bandit:~$ cat data.txt 
Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi bandit11@bandit:~$ python3 
Python 3.10.6 (main, Nov 14 2022, 16:10:14) [GCC 11.3.0] on linux 
Type "help", "copyright", "credits" or "license" for more >>>information.
>>>import codecs
 codecs.decode('Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi','rot13')
  'The password is JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv' 
  >>> bandit11@bandit:~$

## Notas adicionales

| comando | descripción |
|-----|-----|
| cat | muestra el contenido de un archivo |
| ls | listar archivos |
| cd | sirve para mostrar el nombre del directorio actual |
| grep | es una herramienta de líneas de comando usada para buscar cadenas de texto |
| sort | Ordenar en orden alfabético|
| find | Busca el archivo file|
| uniq |  sirve para mostrar en pantalla aquellas líneas o palabras que se repitan|

## Referencias
[Over The Wire: Bandit Write Up](https://jwuk.files.wordpress.com/2016/05/writeup1.pdf)
[OTW](https://axcheron.github.io/writeups/otw/bandit/)
