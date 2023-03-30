## Descripcion
There is some interesting information hidden around this site [http://mercury.picoctf.net:55079/](http://mercury.picoctf.net:55079/). Can you find it?

## Pistas
-You should have enough hints to find the files, don't run a brute forcer

## Solucion
-Ir a la página que da el reto
-La primera parte la da en el codifo fuente en la parte de abajo
-La segunda parte en [mycss.css](view-source:http://mercury.picoctf.net:55079/mycss.css)
-y las siguientes partes entramos a las páginas sig:
-view-source:http://mercury.picoctf.net:55079/robots.txt
User-agent: *
Disallow: /index.html
 Part 3: t_0f_pl4c
 I think this is an apache server... can you Access the next flag?

-view-source:http://mercury.picoctf.net:55079/.htaccess
 Part 4: 3s_2_lO0k
 I love making websites on my Mac, I can Store a lot of information there.

-view-source:http://mercury.picoctf.net:55079/.DS_Store
Congrats! You completed the scavenger hunt. Part 5: _74cceb07}

```
`picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_74cceb07}`
```

## Bandera
picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_74cceb07}


