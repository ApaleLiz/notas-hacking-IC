### Bandit Level 10 → Level 11

## Objetivo
The password for the next level is stored in the file **data.txt**, which contains base64 encoded data

## Datos de acceso al nivel
bandit10 
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

## Solución
```
bandit10@bandit:~$ ls
data.txt 
bandit10@bandit:~$ cat data.txt VGhlIHBhc3N3b3JkIGlzIElGdWt3S0dzRlc4TU9xM0lSRnFyeEUxaHhUTkViVVBSCg== 
bandit10@bandit:~$ 
bandit10@bandit:~$ echo "hola mundo"
hola mundo
bandit10@bandit:~$ echo "hola mundo" | base64 aG9sYSBtdW5kbwo=
bandit10@bandit:~$ echo -n aG9sYSBtdW5kbwo= | base64 -d
hola mundo 
bandit10@bandit:~$ base64 -d data.txt
The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR bandit10@bandit:~$ 
bandit10@bandit:~$ cat data.txt VGhlIHBhc3N3b3JkIGlzIDZ6UGV6aUxkUjJSS05kTllGTmI2blZDS3pwaGxYSEJNCg==
bandit10@bandit:~$ cat data.txt | base64 -d
The password is 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
```

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
| base64 | Permite codificar y decodificar y decodificar cadenas de caracteres desde linea de comandos en Linux|


## Referencias
[Over The Wire: Bandit Write Up](https://jwuk.files.wordpress.com/2016/05/writeup1.pdf)
[OTW](https://axcheron.github.io/writeups/otw/bandit/)
[Comando Uniq](https://nksistemas.com/comando-uniq-de-linux-explicado-con-ejemplos/#:~:text=Uniq%20es%20un%20comando%20que,como%20funciona%20con%20un%20simple)