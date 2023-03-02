### Bandit Level 5 → Level 6

## Objetivo
The password for the next level is stored **somewhere on the server** and has all of the following properties:

-   owned by user bandit7
-   owned by group bandit6
-   33 bytes in size

## Datos de acceso al nivel
bandit5
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

## Solución
bandit5@bandit:~$ ls 
inhere 
bandit5@bandit:~$ cd inhere/ 
bandit5@bandit:~/inhere$ ls
maybehere00 maybehere04 maybehere08 maybehere12 maybehere16 maybehere01 maybehere05 maybehere09 maybehere13 maybehere17 maybehere02 maybehere06 maybehere10 maybehere14 maybehere18 maybehere03 maybehere07 maybehere11 maybehere15 maybehere19 bandit5@bandit:~/inhere$ find . -readable -type f -size 1033c ./maybehere07/.file2 
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2 P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

## Notas adicionales

| comando | descripción |
|-----|-----|
| cat | muestra el contenido de un archivo |
| ls | listar archivos |
| cd | **sirve** para mostrar el nombre del directorio actual |
| file |determinar el tipo y formato de un archivo |
| du |se utiliza para estimar la cantidad **de** espacio en disco utilizado por un archivo o directorio |

## Referencias
[Over The Wire: Bandit Write Up](https://jwuk.files.wordpress.com/2016/05/writeup1.pdf)
[OTW](https://axcheron.github.io/writeups/otw/bandit/)
