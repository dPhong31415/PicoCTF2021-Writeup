#Mod 26
Category : Cryptography
Points : 10

### 1.Description
Cryptography can be easy, do you know what ROT13 is?
``` 
cvpbPGS{arkg_gvzr_V'yy_gel_2_ebhaqf_bs_ebg13_MAZyqFQj}
```
### 2.Solution

Use 'tr' command to decode ROT13 code by shifting every letter 13 times. Keep number and other character the same.

```bash
echo "cvpbPGS{arkg_gvzr_V'yy_gel_2_ebhaqf_bs_ebg13_MAZyqFQj}" | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```
### 3.Flag
```bash
picoCTF{next_time_I'll_try_2_rounds_of_rot13_ZNMldSDw}
```
### 4.Resources
[ROT13 explain](https://en.wikipedia.org/wiki/ROT13)
['tr' command explain](https://linuxhint.com/bash_tr_command/)
