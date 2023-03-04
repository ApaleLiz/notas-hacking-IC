### Bandit Level 25→ Level 26

## Objetivo
Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not **/bin/bash**, but something else. Find out what it is, how it works and how to break out of it.

## Datos de acceso al nivel
bandit25
p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d

## Solución
```
bandit25@bandit:~$ ls 
bandit26.sshkey bandit25@bandit:~$ ssh -i bandit26.sshkey bandit26@localhost -p 2220

bandit25@bandit:~$ cat /etc/passwd | grep bandit26 bandit26:x:11026:11026:bandit level 26:/home/bandit26:/usr/bin/showtext 
bandit25@bandit:~$ cat /usr/bin/showtext
#!/bin/sh 
export TERM=linux 
exec more ~/text.txt 
exit 0

```
## Notas adicionales

| comando | descripción |
|-----|-----|
| cat | muestra el contenido de un archivo |
| ls | listar archivos |
| ssh | ofrece comunicación encriptada y segura entre dos sistemas sobre una red no segura |

## Referencias
- [Secure Shell (SSH) on Wikipedia](https://en.wikipedia.org/wiki/Secure Shell)
- [How to use SSH on wikiHow](https://www.wikihow.com/Use-SSh)