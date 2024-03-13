# riscv-product-class
 Exercises from the Risc-V product class taught by Kunal Ghosh
 # Exercise 1. 
 ### Counter
 Comparing the counter code in RISC-V to x86 and ARM

 ![alt text](https://github.com/brickstackr/riscv-product-class/blob/main/ex1/ex1-1.png "comparing compiler output")

 The RISC-V code is significantly longer than the output from the x86 or ARM compilers. It is 74 lines, x86 was 60 lines of output, and the ARM compiler was 69 lines. With the reduced instruction set the compiler has to do more operations to make the code work. 

 ### Matrix Multiplication
![alt text](https://github.com/brickstackr/riscv-product-class/blob/main/ex1/ex1-2.png "comparing compiler output")

Once again the RISC-V code is significantly longer - the RISC-V output is 161 lines while the x86 compiler was only 124. 

The x86 code is mostly just mov and add instructions. 
The RISC-V code has a lot of SLLI (Shift Left Logical Immediate) instructions and load instructions. It's a little bit harder to read. 