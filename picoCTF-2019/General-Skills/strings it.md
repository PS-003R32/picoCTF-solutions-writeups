Description
Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings) without running it?

the *strings* prints the printable character sequences that are at least 4 characters long
if you 'man strings' you will see options for strings.
just use the grep command to find the flag in format picoCTF.
```bash
strings strings | grep pico
```
flag: picoCTF{5tRIng5_1T_d66c7bb7}
