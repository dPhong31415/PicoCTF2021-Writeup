#Transformation
Category : Reverse Engineering
Points : 20

###1.Description
I wonder what this really is... [enc](https://mercury.picoctf.net/static/2b4cea9b07db22bf4f933fddd1b8caa9/enc) 
```
''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])
```
###2.Solution
First, let's read what in the file using :
```bash
cat enc
```
You will see a bunch of Chinese characters mix with Korean mix with Japanese. So that's UTF-16 encoded text.Decode it using : (or you can use online decode tool like ASCIItohex)
```bash
iconv -f UTF-8 -t UTF-16BE <enc 
```
###3.Flag
```bash
picoCTF{16_bits_inst34d_of_8_04c0760d}
```
###4.Resources
[What is UNICODE ?](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)
[Why do we need UNICODE](https://stackoverflow.com/questions/2241348/what-is-unicode-utf-8-utf-16)
[Use iconv to convert UTF-8 to UTF-16](https://unix.stackexchange.com/questions/17240/chinese-characters-instead-of-latin-being-written-to-file)