### Bandit Level 18 → Level 19

## Objetivo
The password for the next level is stored in a file **readme** in the homedirectory. Unfortunately, someone has modified **.bashrc** to log you out when you log in with SSH.


## Datos de acceso al nivel
bandit18
hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg

## Solución
```
ssh bandit18@bandit.labs.overthewire.org -p 2220 ...
...
Byebye ! 
Connection to bandit.labs.overthewire.org closed. >> Forma 1
ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme 

 This is an OverTheWire game server.
  More information on http://www.overthewire.org/wargames 
  bandit18@bandit.labs.overthewire.org's password: awhqfNnAbc1naukrpqDYcF95h7HoMTrC
```
## Notas adicionales
| comando | descripción |
|-----|-----|
| cat | muestra el contenido de un archivo |
| ls | listar archivos |

## Referencias
- [Secure Shell (SSH) on Wikipedia](https://en.wikipedia.org/wiki/Secure Shell)
- [How to use SSH on wikiHow](https://www.wikihow.com/Use-SSh)