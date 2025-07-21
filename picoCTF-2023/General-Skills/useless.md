Description
There's an interesting script in the user's home directory The work computer is running SSH. 
We've been given a script which performs some basic calculations, explore the script and find a flag.

Hostname: saturn.picoctf.net
Port:     55953
Username: picoplayer
Password: password

connect using ssh:
```bash
ssh picoplayer@saturn.picoctf.net -p 55953
```
you will see a script which after you cat, does some mathematical calculations but doesnt reveal the flag.
In the else statement it says to read the manual. which will reveal the flag.
```bash
cat useless
```
```bash
man useless
```
<img width="549" height="675" alt="image" src="https://github.com/user-attachments/assets/9fa7b42d-90ef-4713-b0e3-8ae9ddf60360" />

<img width="962" height="460" alt="image" src="https://github.com/user-attachments/assets/274b9c38-1271-4f43-9af3-4b8a1e194d7a" />

flag: picoCTF{us3l3ss_ch4ll3ng3_3xpl0it3d_4151}
