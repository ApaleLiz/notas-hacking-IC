### Bandit Level 9 → Level 10

## Objetivo
The password for the next level is stored in the file **data.txt** in one of the few human-readable strings, preceded by several ‘=’ characters.

## Datos de acceso al nivel
bandit9 
EN632PlfYiZbn3PhVK3XOGSlNInNE00t

## Solución
```
bandit9@bandit:~$ ls
data.txt 
bandit9@bandit:~$ file data.txt 
data.txt: data 
bandit9@bandit:~$ strings data.txt | grep ==
c========== the
h;========== password 
========== isT 
n.E========== G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s bandit9@bandit:~$
```

## Notas adicionales

| comando | descripción |
|-----|-----|
| cat | muestra el contenido de un archivo |
| ls | listar archivos |
| cd | **sirve** para mostrar el nombre del directorio actual |
| grep | es una herramienta de líneas de comando usada para buscar cadenas de texto |
| sort | Ordenar en orden alfabético|
| find | Busca el archivo file|

## Referencias
[Over The Wire: Bandit Write Up](https://jwuk.files.wordpress.com/2016/05/writeup1.pdf)
[OTW](https://axcheron.github.io/writeups/otw/bandit/)
