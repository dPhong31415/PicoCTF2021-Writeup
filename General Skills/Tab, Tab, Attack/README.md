#Tab, Tab, Attack
Category : General Skills
Points : 20

###1.Description
Using tabcomplete in the Terminal will add years to your life, esp. when dealing with long rambling directory structures and filenames: [Addadshashanammu.zip](https://mercury.picoctf.net/static/659efd595171e4c40378be6a2e9b7298/Addadshashanammu.zip)
###2.Solution
Download the zip file and unzip it using :
```bash
unzip Addadshashanammu.zip
```
Then type cd and Tab until the auto-complete stop:
```bash
cd /Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku
```
Then run the file inside the last bin :
```bash
./fang-of-haynekhtnamet
```
###3.Flag
```bash
picoCTF{l3v3l_up!_t4k3_4_r35t!_524e3dc4}

```
###4.Resources
[Install TAB auto-completion on Linux](https://faun.pub/configure-bash-auto-completion-tab-completion-on-linux-db0d9310818b)