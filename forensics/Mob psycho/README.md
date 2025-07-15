wget the file
using the hint you can see we can unzip the apk file from the terminal.
unzip the apk file or extract it manualy in the filesystem.
find for the flag using the find command or use the grep command with -r to recursively find for matches.
cat the file flag, it returns a Hexadecimal string.
finaly use any online tool to change it to ascii.


$wget https://artifacts.picoctf.net/c_titan/140/mobpsycho.apk
$sudo unzip mobpsycho.apk
$find . -name flag.txt
$cat ./res/color/flag.txt (7069636f4354467b6178386d433052553676655f4e5838356c346178386d436c5f35653637656135657d)

use any online tool to convert to ascii: picoCTF{ax8mC0RU6ve_NX85l4ax8mCl_5e67ea5e}
