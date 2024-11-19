## EX 02 : BOOLEAN_FUNCTION_MINIMIZATION
### Date : 22/09/24
## **AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

## **Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

## **Software – Quartus prime**

## **Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## **Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
Developed by: VISHAL.MA
RegisterNumber: 212222230177

module EXP_2(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
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
```
## **RTL realization**
![ex 2 rtl](https://github.com/user-attachments/assets/db506106-c363-44f7-a93e-582dad2044c2)



## **Output:**
![ex 2 out](https://github.com/user-attachments/assets/9b1ae286-1284-47a6-bdbe-79265ae2c5a7)


## **Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

