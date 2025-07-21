Description
I accidentally wrote the flag down. Good thing I deleted it! You download the challenge files here:
    [challenge.zip](https://artifacts.picoctf.net/c_titan/77/challenge.zip)

In this easy level challenge we have to perform some git commands.
Download the challenge.zip file and unzip the file.
Move to drop-in directory and you have a txt file which when cat ourt shows 'TOP SECRET'.
we will use git commands to solve this challenge. use '$git + TAB' to view all options for git.

How to solve:
```bash
wget https://artifacts.picoctf.net/c_titan/77/challenge.zip
```
```bash
unzip challenge.zip && cd drop-in
```
```bash
git + tab (to view options)
```
```bash
git log
```
```bash
git show <commit ID of 'remove sensitive info'> (this will reveal the flag)
```
flag:picoCTF{s@n1t1z3_30e86d36}
