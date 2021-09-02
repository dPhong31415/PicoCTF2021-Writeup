# Mind your P's and Q's

Category : Cryptography

Points : 20

### 1.Description
[]()
### 2.Solution

Write a python script to decrypt with given n,e,c
```python
#!/usr/bin/env python
from Crypto.Util.number import inverse, long_to_bytes
c= 62324783949134119159408816513334912534343517300880137691662780895409992760262021
n= 1280678415822214057864524798453297819181910621573945477544758171055968245116423923
e= 65537


p = 1899107986527483535344517113948531328331
q = 674357869540600933870145899564746495319033

phi = (p -1 ) * (q - 1)
d = inverse(e,phi)

m = pow(c,d,n)
print(long_to_bytes(m))
```
### 3.Flag

```bash
picoCTF{sma11_N_n0_g0od_05012767}
```
### 4.Resources
[picoCTF cryptography guide](https://picoctf.org/learning_guides/Book-2-Cryptography.pdf)
[Basic cryptography](https://youtube.com/playlist?list=PL1ZN4kabqbof_aDUyIcD6tQntun8LLIgL)
[Very easy to understand Modular Arithmetic explain](https://www.youtube.com/watch?v=-zEcHLdABfo)
[RSA Encryption Algorithm](https://www.youtube.com/watch?v=wXB-V_Keiu8)
[RSA decryption with python](https://www.youtube.com/watch?v=Ovi33rfaLLk&t=135s)