# Description
Can you make sense of this file? Download the file [here](https://artifacts.picoctf.net/c/471/enc_flag)

In this easy level challenge when you cat the file you will see a base64 encoded ascii. We will use the commandline tool 
to decode the string.
# Command
```bash
echo "<the_encoded_text>" | base64 -d
```
-d is for decode. do this till you get the flag. replace the string every time you get the output
from the previous step.(Its around 6 times till you get the flag).
