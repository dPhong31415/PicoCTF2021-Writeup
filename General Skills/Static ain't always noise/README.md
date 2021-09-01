#Static ain't always noise

Category : General Skills

Points : 20

### 1.Description

Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/bc72945175d643626d6ea9a689672dbd/static?) This [BASH script](https://mercury.picoctf.net/static/bc72945175d643626d6ea9a689672dbd/ltdis.sh) might help!

### 2.Solution

Change permission of ltdis.sh to executable

```bash
chmod +x ltdis.sh
```
Pass 'static' file as first argument and run the BASH script

```bash
./ltdis.sh static
```
Read the output file

```bash
cat static.ltdis.strings.txt
```
### 3.Flag

```bash
picoCTF{d15a5m_t34s3r_1e6a7731}
```
### 4.Resources

[Understand arguments in C programming](https://www.youtube.com/watch?v=JGoUaCmMNpE&list=PLhixgUqwRTjxglIswKp9mpkfPNfHkzyeN&index=3)
