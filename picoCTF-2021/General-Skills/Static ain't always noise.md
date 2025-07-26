## Description
Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/static)? This [BASH script](https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/ltdis.sh) might help!

---
In this challenge we have two files. one is a shell code and other one is an ELF file. change the user permission to executable.
Do `chmod +x static && chmod +x ltdis.sh`. after that, try to run these scripts one by one to find any hints or leads to retrieve the flag.
when you execute the static file `./static` it returns some text, which is of no use to us. Then run the file `./ltdis.sh`, you will see 
it asks for a file as a parameter... since it reveals nothing about the flag we will simply provide the `static` file as the parameter and see if we get something.

<img width="757" height="92" alt="image" src="https://github.com/user-attachments/assets/bf3a6e01-3273-46db-914d-134c9d532723" /><br>

`./ltdis.sh static` , You will notice the program runs successfully. and also returns two files `static.ltdis.strings.txt` and `static.ltdis.x86_64.txt`.

<img width="557" height="55" alt="image" src="https://github.com/user-attachments/assets/0f7fbc63-1006-4e3e-9a4e-5687e7ca63dd" />

cat out both of them and see if it has the flag, `cat static.ltdis.strings.txt | grep pico` and `cat static.ltdis.x86_64.txt | grep pico`.
you will see static.ltdis.strings.txt returns our flag.

<img width="386" height="50" alt="image" src="https://github.com/user-attachments/assets/c8e71368-76ec-4a43-a0a8-cbf620333799" />

---
Flag:
```text
picoCTF{d15a5m_t34s3r_f5aeda17}
```
