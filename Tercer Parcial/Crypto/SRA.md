## Descripcipción

I just recently learnt about the SRA public key cryptosystem... or wait, was it supposed to be RSA? Hmmm, I should probably check...Connect to the program on our server: `nc saturn.picoctf.net 50052`Download the program: [chal.py](https://artifacts.picoctf.net/c/299/chal.py)

## Pistas

-   (None)

## Solucion

```
apaleliz-picoctf@webshell:~$ nc saturn.picoctf.net 50052
anger = 22215951805784203978788133118384350551046278420170890475201413886822992910914
envy = 49730312626884230056576823397518327804654348750867100504678321583667385400697
vainglory?
> 2116934368449833716546812459265827098747033264721065810557661255683900245023307642794833803777750776348657486697528213628700203417868078769156431779042779145583382563332057098971899163669483908229805892682681550893467091610327264722
> Hubris!
```

## Bandera
picoCTF{7h053_51n5_4r3_n0_m0r3_2b7ad1ae}