### Bandit Level 14 → Level 15

## Objetivo
The password for the next level can be retrieved by submitting the password of the current level to **port 30000 on localhost**.

## Datos de acceso al nivel
bandit14 
fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq

## Solución
```
bandit14@bandit:~$ 
bandit14@bandit:~$ nc localhost 30000 fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq 
Correct!
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt 

^C 
bandit14@bandit:~$
```

## Notas adicionales

| comando | descripción |
|-----|-----|
| IP address | es una dirección única que identifica a un dispositivo en Internet o en una red loca |
## Referencias
[Over The Wire: Bandit Write Up](https://jwuk.files.wordpress.com/2016/05/writeup1.pdf)
[OTW](https://axcheron.github.io/writeups/otw/bandit/)
