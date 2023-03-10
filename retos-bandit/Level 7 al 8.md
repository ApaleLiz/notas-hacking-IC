### Bandit Level 7 → Level 8

## Objetivo
The password for the next level is stored in the file **data.txt** next to the word **millionth**

## Datos de acceso al nivel
bandit7
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

## Solución
```
bandit7@bandit:~$ ls
data.txt 
bandit7@bandit:~$ wc data.txt 
98567 197133 4184396 data.txt 
bandit7@bandit:~$ grep millionth data.txt
millionth TESKZC0XvTetK0S9xNwm25STk5iWrBvP 
bandit7@bandit:~$ cat data.txt | grep 
millionth millionth TESKZC0XvTetK0S9xNwm25STk5iWrBvP bandit7@bandit:~$
```

## Notas adicionales

| comando | descripción |
|-----|-----|
| cat | muestra el contenido de un archivo |
| ls | listar archivos |
| cd | **sirve** para mostrar el nombre del directorio actual |
| grep | es una herramienta de líneas de comando usada para buscar cadenas de texto |

## Referencias
[Over The Wire: Bandit Write Up](https://jwuk.files.wordpress.com/2016/05/writeup1.pdf)
[OTW](https://axcheron.github.io/writeups/otw/bandit/)
