## Description
Attackers have hidden information in a very large mass of data in the past, maybe they are still doing it. 
Download the data [here](https://artifacts.picoctf.net/c/126/anthem.flag.txt).

---
`wget` the file and if you cat out the anthem.flag.txt it has so many lines of strings. To find the flag we will try to find the flag
using the grep command. `grep -r -e 'pico'` this will recursively find the string pico inside the current directory.<br>

<img width="683" height="51" alt="image" src="https://github.com/user-attachments/assets/b40ab520-a931-4230-a00d-48c3e0309327" /><br>

---
Flag:
```text
picoCTF{gr3p_15_@w3s0m3_2116b979}
```
