# Nice netcat...
Category : General Skills

Points : 15

### 1.Description
There is a nice program that you can talk to by using this command in a shell: 
```
$ nc mercury.picoctf.net 43239
```
but it doesn't speak English...

### 2.Solution

Run the command in description you will receive a list of number. These are decimal representations of ascii characters (you can detect it by looking at the number, it will be between 65 - 126 for latin alphabet). So you need to convert from decimal to string using :

```bash
for n in $(echo | nc mercury.picoctf.net 43239); do
	printf "\\$(printf %03o "$n")";
done
```
### 3.Flag

```bash
picoCTF{g00d_k1tty!_n1c3_k1tty!_7c0821f5}
```
###4.Resources
