## Description
How about some hide and seek heh? Download this [file](https://artifacts.picoctf.net/c/377/trace.pcap) and find the flag.

---
In this challenge we have to analyze the `trace.pcap` file. Download the file and open it using wireshark `wireshark trace.pcap`.
You will notice it has over 1500 packets, which will be hard for us to find the flaf.
We will use the find packet utility in wireshark. press `Ctrl+F` to open the window.<br>
<img width="746" height="292" alt="image" src="https://github.com/user-attachments/assets/fee74149-4c8b-4f08-8b69-71e8d5cd22af" /><br>
And we have found our flag but its encrypted.<br>
<img width="1465" height="997" alt="image" src="https://github.com/user-attachments/assets/757156a7-5c04-49bd-943d-c3eeab8848e4" /><br>
You can manually type in the flag by right click and `follow TCP stream` or
Right click on the picoCTf string and copy it as a base64 string so that it will be easy for us to decode it using the base64 cli utility.
<img width="791" height="627" alt="image" src="https://github.com/user-attachments/assets/4eea88ff-0e8c-44a6-923d-a1806fe32d6d" />
Now open a terminal window and use the following command to decode the base64 string:
```bash
echo "<past-the-copied-string>" | base64 -d
```
<img width="1057" height="79" alt="image" src="https://github.com/user-attachments/assets/d96dd690-e05f-462d-99be-323c963307be" />

---
Flag:
```text
picoCTF{P64P_4N4L7S1S_SU55355FUL_31010c46}
```
