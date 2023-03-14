
## Descripcion
Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 14291`.

## Pistas
Remember the flag format is picoCTF{XXXX}
What's a pipe? No not that kind of pipe... This [kind](http://www.linfo.org/pipes.html)

## Solucion
apaleliz-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 14291
apaleliz-picoctf@webshell:~$ ls
README.txt  flagout.txt  picobrowser  strings
apaleliz-picoctf@webshell:~$ cat flagout.txt | grep pico
picoCTF{digital_plumb3r_ea8bfec7}
```
picoCTF{digital_plumb3r_ea8bfec7}
```

## Bandera
picoCTF{digital_plumb3r_ea8bfec7}

## Notas adicionales



## Referencias
