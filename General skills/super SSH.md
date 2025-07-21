Description
Using a Secure Shell (SSH) is going to be pretty important. Can you ssh as ctf-player to 
titan.picoctf.net at port 54501 to get the flag? You'll also need the password 1ad5be0d. 
If asked, accept the fingerprint with yes. If your device doesn't have a shell, you can 
use: https://webshell.picoctf.org If you're not sure what a shell is, 
check out our Primer: https://primer.picoctf.com/#_the_shell

After launching the instance connect using ssh, enter the following command:
```bash
ssh ctf-player@titan.picoctf.net -p 54501
```
<img width="882" height="157" alt="image" src="https://github.com/user-attachments/assets/64ec6860-912e-4d0a-920f-3d72e0baf34e" />

flag: picoCTF{s3cur3_c0nn3ct10n_8306c99d}

