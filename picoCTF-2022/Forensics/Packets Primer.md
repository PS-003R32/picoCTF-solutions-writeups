Description
Download the packet capture file and use packet analysis software to find the flag.
    [Download packet capture](https://artifacts.picoctf.net/c/194/network-dump.flag.pcap)

After downloading the challenge file, you will notice its a .pcap (packet capture) file. using wireshark we will analyse the file.
Notice the TCP flag PUSH, ACK in the Info window, there's the flag in the TCP stream in plain sight.
```bash
wireshark network-dump.flag.pcap
```
<img width="1365" height="804" alt="image" src="https://github.com/user-attachments/assets/cd7d5f3a-517b-40e6-8ef5-9cd305dafd28" />

Right click  on the request with the above tcp flags > click of follow > follow tcp stream > select show as ASCII. And theres the flag.

<img width="994" height="885" alt="image" src="https://github.com/user-attachments/assets/40db8e68-d8a4-43ca-bb6a-926fc91496fc" />

flag: picoCTF{p4ck37_5h4rk_ceccaa7f}
