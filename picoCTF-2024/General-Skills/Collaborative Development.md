Description<br>
My team has been working very hard on new features for our flag printing program!<br>
I wonder how they'll work together? You can download the challenge files here:<br>

    challenge.zip (https://artifacts.picoctf.net/c_titan/70/challenge.zip)<br>

Download the challenge.zip file and move to drop-in directory after unzipping it.<br>
Using '$git log' you can we get the commit history with the commit ID.<br>
<img width="602" height="115" alt="image" src="https://github.com/user-attachments/assets/5f6fb4e4-8194-4419-8f5d-ecd5eb58a70c" /><br>
Using '$git show' it reveals nothing. We need to use other commands to find the flag. use the 'git+tab button' to view all commands.<br>
<img width="595" height="231" alt="image" src="https://github.com/user-attachments/assets/ca920a2b-5cf9-4d47-8803-6a015332c35d" /><br>

we will use git branch to view the branches available.<br>
<img width="252" height="82" alt="image" src="https://github.com/user-attachments/assets/8706c00c-5ee0-44e7-97d4-3e862c6f3b0b" /><br>

to enter the branch we will use '$ git log feature/part-1 and git show <commit id of add part 1>' we get the first half of the flag.<br>
Similarly do it for the other two branches to get the flag.<br>
<img width="606" height="246" alt="image" src="https://github.com/user-attachments/assets/fa7f6875-6239-42bb-9c45-9926446aa711" /><br>

flag: picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_7ffa0077}
