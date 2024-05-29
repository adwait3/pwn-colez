__________________________________________________________________________
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
```echo -e "\xA9\x77\xAE\x73\xB5\x69\xB9\x61\x62\xBA\x68\xB7\x6D\xAF\x73\xAF\x76" | ./babyrev_level6.0```

flag: ```pwn.college{cvcoqWTpHfpaw-Owt4ztLaCVQnf.0VM2IDL0QTMyUzW}```



05 0b 4e 4f 51 58 59 6b 81 8b 93 93 93 95 96 a9 b1
05 0b 4e 4f 51 58 59 6b 81 8b 93 93 93 95 96 a9 b1
______________________________________________________________________________________

# level 6.1
in this the even bits are xord with 9d 

odd bits with 8f 


  81 89 91 93 94 95 9a 9f e5 ed ee f2 f6 f8 fc fe ff

  after xor
  
 1c 71 0c 6b 09 6d 07 67 78 15 73 0a 6b 00 61 06 62


finnal command 
```
echo -e "\x1c\x71\x0c\x6b\x09\x6d\x07\x67\x78\x15\x73\x0a\x6b\x00\x61\x06\x62" | ./babyrev_level6.1
```


flag: `pwn.college{kDAp2rjQYyTWIuFNBU_cz3d7YSW.0lM2IDL0QTMyUzW}`
______________________________________________________________________________________

# level 7.0

expected output

cd 4f 05 0e dd da 98 56 18 0b 97 d9 d0 56 03 0e 92 d6 cf 5e 0e 00 9b db d9 48 05 1b 9c

processes ibvolved 
>1. XOR even byte = 78 , odd byte = d0
>2. XOR multiple of 3 =1c , one more = 58 , 2 more = c7
>3. SWAP 6,4
>4. XOR odd = a6 , even de
>5. SWAP 3 , 20

reversing swap 

cd 4f 05 0e dd da 98 56 18 0b 97 d9 d0 56 03 0e 92 d6 cf 5e 0e 00 9b db d9 48 05 1b 9c

reversing xor 

13 e9 db a8 03 7c 46 f0 c6 ad 49 7f 0e f0 dd a8 4c 70 11 f8 d0 a6 45 7d 07 ee db bd 42

swaping 6 and 4

13 e9 db a8 46 7c 03 f0 c6 ad 49 7f 0e f0 dd a8 4c 70 11 f8 d0 a6 45 7d 07 ee db bd 42


xor 3%

0f b1 1c f0 5a bb 1f a8 61 b1 11 b8 12 a8 19 b4 14 b7 1c a0 67 b2 1d ba 1b b6 1c a1 1a


xor 

77 61 64 20 22 6b 67 78 18 61 69 68 6a 78 61 64 6c 67 64 70 1f 62 65 6d 65 56 64 71 62


converting from hex gives us teh key 
`123456789abcdefgh`

13 e9 db a8 46 7c 03 f0 c6 ad 49 7f 0e f0 dd a8 4c 70 11 f8 d0 a6 45 7d 07 ee db bd 42
0  1  2  3  4  5  6  7  8  9  10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28

13 a8 03 ad 0e a8 11 a6 07 bd
`0f b4 1f b1 12 b4 0d ba 1b a1`


e9 46 f0 49 f0 4c f8 a6 07 42
`b1 1e a8 11 a8 14 a0 fe 5f 1a`


db 7c c6 7f dd 70 d0 7d db
`1c bb b1 b8 1a b7 17 ba 1c`

0f b1 1c b4 1e bb 1f a8 b1 b1 11 b8 12 a8 1a b4 14 b7 0d a0 17 ba fe ba 1b 5f 1c a1 1a


after xor 
77 61 64 64 66 6b 67 78 c9 61 69 68 6a 78 62 64 6c 67 75 70 6f 6a 86 6a 63 8f 64 71 62


"x77\x61\x64\x64\x66\x6b\x67\x78\x79\x61\x69\x68\x6a\x78\x62\x64\x6c\x67\x75\x70\x6f\x6a\x86\x6a\x63\x8f\x64\x71\x62"
finnal command 
```
echo -e "\x77\x61\x64\x64\x66\x6b\x67\x78\x79\x61\x69\x68\x6a\x78\x62\x64\x6c\x67\x75\x70\x6f\x6a\x65\x6a\x63\x66\x64\x71\x62" | ./babyrev_level7.0
```


flag: `pwn.college{QdIgNS8Gad0cqeqN30dWIuZN5-s.01M2IDL0QTMyUzW}`

______________________________________________________________________________________

# level 7.1
expected result
wwuuuqpponkgiggkffeeeddbaaa




flag: `pwn.college{I-ClQh5noCs-WSFLL8LnDkKxPjn.0FN2IDL0QTMyUzW}`
______________________________________________________________________________________

# level 8.0

expected result

e8 b9 7b e4 85 b5 a5 ab ea dc 77 f2 bc 33 d9 2c 35 ed 23 05 2d 6d 2a 6f 0a ef 75 68 a1 53 3d a7 65 34 91 a1

after reversal

a1 91 34 65 a7 3d 53 a1 68 75 ef 0a 6f 2a 6d 2d 05 23 ed 35 2c d9 33 bc f2 77 dc ea ab a5 b5 85 e4 7b b9 e8

after modulo 5 

