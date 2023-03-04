### Bandit Level 6 → Level 7

## Objetivo
The password for the next level is stored **somewhere on the server** and has all of the following properties:

-   owned by user bandit7
-   owned by group bandit6
-   33 bytes in size

## Datos de acceso al nivel
bandit6 
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

## Solución
```
bandit6@bandit:~$ ls 
bandit6@bandit:~$ ls -la 
total 20
drwxr-xr-x 2 root root 4096 Jan 11 19:18 .
drwxr-xr-x 70 root root 4096 Jan 11 19:19 ..
-rw-r--r-- 1 root root 220 Jan 6 2022 .bash_logout 
-rw-r--r-- 1 root root 3771 Jan 6 2022 .bashrc 
-rw-r--r-- 1 root root 807 Jan 6 2022 .profile 
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null /
var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
bandit6@bandit:~$
```

## Notas adicionales

| comando | descripción |
|-----|-----|
| cat | muestra el contenido de un archivo |
| ls | listar archivos |
| cd | **sirve** para mostrar el nombre del directorio actual |
| file |determinar el tipo y formato de un archivo |
| grep | es una herramienta de líneas de comando usada para buscar cadenas de texto |

## Referencias
[Over The Wire: Bandit Write Up](https://jwuk.files.wordpress.com/2016/05/writeup1.pdf)
[OTW](https://axcheron.github.io/writeups/otw/bandit/)
