# information
Category : Forensics

Points : 10

### 1.Description
Files can always be changed in a secret way. Can you find the flag? [cat.jpg](https://mercury.picoctf.net/static/b4d62f6e431dc8e563309ea8c33a06b3/cat.jpg)
### 2.Solution
First you need a program to read metadata of images
Download ExifTool [here](https://www.geeksforgeeks.org/installing-and-using-exiftool-on-linux/)
Read 'cat.jpg' with exiftool
```bash
exiftool cat.jpg
```
You will see a bit of encoded text wrap in between two "PicoCTF" like this :
![image-2](/Images/image-2.PNG)

That's a text encoded with Base64. So you can use 'base64' command to decode it (or use online decode tool)
```bash
echo cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9 | base64 -d
```
### 3.Flag
```bash
picoCTF{the_m3tadata_1s_modified}
```
### 4.Resources
Some useful resources to learn about Base64 algorithm

[Base64 Decode Algorithm](https://base64.guru/learn/base64-algorithm/decode)

[Base64 Algorithm](https://fm4dd.com/programming/base64/base64_algorithm.shtm)
