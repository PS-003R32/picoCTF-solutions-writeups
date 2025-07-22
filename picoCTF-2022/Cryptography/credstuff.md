## Description
We found a leak of a blackmarket website's login credentials. 
Can you find the password of the user `cultiris` and successfully decrypt it? 
Download the leak [here](https://artifacts.picoctf.net/c/151/leak.tar). 
The first user in `usernames.txt` corresponds to the first password in `passwords.txt`. 
The second user corresponds to the second password, and so on.

In this medium level cryptography challenge, you will see after maping the password for user cultiris the password looks like a flag format `cvpbPGS{P7e1S_54I35_71Z3}`.
It looks like a substitution cypher. use any online tool to bruteforce it.
wget the file using,
```bash
wget https://artifacts.picoctf.net/c/151/leak.tar
```
Extract it using
```bash
tar xvf leak.tar
```
<img width="428" height="339" alt="image" src="https://github.com/user-attachments/assets/bb0ccc58-8284-4ce0-b6cc-dcdec12dc48b" />
<img width="998" height="673" alt="image" src="https://github.com/user-attachments/assets/1313c92b-1d29-492e-b183-ee47489f0487" />

Flag: picoCTF{C7r1F_54V35_71M3}
