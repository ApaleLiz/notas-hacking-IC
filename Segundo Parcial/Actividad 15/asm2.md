## Descripcipción

What does asm2(0x4,0x2d) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/ceac75672637589213b952abe32c84b3/test.S)

## Pistas

-   assembly [conditions](https://www.tutorialspoint.com/assembly_programming/assembly_conditions.htm)

## Solucion
```
[      ] < ebp-0x10 < esp
[      ] < ebp-0xc
[ 0x78 ] < ebp-0x8
[ 0x22 ] < ebp-0x4 
[ ebp  ] < ebp 
[ ret  ] < ebp+0x4
[ 0x4  ] < ebp+0x8
[ 0x21 ] < ebp+0xc

registers
[     ]eax
asm2:(0x4,0x21)
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
>>> 0x4 <= 0xfb46
True
>>> hex(0x21 + 0x1)
'0x22'
>>> hex(0x4+0x74)
'0x78'
>>> 0x78 <= 0xfb46
True
>>> 0xfb46 / 0x74
554.5344827586207
>>> int(0x21)
33
>>> hex(555+33)
'0x24c'
>>> 
```
## Bandera
0x24c