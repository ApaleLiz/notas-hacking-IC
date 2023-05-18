## Descripcipción

I have these 2 images, can you make a flag out of them? [scrambled1.png](https://mercury.picoctf.net/static/75e646e4ad19967ca1811f895fb40465/scrambled1.png) [scrambled2.png](https://mercury.picoctf.net/static/75e646e4ad19967ca1811f895fb40465/scrambled2.png)

## Pistas

-  [https://en.wikipedia.org/wiki/Visual_cryptography](https://en.wikipedia.org/wiki/Visual_cryptography)
- Think of different ways you can "stack" images

## Solucion
```
Usando python
from PIL import Image
import numpy as np
imagen1 = np.asarray(Image.open('scrambled1.png'))
imagen2 = np.asarray(Image.open('scrambled2.png'))

print(imagen1)
print(imagen2)

datos = imagen1.copy() + imagen1.copy()
nueva = Image.fromarray(datos
nueva.save('nueva.png','PNG')
```
## Bandera
picoCTF{1b867c3e}