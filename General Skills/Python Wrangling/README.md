#Python Wrangling
Category : General Skills
Points : 10

###1.Description

Python scripts are invoked kind of like programs in the Terminal... Can you run [this Python script](https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/ende.py) using [this password](https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/pw.txt) to get [the flag](https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/flag.txt.en)?

###2.Solution

Open file ende.py in editor, you will find a instruction like this
![image-1](/image-1.PNG). Follow the instruction : 

```bash
python3 ende.py -d flag.txt.en
```
It will ask for password. Then you copy and pass in the password in file 'pw.txt'
```bash
Please enter the password:aa821c16aa821c16aa821c16aa821c16
```
###3.Flag

```bash
picoCTF{4p0110_1n_7h3_h0us3_aa821c16}
```

###4.Resources
You need to install python3 first
[Python3 install guide for Linux](https://docs.python-guide.org/starting/install3/linux/)
