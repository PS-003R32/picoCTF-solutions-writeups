Description
A new modular challenge! Download the message [here](https://artifacts.picoctf.net/c/178/message.txt). Take each number mod 41 and find the modular inverse for the result. 
Then map to the following character set: `1-26` are the `alphabet`, `27-36` are the `decimal digits`, and `37` is an `underscore`. 
Wrap your decrypted message in the picoCTF flag format (i.e. picoCTF{decrypted_message})

The script from the basic-mod1 challenge will be helpful in this challenge. We will modify the script for this challenge.
The inverse mod of a number x with y can be found using the pow function in python, which is `pow(num,-1,41)` for this challenge.
For this challenge.
```python
#! /usr/bin/env python3
from string import ascii_uppercase, digits
import math
flag=[]
with open("message.txt") as cat:
        numbers=cat.read()
        list=[int(val) for val in numbers.split()]
        for i in list:
                modinv=pow(i,-1,41)
                if modinv in range(1,27):
                        flag.append(ascii_uppercase[modinv-1])
                elif modinv in range(27,37):
                        flag.append(digits[modinv-27])
                else:
                        flag.append('_')
print("picoCTF{"+"".join(flag)+"}")
```
Flag: picoCTF{1NV3R53LY_H4RD_C680BDC1}
