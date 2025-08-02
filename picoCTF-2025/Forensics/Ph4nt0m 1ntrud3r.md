## Description
A digital ghost has breached my defenses, and my sensitive data has been stolen! 
😱💻 Your mission is to uncover how this phantom intruder infiltrated my system and retrieve the hidden flag. 
To solve this challenge, you'll need to analyze the provided PCAP file and track down the attack method. 
The attacker has cleverly concealed his moves in well timely manner. Dive into the network traffic, 
apply the right filters and show off your forensic prowess and unmask the digital intruder! 
Find the PCAP file here [Network Traffic PCAP](https://challenge-files.picoctf.net/c_verbal_sleep/a917f567b9cc0f1a730a7801b309955df4d2234a8114326857b9759e9e5d0453/myNetworkTraffic.pcap) file and try to get the flag.

---
The pcap file has 22 packets that we need to analyze. From the hints you will get that the attacks were done in a timely manner.
In each packet you will se a base64 encoded string. `0.000000` is the starting point and `+0.000xxx` means the event occured delayed the expected time and `-0.00xxxx` means event
occured before expected time. Now if you see the length, we have a len of 4 which is unique. now folloe the TCP stream and copy the basecy encoded string,
use the cli to decode the string.<br>
<img width="700" height="238" alt="image" src="https://github.com/user-attachments/assets/2a3818f3-794f-4918-83e7-635558972fc5" /><br>
We get the a portion of the flag here.<br>
Now we have the length 12 , analyse all the len 12 packets and decode using base64 cli.<br>
<img width="562" height="160" alt="image" src="https://github.com/user-attachments/assets/dc91931b-d07c-4c45-b537-fb20dac3d482" /><br>
Do it for the remaining ones.<br>

---
Flag:
```text
picoCTF{1t_w4snt_th4t_34sy_tbh_4r_959f50d3}
```
