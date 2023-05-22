## Descripcipción

Our data got corrupted on the way here. Luckily, nothing got replaced, but every block of 3 got scrambled around! The first word seems to be three letters long, maybe you can use that to recover the rest of the message.Download the corrupted message [here](https://artifacts.picoctf.net/c/191/message.txt).

## Pistas

-  Split the message up into blocks of 3 and see how the first block is scrambled

## Solucion

```
apaleliz-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/191/message.txt
--2023-05-22 00:14:04--  https://artifacts.picoctf.net/c/191/message.txt
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 108.156.172.6, 108.156.172.74, 108.156.172.120, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|108.156.172.6|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 54 [application/octet-stream]
Saving to: 'message.txt.3'

message.txt.3       100%[==================>]      54  --.-KB/s    in 0s      

2023-05-22 00:14:05 (28.0 MB/s) - 'message.txt.3' saved [54/54]

apaleliz-picoctf@webshell:~$ cat message.txt.3
heTfl g as iicpCTo{7F4NRP051N5_16_35P3X51N3_V6E5926A}4

- PEGAR LA BANDERA EN LA SIGUIENTE PAGINA https://tholman.com/other/transposition/
- PONER 3 COLUMNAS
- LAS TERCERA SE PASA AL PRINCIPIIO Y TE DA LA BANDERA
```

## Bandera
picoCTF{7R4N5P051N6_15_3XP3N51V3_56E6924A}