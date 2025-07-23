## Description
A program has been provided to you, what happens if you try to run it on the command line? 
Download the program [here](https://artifacts.picoctf.net/c/218/run).

If you use the `file` command you will see its a ELF file but the permissions is not set to execute. We will change the permissions
by using `chmod +x run` to make it executable and see what the program does. Run the program, `./run` and theres the flag.

<img width="720" height="195" alt="image" src="https://github.com/user-attachments/assets/f2daa392-4fd3-4cad-aed4-3f6b3550a8c7" />

Flag: picoCTF{U51N6_Y0Ur_F1r57_F113_9bc52b6b}
