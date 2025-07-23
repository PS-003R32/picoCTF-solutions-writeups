Description
Download this image file and find the flag.
  [Download image file](https://artifacts.picoctf.net/c/100/drawing.flag.svg).

In this medium level challenge theres a `SVG` file if you use the `file` command on drawing.flag.txt and we need to find the flag.
with the `exiftool` we will search for metadata that can lead us to a flag such as a comment. you can see below that it has nothing interesting in the metadata:
```bash
exiftool drawing.flag.svg
```
<img height="280" alt="image" src="https://github.com/user-attachments/assets/3644d242-ae12-48fc-95a7-57bd4904cb18" />

to find any string such as the flag format `picoCTF` we have tools such as the `strings` tool that prints printable characters and other tools such as
`hexedit` which allows to edit file content in hexadecimal format.
In this case both the tools reveal something about the flag if you just eyeball around or play with it.
```bash
hexedit drawing.flag.txt
```
<img height="280" alt="image" src="https://github.com/user-attachments/assets/94f0f3e5-552e-4071-9f48-50fc8f66871d" />

```bash
strings drawing.flag.txt
```
<img  height="280" alt="image" src="https://github.com/user-attachments/assets/5fb5640d-b094-4b60-b895-ed66f8719585" />

To grep the flag we will use some delimiters to filter out our flag.
see the flag appears:
```bash
strings drawing.flag.svg| grep "</tspan"
```
<img width="556" height="159" alt="image" src="https://github.com/user-attachments/assets/04c3b35c-8856-4d79-ab4c-a4d558b8098c" />

now we will truncate the other parts of the string, to filter out our flag. With the cut operation we need to specify feild as you can see below. 
With the feild f2 being the left part of the string from ">" and f1 the right part. Now we see the flag clearly.
```bash
strings drawing.flag.svg| grep "</tspan" | cut -d ">" -f2 | cut -d "<" -f1
```
<img width="707" height="233" alt="image" src="https://github.com/user-attachments/assets/d7be4d4a-b6e1-494b-8ac1-69eb66d65b03" />

Now just truncate the new line char `\n` and spaces in between to get the intact flag.
```bash
strings drawing.flag.svg| grep "</tspan" | cut -d ">" -f2 | cut -d "<" -f1 | tr -d "\n" | tr -d " "
```
Flag: ```picoCTF{3nh4nc3d_aab729dd}```
