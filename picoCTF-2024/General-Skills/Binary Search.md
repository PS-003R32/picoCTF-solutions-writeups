# Description
Want to play a game? As you use more of the shell, you might be interested in how they work!
Binary search is a classic algorithm used to quickly find an item in a sorted list.
Can you find the flag? You'll have 1000 possibilities and only 10 guesses. Cyber security
often has a huge amount of data to look through - from logs, vulnerability reports, and forensics.
Practicing the fundamentals manually might help you in the future when you have to write your own
tools! You can download the challenge files here:<br>
    [challenge.zip](https://artifacts.picoctf.net/c_atlas/5/challenge.zip)
Additional details will be available after launching your challenge instance.<br>

View the guessing_game.sh at /home/ctf-player/drop-in using a text editor. you can observe that it generated a random number
between 1 to 1000 and only 10 guesses to get it right. To get it right you have to pridict it by entering numbers using the
concept of binary search.<br>
Enter 500 as the program is generating a number in the range 1-1000. The program then has three outputs after a guess which is, 
<img width="598" height="138" alt="image" src="https://github.com/user-attachments/assets/67afebc7-88ac-4f9a-974e-7149a3d6a712" /><br>

Enter a number half of your previous guess or ++ or --. <br>

flag: picoCTF{g00d_gu355_********}<br>
