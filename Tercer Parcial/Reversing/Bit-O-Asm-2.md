## Descripcipción

Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Download the assembly dump [here](https://artifacts.picoctf.net/c/510/disassembler-dump0_b.txt).

## Pistas

- `PTR`'s or 'pointers', reference a location in memory where values can be stored.

## Solucion

```
apaleliz-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/510/disassembler-dump0_b.txt
--2023-05-22 00:36:18--  https://artifacts.picoctf.net/c/510/disassembler-dump0_b.txt
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 108.156.172.120, 108.156.172.74, 108.156.172.6, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|108.156.172.120|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 270 [application/octet-stream]
Saving to: 'disassembler-dump0_b.txt'

disassembler-dump0_ 100%[==================>]     270  --.-KB/s    in 0s      

2023-05-22 00:36:18 (96.1 MB/s) - 'disassembler-dump0_b.txt' saved [270/270]

apaleliz-picoctf@webshell:~$ cat disassembler-dump0_b.txt
<+0>:     endbr64 
<+4>:     push   rbp
<+5>:     mov    rbp,rsp
<+8>:     mov    DWORD PTR [rbp-0x14],edi
<+11>:    mov    QWORD PTR [rbp-0x20],rsi
<+15>:    mov    DWORD PTR [rbp-0x4],0x9fe1a
<+22>:    mov    eax,DWORD PTR [rbp-0x4]
<+25>:    pop    rbp
<+26>:    ret
```

## Bandera
picoCTF{654874}