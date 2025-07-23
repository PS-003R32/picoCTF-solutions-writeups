## Description
A message has come in but it seems to be all scrambled. Luckily it seems to have the key at the beginning. 
Can you crack this substitution cipher? Download the message [here](https://artifacts.picoctf.net/c/153/message.txt).

In this challenge we have a substitution cypher encoded text. After you `wget` the file, and `cat` out the `message.txt` file you
will notice the flag format at the bottom which is encoded.
At the top we have the cypher, we will map it to the plaintext alphabets:
Cipher alphabet: OHNFUMWSVZLXEGCPTAJDYIRKQB
Plain alphabet: ABCDEFGHIJKLMNOPQRSTUVWXYZ
below is a python script that you can make to solve the problem, but also you can use any 
online tool to automatically do it for you. but i will suggest you use the script to better understand the problem...;)

```python
flag = "pvncNDM{5YH5717Y710G_3I0XY710G_03055505}"
cipher = "OHNFUMWSVZLXEGCPTAJDYIRKQB"
plain = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
decoded = ""
for char in flag:
    if char.isalpha():
        index = cipher.find(char.upper())
        plain_char = plain[index] if index != -1 else char
        decoded += plain_char if char.isupper() else plain_char.lower()
    else:
        decoded += char

print(decoded)
```
Below is the online tool method:
<img width="1815" height="712" alt="image" src="https://github.com/user-attachments/assets/8c26e3a1-ab16-4d1c-8ba0-d7296fc3878d" />

Flag: picoCTF{5UB5717U710N_3V0LU710N_03055505}
