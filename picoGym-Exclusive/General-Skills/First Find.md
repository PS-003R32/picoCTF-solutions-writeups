Description<br>
Unzip this archive and find the file named 'uber-secret.txt'<br>
    [Download zip file](https://artifacts.picoctf.net/c/500/files.zip)

  In this challenge you will see there are many directories and some hidden directories as well.<br>
  Simply using the grep command will not help you to find the flag, although its hidden in plain text.<br>
  to solve this challenge we will recursively find the string 'picoCTF' in the files directory after unzipping files.zip.<br>

  commands:<br>
  ```bash
  wget https://artifacts.picoctf.net/c/500/files.zip<br>
  ```
  ```bash
  unzip files.zip<br>
  ```
  ```bash
  grep -r picoCTF<br>
  ```
  <img width="993" height="52" alt="image" src="https://github.com/user-attachments/assets/19585345-a6ac-456f-a230-3e5b466a4e21" /><br>

flag: picoCTF{f1nd_15_f457_ab443fd1}
