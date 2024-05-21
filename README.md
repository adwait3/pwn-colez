# pwn-colez
![image](https://github.com/adwait3/pwn-colez/assets/148553626/e36f4dc6-6f3c-4183-b55a-a505f3fbe238)


As an example, say:
  [0x1330] = 0x00000000deadc0de

If you examined how it actually looked in memory, you would see:
  [0x1330] = 0xde
  [0x1331] = 0xc0
  [0x1332] = 0xad
  [0x1333] = 0xde
  [0x1334] = 0x00
  [0x1335] = 0x00
  [0x1336] = 0x00
  [0x1337] = 0x00

This format of storing things in 'reverse' is intentional in x86, and its called "Little Endian".

For this challenge we will give you two addresses created dynamically each run.

The first address will be placed in rdi.
The second will be placed in rsi.

Using the earlier mentioned info, perform the following:
  Set [rdi] = 0xdeadbeef00001337
  Set [rsi] = 0xc0ffee0000

Hint: it may require some tricks to assign a big constant to a dereferenced register.
Try setting a register to the constant value then assigning that register to the dereferenced register.

We will now set the following in preparation for your code:
  [0x404350] = 0xffffffffffffffff
  [0x404b48] = 0xffffffffffffffff
  rdi = 0x404350
  rsi = 0x404b48




  ______________________________________________________________________

  # lvl 30
  flag 
  'pwn.college{MLzCLKNQtI2x9682P8Alfyrn3sR.0lNxIDL0QTMyUzW}'
