## Description
This service provides you an encrypted flag. 
Can you decrypt it with just N & e? 
Connect to the program with netcat: $ nc verbal-sleep.picoctf.net 58750 
The program's source code can be downloaded [here](https://challenge-files.picoctf.net/c_verbal_sleep/eb8ebbb7306b0b21cc95fcd08fed7a6e3a0dd1323b8a0279c043d26349e911ff/encrypt.py).

---
When you connect to the remote server you recieve a cypher text and the value of public key and N.
I have used an online [tool](https://www.dcode.fr/rsa-cipher) to decode the cypher for this challenge.<br>

<img width="1150" height="505" alt="image" src="https://github.com/user-attachments/assets/83e11249-cb9b-44dd-8a0f-b610a8a1e2dc" /><br>

---
Flag:
```
picoCTF{tw0_1$_pr!m33991588e}
```
