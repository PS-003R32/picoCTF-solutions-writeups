Description
Python scripts are invoked kind of like programs in the Terminal... 
Can you run this [Python script](https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/ende.py) using this [password](https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/pw.txt) to get the [flag](https://mercury.picoctf.net/static/b351a89e0bc6745b00716849105f87c6/flag.txt.en)?

if you open the ende.py in a text editor you will see it uses base64 and fernet modules for encr and decr.
cat the pw.text file and copy the password.
```bash
cat pw.txt
```
<img width="375" height="47" alt="image" src="https://github.com/user-attachments/assets/0f0b7659-177a-4741-94d3-7b31f78bed51" />

```bash
python3 ende.py -d flag.txt.en
```
<img width="495" height="77" alt="image" src="https://github.com/user-attachments/assets/2e07519a-6c01-46d1-ba50-7d85da2ac57b" />

flag: picoCTF{4p0110_1n_7h3_h0us3_67c6cc96}
