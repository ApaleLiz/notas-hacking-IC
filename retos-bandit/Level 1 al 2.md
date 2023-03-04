
###  Bandit Level 1 → Level 2

## Objetivo
The password for the next level is stored in a file called **-** located in the home directory
## Datos de acceso al nivel
bandit1
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

## Solución
```
bandit1@bandit:~$ ls - bandit1@bandit:~$ cat - ^C bandit1@bandit:~$ cat ./- rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi bandit1@bandit:~$ pwd /home/bandit1 bandit1@bandit:~$ cat /home/bandit1/- rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi bandit1@bandit:~$
```
## Notas adicionales
| comando | dscripción |
|-----|-----|
| cat | muestra el contenido de un archivo |
| ls | listar archivos |
| file |determinar el tipo y formato de un archivo |
| find | buscar archivos y directorios en la línea de comandos de Linux |

## Referencias
[Over The Wire: Bandit Write Up](https://jwuk.files.wordpress.com/2016/05/writeup1.pdf)
[OTW](https://axcheron.github.io/writeups/otw/bandit/)

