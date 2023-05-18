## Descripcipción

What does asm3(0xd73346ed,0xd48672ae,0xd3c8b139) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/17c5620fcffa388fe518d31cb4dd99a0/test.S)

## Pistas

-  more(?) [registers](https://wiki.skullsecurity.org/index.php?title=Registers)

## Solucion
```
asm3:
	<+0>:   push   ebp
        <+1>:   mov    ebp,esp
        <+3>:   cmp    DWORD PTR [ebp+0x8],0x3fb
        <+10>:  jg     0x512 <asm1+37>
        <+12>:  cmp    DWORD PTR [ebp+0x8],0x280
        <+19>:  jne    0x50a <asm1+29>
        <+21>:  mov    eax,DWORD PTR [ebp+0x8]
        <+24>:  add    eax,0xa
        <+27>:  jmp    0x529 <asm1+60>
        <+29>:  mov    eax,DWORD PTR [ebp+0x8]
        <+32>:  sub    eax,0xa
        <+35>:  jmp    0x529 <asm1+60>
        <+37>:  cmp    DWORD PTR [ebp+0x8],0x559
        <+44>:  jne    0x523 <asm1+54>
        <+46>:  mov    eax,DWORD PTR [ebp+0x8]
        <+49>:  sub    eax,0xa
        <+52>:  jmp    0x529 <asm1+60>
        <+54>:  mov    eax,DWORD PTR [ebp+0x8]
        <+57>:  add    eax,0xa
        <+60>:  pop    ebp
        <+61>:  ret      

----------------------------------------------------------------------------
USANDO EMULADOR
start:
push 0xe54409d5
push 0xe6cf51f0
push 0xd2c26416
call asm3

asm3:
		push   ebp
		mov    ebp,esp
		xor    eax,eax
		mov    ah,BYTE PTR [ebp+0x9]
		shl    ax,0x10
		sub    al,BYTE PTR [ebp+0xe]
		add    ah,BYTE PTR [ebp+0xf]
		xor    ax,WORD PTR [ebp+0x12]
		nop
		pop    ebp
		ret    
```
## Bandera
0x375