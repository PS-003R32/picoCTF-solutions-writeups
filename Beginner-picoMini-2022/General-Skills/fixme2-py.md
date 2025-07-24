## Description
Fix the syntax error in the Python script to print the flag. 
[Download Python script](https://artifacts.picoctf.net/c/6/fixme2.py).

---
`wget` the file and run it. You will se it raises an error for if statement. <br>
<img width="750" height="92" alt="image" src="https://github.com/user-attachments/assets/9227e42f-20ce-41b6-ba26-43d52b2d958c" /><br>

Open the script in a text editor, you will notice instead of equality operator<br>
it has an assignment operator. So just replace `=` with `==`.<br>
<img width="552" height="201" alt="image" src="https://github.com/user-attachments/assets/8b094650-4174-435c-9c35-8989b1b9526e" /><br>

---
Now run the program again, it prints the flag.<br>
Flag:picoCTF{3qu4l1ty_n0t_4551gnm3nt_f6a5aefc}
