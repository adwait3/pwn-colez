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
