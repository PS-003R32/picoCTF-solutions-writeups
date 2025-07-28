## Description
Morse code is well known. Can you decrypt this? Download the file [here](https://artifacts.picoctf.net/c/79/morse_chal.wav). Wrap your answer with picoCTF{}, 
put underscores in place of pauses, and use all lowercase.

---
since the file that we have downloaded is a audio file, we have to decode it using the morse codes. If you manually try to map it to the morse codes it will take 
a lot of time. Instead we will use an online tool to decode this. You can search for audio morse code decoder online, here I used [this](https://morsecode.world/international/decoder/audio-decoder-adaptive.html) one.<br>
<img width="1278" height="766" alt="image" src="https://github.com/user-attachments/assets/62ab0919-6e61-4b17-93b0-3982fddbe9a9" /><br>

I tried submitting the flag in the pico{} format but it wasnt working, after trials changed the case of the decoded text and it worked. change the case to lower and add _ in between and remove spaces.

---
Flag:
```text
picoCTF{wh47_h47h_90d_w20u9h7}
```
