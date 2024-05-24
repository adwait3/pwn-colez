![image](https://github.com/adwait3/pwn-colez/assets/148553626/c4247e3e-0abc-4980-a2c2-d46556f40eb2)_________________________________________________________________
# level 1.0
opened the program in ghidra and found a variable named expected result so opeened it and foun the value to be 
```
onkap

```
![Screenshot 2024-05-21 122901](https://github.com/adwait3/pwn-colez/assets/148553626/556c7cad-9f03-4fea-a598-dd1a2016c1b4)

used this value to get the flag 

![Screenshot 2024-05-21 122845](https://github.com/adwait3/pwn-colez/assets/148553626/3a75e7bf-0322-4b70-a1dc-55966fce0562)

flag : "pwn.college{oZA8Hsn4ZSQuW7gZja89n-_fJO0.0VM1IDL0QTMyUzW}"


_____________________________________________________________________________________________

# level 1.1
found the key in a function though ghidra

![Screenshot 2024-05-21 140048](https://github.com/adwait3/pwn-colez/assets/148553626/77836039-740a-4daf-bf45-baa7e519b680)

"dxglh"

using this we get the flag 

![Screenshot 2024-05-21 142604](https://github.com/adwait3/pwn-colez/assets/148553626/ea849d8f-ccdc-4966-9b49-8da3b3e6b47e)

flag: "pwn.college{svdTwK4idyY8wYnzcWwl_VOsLZ9.0lM1IDL0QTMyUzW}"

______________________________________________________________________________________

# level 2.0
found the key in a function though ghidra
"xaech"

![Screenshot 2024-05-21 143424](https://github.com/adwait3/pwn-colez/assets/148553626/c36af266-0e19-4d54-9d63-3885dc3dd861)

we also find that the key is being manipulated 

![Screenshot 2024-05-21 143710](https://github.com/adwait3/pwn-colez/assets/148553626/11b5f653-5935-4627-81c9-10a2f57b2480)

 considering this key becomes 
 "xheca"

flag: "pwn.college{kZxlWNu39Yn40JjtyDCEtW0HBOw.01M1IDL0QTMyUzW}"


______________________________________________________________________________________

# level 2.1
found the key in a function though ghidra
"lodoc"
we iss its being manipulated and the 2nd nad 3rd bits are being replaced so we put the new key as
"loodc"
and we get the flag
![image](https://github.com/adwait3/pwn-colez/assets/148553626/9a4fc6c0-26c3-4f2d-bc09-a76cf2f72301)
this is where the manipulation takes place 

"local_16._2_1_" means the second bit 

flag: "pwn.college{g0LFemLGXiSlYFf0rmIfNvLPahe.0FN1IDL0QTMyUzW}"
______________________________________________________________________________________

# level 3.0
found the key in a function though ghidra
"qxkah"
we have to reverse this 
"hakxq"
and we get the flag

flag: "pwn.college{M1L8O1SZCiwkoQD54PzzwBlV-vb.0VN1IDL0QTMyUzW}"
______________________________________________________________________________________

# level 3.1
found the key in a function though ghidra
"cyeqg"
we have to reverse this 
"gqeyc"
and we get the flag

flag: "pwn.college{ILI3O-DsTEe0GtjmRI_r85NIWJl.0lN1IDL0QTMyUzW}"

______________________________________________________________________________________

# level 4.0
found the key in a function though ghidra
"bfpwx"
the program is performing a bubble sort so we just have to reverse that or just enter those particular bytes in any order
"bfpwx"
and we get the flag

flag: "pwn.college{UeQzj2JFiv2XaA_N7-0dXkx0Cvd.01N1IDL0QTMyUzW}"

______________________________________________________________________________________

# level 4.1
found the key in a function though ghidra
"biyzz"
the program is performing a bubble sort so we just have to reverse that or just enter those particular bytes in any order
"biyzz"
and we get the flag

flag: "pwn.college{IRIlfAj9RZqa3zdiBx5Hok8STCv.0FO1IDL0QTMyUzW}"

______________________________________________________________________________________

# level 5.0
found the key in a function though ghidra
"6d 65 68 73 67"
converting this to decimal
"mehsg"
and we get the flag

flag: "pwn.college{ANwP_AoWuZKeB7IqA1lZRci-0D_.0VO1IDL0QTMyUzW}"

______________________________________________________________________________________

# level 5.1
found the key in a function though ghidra
"a0 a0 bc ab ae"
xor key = "0xda"
after xor "7a 7a 66  71 74"
after reversing this to ascii
"zzfqt"
putting this 
and we get the flag

flag: "pwn.college{A7CFOKo-CYwiVuer7B_7f1cMsmS.0FM2IDL0QTMyUzW}"
______________________________________________________________________________________

# level 6.0

first our input is sawpped at 12 and 16 index 

the nits xored with key '0xe03c' odd bits by '3c' even bits by 'e0'

then its sorted

reversing xor
'e075 e077 e072 e073 e069 e069 e065 e061 e0be e0ba e0b4 e0b7 e0b1 e0af e0af e0af e0aa'

after swapping index

'e075 e077 e072 e073 e069 e069 e065 e061 e0be e0ba e0b4 e0b7 e0aa e0af e0af e0af e0b1'


exoexted result
'49 4b 4e 4f 55 55 59 5d 82 86 88 8b 8d 93 93 93 96'

A9 77 AE 73 B5 69 B9 61 62 BA 68 B7 76 AF 73 AF 6D


uWs7QeI9....ŏ¬֗

��ª�µµ¹badkmsrssv

uWs7QeI9adkmsrssv
uWs7QeIbadkmsrssv

finaly command for answer
'echo -e "\xA9\x77\xAE\x73\xB5\x69\xB9\x61\x62\xBA\x68\xB7\x6D\xAF\x73\xAF\x76" | ./babyrev_level6.0'
flag: "pwn.college{cvcoqWTpHfpaw-Owt4ztLaCVQnf.0VM2IDL0QTMyUzW}"



05 0b 4e 4f 51 58 59 6b 81 8b 93 93 93 95 96 a9 b1
05 0b 4e 4f 51 58 59 6b 81 8b 93 93 93 95 96 a9 b1
______________________________________________________________________________________

# level 6.1


flag: "pwn.college{A7CFOKo-CYwiVuer7B_7f1cMsmS.0FM2IDL0QTMyUzW}"
