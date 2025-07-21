_How to solve picoCTF verify._<br>

run the instance and connect using ssh. <br>
using ls command you can view the files in the current directory, it has checksum.txt, decrypt.sh file and a files directory. Use the cat command to view the checksum value of the checksum.txt file.<br>
useing the grep command we will recursively find the file comtaining the flag which is encrypted. we will pipe out the result of sha256sum for all the files using the grep command.<br>
finaly use the decrypt script to decrypt the flag.<br>

*commands:* <br>
$ls<br>
$cat checksum.txt <br>
$sha256sum ./files/* | grep <_enter the checksum value_><br>
$./decrypt.sh ./files/87590c24<br>

this will return the flag: picoCTF{trust_but_verify_87590c24}<br>
