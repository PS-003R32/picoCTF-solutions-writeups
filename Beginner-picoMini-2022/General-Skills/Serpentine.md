Description<br>
Find the flag in the Python script! <br>
[Download Python script](https://artifacts.picoctf.net/c/35/serpentine.py)

If you run the python script you will notice it has option 'b' to print the flag but it doesn't.<br>
to dig deeper we will use a text editor to view the script. you will notice at line 17 it has some encrypted flag and also a print flag function<br>
to print the encrypted flag, which is just hex.<br>
<img width="916" height="108" alt="image" src="https://github.com/user-attachments/assets/e9afd74a-684f-4360-813c-caffe1b9fdde" /><br>
 Scroll below you will see tht in the conditional statement it is not set to print the encrypted flag:<br>
 <img width="837" height="167" alt="image" src="https://github.com/user-attachments/assets/64c97505-e6c4-44f1-b496-4d31fdf4930e" /><br>

edit the line to call print flag function to print the flag:<br>
<img width="896" height="243" alt="image" src="https://github.com/user-attachments/assets/243cf901-47ec-480b-80d6-92d27df78319" /><br>


 Flag: picoCTF{7h3_r04d_l355_7r4v3l3d_ae0b80bd}
