# Description
Know of little and big endian? [Source](https://artifacts.picoctf.net/c_titan/116/flag.c)
Launch your live instance: nc titan.picoctf.net 00000<br>

You need to know little and big endian representation.<br>
Example: Suppose you have the 4-byte hexadecimal value 0x12345678.<br>
Big Endian memory representation: 12 34 56 78<br>
Little Endian memory representation: 78 56 34 12<br>

<img width="692" height="120" alt="image" src="https://github.com/user-attachments/assets/713fff8e-415e-4041-b7fa-176350f363d3" /><br>

Use any online tool such as this one,<br>
<img width="495" height="447" alt="image" src="https://github.com/user-attachments/assets/e94f8a1e-8925-42dd-a325-6e1847d96cd2" /><br>

Map the string and provide the input in little and big endian formats as asked. for every correct answer the program will step ahead and reveal the flag.<br>

flag: picoCTF{3ndi4n_sw4p_su33ess_********}
