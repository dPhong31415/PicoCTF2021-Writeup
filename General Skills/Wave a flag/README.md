# Wave a flag

Category : General skills

Points : 10

### 1.Description

Can you invoke help flags for a tool or binary? [This program](https://mercury.picoctf.net/static/a14be2648c73e3cda5fc8490a2f476af/warm) has extraordinarily helpful information...

### 2.Solution

Just run the program with './' command

```bash
$ ./warm
Hello user! Pass me a -h to learn what I can do!
```
Then pass it a -h

```bash
./warm -h
```
### 3.Flag

```bash
picoCTF{b1scu1ts_4nd_gr4vy_755f3544}
```
