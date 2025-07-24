## Description
The Rust saga continues? I ask you, can I borrow that, pleeeeeaaaasseeeee? Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/babfbee79718a6363826ba86300173ffde6d81577e9dd07d4130c53a7eecf6c3/fixme2.tar.gz). 

---
`wget` the file and unzip using `gunzip fixme2.tar.gz` and then `tar -xvf fixme2.tar `.<br>

Run the program:
> cargo build.<br>
> cargo run.

After you run it shows a bunch of errors which we need to fix in order to get the flag...
Errors:
> at line 3, fix to mutable. change `borrowed_string: &String` to `borrowed_string: &mut String`. because &String creates an immutable reference. <br>
> at line 35 it needs the same fix. add mut after &. `&mut party_foul`.main() must be declared as mutable with mut to allow changes via a &mut borrow. <br>
> at line 34 also, fix `let party_foul` to `let mut party_foul`.

run again and it returns us the flag...
<img width="810" height="152" alt="image" src="https://github.com/user-attachments/assets/93482f36-d309-463e-a54d-10009736b07f" /><br>

---
Flag: `picoCTF{4r3_y0u_h4v1n5_fun_y31?}`
