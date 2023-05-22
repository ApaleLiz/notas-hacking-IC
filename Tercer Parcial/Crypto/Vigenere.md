## Descripcipción

Can you decrypt this message?Decrypt this [message](https://artifacts.picoctf.net/c/160/cipher.txt) using this key "CYLAB".

## Pistas

-   https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher

## Solucion

```
apaleliz-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/160/cipher.txt
--2023-05-22 00:20:33--  https://artifacts.picoctf.net/c/160/cipher.txt
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 108.156.172.6, 108.156.172.42, 108.156.172.120, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|108.156.172.6|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 43 [application/octet-stream]
Saving to: 'cipher.txt'

cipher.txt          100%[==================>]      43  --.-KB/s    in 0s      

2023-05-22 00:20:33 (17.5 MB/s) - 'cipher.txt' saved [43/43]

apaleliz-picoctf@webshell:~$ cat cipher.txt
rgnoDVD{O0NU_WQ3_G1G3O3T3_A1AH3S_2951c89f}

-PEGAR EN LA SIG LIGA https://www.boxentriq.com/code-breaking/vigenere-cipher
-PONER LA BANDERA PARA DECODIFICAR
- LLAVE CYLAB
- TE DA LA BANDERA
```

## Bandera
picoCTF{D0NT_US3_V1G3N3R3_C1PH3R_2951a89h}