
## Descripcion
Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/e9dd71b5d11023873b8abe99cdb45551/static)? This [BASH script](https://mercury.picoctf.net/static/e9dd71b5d11023873b8abe99cdb45551/ltdis.sh) might help!

## Pistas
No hay

## Solucion
wget https://mercury.picoctf.net/static/e9dd71b5d11023873b8abe99cdb45551/static
ltdis.sh static
chmod +x ltdis.sh
ltdis.sh static
./ltdis.sh static
cat static.ltdis.string.txt static.ltdis.x86_64.txt

```
picoCTF{d15a5m_t34s3r_ae0b3ef2}
```

## Bandera
picoCTF{d15a5m_t34s3r_ae0b3ef2}
## Notas adicionales



## Referencias


