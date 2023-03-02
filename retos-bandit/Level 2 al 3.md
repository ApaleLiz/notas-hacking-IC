### Bandit Level 2 → Level 3

## Objetivo
The password for the next level is stored in a file called **spaces in this filename** located in the home directory

## Datos de acceso al nivel
bandit2
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

## Solución
bandit2@bandit:~$ ls
spaces in this filename
bandit2@bandit:~$ cat spaces in this filename
cat: spaces: No such file or directory 
cat: in: No such file or directory 
cat: this: No such file or directory 
cat: filename: No such file or directory bandit2@bandit:~$ cat spaces\ in\this\ filename 
aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG 
bandit2@bandit:~$ cat "spaces in this filename" aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG 
bandit2@bandit:~$

## Notas adicionales

| comando | dscripción |
|-----|-----|
| cat | muestra el contenido de un archivo |
| ls | listar archivos |
| cd | **sirve** para mostrar el nombre del directorio actual |
| file |determinar el tipo y formato de un archivo |


## Referencias
[Over The Wire: Bandit Write Up](https://jwuk.files.wordpress.com/2016/05/writeup1.pdf)
[OTW](https://axcheron.github.io/writeups/otw/bandit/)
