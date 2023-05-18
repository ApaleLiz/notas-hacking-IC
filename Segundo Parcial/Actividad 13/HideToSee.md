## Descripcipción

How about some hide and seek heh?Look at this image [here](https://artifacts.picoctf.net/c/237/atbash.jpg).

## Pistas

-   Download the image and try to extract it.

## Solucion

```
apaleliz-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/237/atbash.jpg
--2023-05-18 01:35:07--  https://artifacts.picoctf.net/c/237/atbash.jpg
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 108.156.172.6, 108.156.172.74, 108.156.172.42, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|108.156.172.6|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 51508 (50K) [application/octet-stream]
Saving to: 'atbash.jpg.3'

atbash.jpg.3        100%[==================>]  50.30K  --.-KB/s    in 0.02s   

2023-05-18 01:35:07 (2.00 MB/s) - 'atbash.jpg.3' saved [51508/51508]

apaleliz-picoctf@webshell:~$ file atbash.jpg 
atbash.jpg: JPEG image data, JFIF standard 1.01, aspect ratio, density 1x1, segment length 16, baseline, precision 8, 465x455, components 3
apaleliz-picoctf@webshell:~$ steghide extract -sf atbash.jpg
Enter passphrase: 
the file "encrypted.txt" does already exist. overwrite ? (y/n) y
wrote extracted data to "encrypted.txt".
apaleliz-picoctf@webshell:~$ 
apaleliz-picoctf@webshell:~$ cat encrypted.txt 
krxlXGU{zgyzhs_xizxp_05y2z65z}

Nos ayudamos con cyberchef para terminar de desencryptar usando
-Atbash Cipher
```


## Bandera
picoCTF{atbash_crack_05b2a65a}