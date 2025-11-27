# BOOLEAN_FUNCTION_MINIMIZATION
### Name:G SANJAY
### Reg No:212224230243
**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Logic function is implemented using Verilog, a hardware description language used to model electronic systems. Verilog enables the design and simulation of digital circuits efficiently. Quartus software is utilized to compile, synthesize, and verify the logic function through simulation. This process ensures the functionality aligns with the expected behavior of the logic design.


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

module DE2(A, B, C, D, W, X, Y, Z, F1,F2);

input A, B, C, D, W, X, Y, Z;

wire x1, x2, x3, x4, x5, x6, x7, x8, x9, x10;

output F1, F2;

assign x1=(~A) & (~B) & (~C) & (~D);

assign x2=(A)&(~C)&(~D);

assign x3=(~B)&(C)&(~D);

assign x4=(~A)&(B)&(C)&(D);

assign x5=(B)&(~C)&(D);

assign x6=(X)&(~Y)&(Z);

assign x7=(~X)&(~Y)&(Z);

assign x8=(~W)&(X)&(Y);

assign x9=(W)&(~X)&(Y);

assign x10=(W)&(X)&(Y);

assign F1=x1|x2|x3|x4|x5;

assign F2=x6|x7|x8|x9|x10;

endmodule 


**RTL realization**

![Screenshot (75)](https://github.com/user-attachments/assets/49728223-7198-4966-acd7-d2e4d62c2a63)




**Output:**

![388523450-42267acf-5bb4-43ba-9b18-b0551e02a1df](https://github.com/user-attachments/assets/592d3d92-47a3-4581-be04-a4a12b94c5f4)






**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

