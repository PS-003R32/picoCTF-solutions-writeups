## Description
Can you find the flag in this disk image? 
Download the disk image [here](https://artifacts.picoctf.net/c/536/disko-1.dd.gz). 

---
`wget` the file and use the `file disko-1.dd` command to view details, its a gzip file. Use `gunzip disko-1.dd.gz` to unzip the file.
Perform to extract the meta data of the file to find any hints or comments for the flag. The `exiftool disko-1.dd` returns no data.
But we can find printable strings in the file using `strings filename` and also you can use `hexedit` to find any hints.

here i will use strings, `strings disko-1.dd | grep pico`. And theres the flag:
<img width="613" height="218" alt="image" src="https://github.com/user-attachments/assets/323847c8-c14e-483b-bc51-25fbaa563bd1" />

---
Flag:
```
picoCTF{1t5_ju5t_4_5tr1n9_c63b02ef}
```
