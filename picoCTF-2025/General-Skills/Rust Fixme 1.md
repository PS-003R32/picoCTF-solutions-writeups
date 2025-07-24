## Description
Have you heard of Rust? Fix the syntax errors in this Rust file to print the flag! 
Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/3f0e13f541928f420d9c8c96b06d4dbf7b2fa18b15adbd457108e8c80a1f5883/fixme1.tar.gz). 

---
`wget` the file and follow the image below to unzip the file.<br>
<img width="1012" height="455" alt="image" src="https://github.com/user-attachments/assets/9d516377-771b-4182-882e-c99612526c18" /><br>

As the challenge says we need to fix some errors in the rust file. Now run the program and we will se if it throws errors and help us identify
the errors.
```bash
cargo build
cargo run
```
These are the errors that are there:
> line 5, `let key=...` the semicolon is missing.
> replace ret with return at line 23.
> at line 25, replace `:?` with `{}`.

And thats it follow the commands above to run the program to get the flag.<br>
<img width="762" height="415" alt="image" src="https://github.com/user-attachments/assets/eef31e77-d0d1-4b46-9194-ed4866af889b" /><br>

---
Flag: `picoCTF{4r3_y0u_4_ru$t4c30n_n0w?}`
