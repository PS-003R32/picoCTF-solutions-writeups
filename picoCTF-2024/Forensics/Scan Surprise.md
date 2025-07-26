## Description
I've gotten bored of handing out flags as text. Wouldn't it be cool if they were an image instead? You can download the challenge files here:
    [challenge.zip](https://artifacts.picoctf.net/c_atlas/13/challenge.zip).
The same files are accessible via SSH here: ssh -p 49415 ctf-player@atlas.picoctf.net Using the password f3b61b38. Accept the fingerprint with yes, 
and ls once connected to begin. Remember, in a shell, passwords are hidden!

---
wget and unzip the file and then go to `cd home/ctf-player/drop-in` you will notice theres a png file. Open the image `eog flag.png`.
Theres just a qr code, you might try to scan it from your phone, don't because you dont know what happens( if you use strings you will get nothing useful). 
Use any online tool to scan the qr. thsts it you have the flag.

<img width="787" height="552" alt="image" src="https://github.com/user-attachments/assets/683d62b8-ae29-4c13-b485-8de6b790d8ff" />

---
Flag:
```text
picoCTF{p33k_@_b00_d4ca652e}
```
