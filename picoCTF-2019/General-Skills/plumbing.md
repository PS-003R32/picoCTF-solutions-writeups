# Description
Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from <br>
this program and search for the flag? Connect to jupiter.challenges.picoctf.org 14291.<br>

use the netcat command to connect.<br>
'$ nc jupiter.challenges.picoctf.org 14291'<br>
<img width="666" height="541" alt="image" src="https://github.com/user-attachments/assets/898df2ac-b473-42ac-aa95-d939de29c343" /><br>

you will se it outputs thousands of lines of string and its very difficult to eyeball the flag. So, we will use <br>
the grep command to pipe the output and find the flag.<br>

<img width="511" height="57" alt="image" src="https://github.com/user-attachments/assets/a893edc6-831c-4825-994e-c175fbe632a7" />

flag: picoCTF{digital_plumb3r_ea8bfec7}
