### Bandit Level 12 → Level 13

## Objetivo
The password for the next level is stored in the file **data.txt**, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Datos de acceso al nivel
bandit12
JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

## Solución
Algunos tipos de compresion en Linux
ext           comp      desc                                ver en consola
.gz            gzip        gzip -d   (gunzip)             zcat 
.bz2          bzip2      bzip2 -d   (bunzip2)         bzcat
.tar           tar           tar xf                                 tar xO 

otros (instalar) :
.zip    zip     unzip (7z x)
.rar    rar      unrar (7z x)

## Notas adicionales

| comando | descripción |
|-----|-----|
| cat | muestra el contenido de un archivo |
| mv | mover archivos y directorios de un directorio a otro o para renombrar un archivo o directorio |
| cd | sirve para mostrar el nombre del directorio actual |
| tar | archiva y recupera archivos en y a partir de un solo archivo denominado tarfile|
| base64 | Permite codificar y decodificar y decodificar cadenas de caracteres desde linea de comandos en Linux|
| bzip2 | comprime ficheros utilizando el algoritmo de comprension de texto por ordenacion de bloques de Burrows-Where|
## Referencias
[Over The Wire: Bandit Write Up](https://jwuk.files.wordpress.com/2016/05/writeup1.pdf)
[OTW](https://axcheron.github.io/writeups/otw/bandit/)
[Comando bzip2 ](https://www.google.com/search?q=comando+bzip2+en+linux+que+gace&rlz=1C1UEAD_esMX1021MX1021&oq=comando+bzip2+en+linux+que+gace&aqs=chrome..69i57j33i10i160.10650j0j7&sourceid=chrome&ie=UTF-8)
[Comando tar](https://docs.oracle.com/cd/E19620-01/805-5917-10/z400009a1190/index.html#:~:text=El%20comando%20tar%20archiva%20y,tratarse%20de%20un%20archivo%20cualquiera.)