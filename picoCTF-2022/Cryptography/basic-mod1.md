### Description
We found this weird message being passed around on the servers, we think we have a working decryption scheme. 
Download the message [here](https://artifacts.picoctf.net/c/128/message.txt). Take each number mod 37 and map it to the following character set: `0-25` is the 
`alphabet (uppercase)`, `26-35` are the `decimal digits`, and `36` is an `underscore`. Wrap your decrypted message in the 
picoCTF flag format (i.e. picoCTF{decrypted_message})

So in the description it says we have to map the alphabets and numbers to the num range we get after % 37. We will use the `string` module 
to map instead of creating `A,B,C,...,Z` and map it. I have attached script below:

```python
#! /usr/bin/env python3
from string import ascii_uppercase, digits
flag=[]
with open("message.txt") as cat:
        numbers=cat.read()
        list=[int(val) for val in numbers.split()]
        for i in list:
                mod=i % 37
                if mod in range(26):
                        flag.append(ascii_uppercase[mod])
                elif mod in range(26,36):
                        flag.append(digits[mod-26])
                else:
                        flag.append('_')
print("picoCTF{"+"".join(flag)+"}")
```
Here we will first read the contents of the flag file and store the encrypted numbers in a list. then each number will be moded with 37
to get the remainder. the remainder will be mapped with the above conditional statements.
<img width="740" height="497" alt="image" src="https://github.com/user-attachments/assets/d3485e8c-0705-4f49-88f2-7ddb1ad81350" />

Flag: ```picoCTF{R0UND_N_R0UND_B6B25531}```