4c 8a 1b d6 09 d0 48 8e db db 02 11 40 99 c3 c0 1e 0c 5e 9b c1 c2 1c 0f 5c 9a c7 c5 18 0b 58 9e cb c8 17 05

after swap 

4c 8a d0 d6 09 1b 48 8e db db 02 11 40 99 c3 c0 1e 0c 5e 9b c1 c2 1c 0f 5c 9a c7 c5 18 0b 58 9e cb c8 17 05

after modulo 3

c1 1f 35 5b 9c fe c5 1b 3e 56 97 f4 cd 0c 26 4d 8b e9 d3 0e 24 4f 89 ea d1 0f 22 48 8d ee d5 0b 2e 45 82 e0

after modulo 3

14 92 ea 8e 11 21 10 96 e1 83 1a 2b 18 81 f9 98 06 36 06 83 fb 9a 04 35 04 82 fd 9d 00 31 00 86 f1 90 0f 3f

after modulo 6 

63 63 63 66 67 67 67 67 68 6b 6c 6d 6f 70 70 70 70 70 71 72 72 72 72 73 73 73 74 75 76 77 77 77 78 78 79 79

final key 

pwn.college{I-ClQh5noCs-WSFLL8LnDkKxPjn.0FN2IDL0QTMyUzW}

flag: `pwn.college{wtHH4NT0hpjANejMrc_18sl3GfW.0VN2IDL0QTMyUzW}`

______________________________________________________________________________________

# level 8.1

expected result

31 48 eb 01 3c 40 e6 0f 3c 44 e4 0c 3f 40 2f 0f 3b 5d fe 10 26 5f fd 14 27 58 fb 17 2c 54 f7 1e e3 53 f0

after reversal 

f0 53 e3 1e f7 54 2c 17 fb 58 27 14 fd 5f 26 10 fe 5d 3b 0f 2f 40 3f 0c e4 44 3c 0f e6 40 3c 01 eb 48 31

after swapping (7, 15)(2,20)

0  1  2  3  4  5  6  7  8  9  10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34

f0 53 2f 1e f7 54 2c 10 fb 58 27 14 fd 5f 26 17 fe 5d 3b 0f e3 40 3f 0c e4 44 3c 0f e6 40 3c 01 eb 48 31

after xor mod 4

61 61 64 66 66 66 67 68 6A 6A 6C 6C 6C 6D 6D 6F 6F 6F 70 77 72 72 74 74 75 76 77 77 77 72 77 79 7A 7A 7A

after swap (19,29)

61 61 64 66 66 66 67 68 6A 6A 6C 6C 6C 6D 6D 6F 6F 6F 70 72 72 72 74 74 75 76 77 77 77 77 77 79 7A 7A 7A

rest is bubble sort and reversal which can be ignored.

flag: `pwn.college{sjIXxOVcB4lSgirndF8kRPUn0wj.0lN2IDL0QTMyUzW}`


______________________________________________________________________________________

# level 9.0
expected result
1A F6 0E CD 6E A6 82 1B  1E 39 DA F9 1C 73 D7 69

first we take the file and see source code and figure out the part which needs patching.

![patch](https://github.com/adwait3/pwn-colez/assets/148553626/a8f8b634-9472-4f5e-b6f2-3cfa8f95c367)

in our case we want to change that jnz(condition jmp) to jz now we see the hex code

![hex](https://github.com/adwait3/pwn-colez/assets/148553626/b5a81322-47c8-4057-84ba-de06f4338033)

in this we see 75 that is basically the jnz to change  it to jz we change that byte to 74.

steps 
>1. run the file
>2. put adress as `1de1`
>3. put byte as 74
>4. put rest as 0 as they are unecessary



flag: `pwn.college{4tVxSLg5WPdFBWzx5lJE9rXJtKZ.01N2IDL0QTMyUzW}`

______________________________________________________________________________________

# level 9.1
steps 
>1. run the file
>2. put adress as `1e14`
>3. put byte as 74
>4. put rest as 0 as they are unecessary



flag: `pwn.college{E5b82AgKClGnhe0D7hpYFwch-dh.0FO2IDL0QTMyUzW}`


______________________________________________________________________________________

# level 10.0
steps 
>1. run the file
>2. put adress as `1db5`
>3. put byte as 74
>4. put rest as 0 as they are unecessary


flag: `pwn.college{M3TDXAZuCr4E1AKVmFmhLirGDjA.0VO2IDL0QTMyUzW}`


______________________________________________________________________________________

# level 10.1
steps 
>1. run the file
>2. put adress as `269e`
>3. put byte as 74
>4. put rest as 0 as they are unecessary

flag: `pwn.college{wkDyuFZRkMjp5uTv_mMOBl0eYd6.0FM3IDL0QTMyUzW}`
______________________________________________________________________________________

# level 11.0

in this level there is extra integreti hash also so we have to bypass that too.

steps 
>1. run the file
>2. put address as `1f3f`
>3. put byte as 74
>4. put address for second as `2d15`
>5. put byte as 74

flag: `pwn.college{ccfylxRASgoKdARmzuDM-0GMcT3.0VM3IDL0QTMyUzW}`
______________________________________________________________________________________

# level 11.1
steps 
>1. run the file
>2. put address as `223b`
>3. put byte as 74
>4. put address for second as `215a`
>5. put byte as 84

flag: `pwn.college{05jmNNjb5KPxGC7mKIY9a-1Gj7n.0lM3IDL0QTMyUzW}`
