## Description
Have you heard of Rust? Fix the syntax errors in this Rust file to print the flag! Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/dcdaf491b35c1d0f5075e9583edbbb7aaea1dffb6ad32bc000e4d87b5200ff7b/fixme3.tar.gz).

---
`wget` the file and unzip using `gunzip fixme3.tar.gz` and then `tar -xvf fixme3.tar `.<br>

Run the program:
> cargo build.<br>
> cargo run.

After you run it shows a bunch of errors which we need to fix in order to get the flag...
Errors:
> line 3 mutable string within the decrypt function.`fn decrypt(encrypted_buffer: Vec<u8>, borrowed_string: &mut String)`<br>
> line 42 declare mut for party_foul. `let mut party_foul = String::from("Using memory unsafe languages is a: ");`<br>
> again at line 43, change the function call parameter. `decrypt(encrypted_buffer, &mut party_foul);`.<br>
> ine 22 change, `borrowed_string.push_str(&String::from_utf8_lossy(&decrypted_buffer));` <br>

After these fixes, run the program again.
<img width="836" height="268" alt="image" src="https://github.com/user-attachments/assets/76f855e9-845d-41af-b3c5-94eec9b579da" />

---
Flag: `picoCTF{n0w_y0uv3_f1x3d_1h3m_411}`
