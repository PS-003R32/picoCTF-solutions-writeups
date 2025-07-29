## Description
Lyrics jump from verses to the refrain kind of like a subroutine call. There's a hidden refrain this program doesn't print by default. 
Can you get it to print it? There might be something in it for you. 
The program's source code can be downloaded [here](https://challenge-files.picoctf.net/c_verbal_sleep/064d0eba10978d362ad2517e0e6c7d68185078e0b2fca217f8bce134d3180cfc/lyric-reader.py). Connect to the program with netcat: 
$ nc verbal-sleep.picoctf.net 51134

---
Download the file and view the code carefully you will notice the re module matches the string RETURN with numbers.<br>
<img width="559" height="192" alt="image" src="https://github.com/user-attachments/assets/0786a114-9e69-4d0b-b050-cc0395752bab" /><br>

Now we just need to print the first paragraph containing our flag. Notice in the for loop it splits the paragraph with a `;`. You can only obfuscate the program by providing
an input and return the paragraph number indexed 0. Input : `text;RETURN 0` this will print the flag.

<img width="610" height="522" alt="image" src="https://github.com/user-attachments/assets/3ee68f73-6e2d-421a-b72d-94ad74264053" />

---
Flag:
```text
picoCTF{70637h3r_f0r3v3r_ac197d12}
```
