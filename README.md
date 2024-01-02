# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: YAZHINI S
RegisterNumber: 212223050062 
*/

##Code

module ex2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);

assign F1=x1|x2|x3|x4|x5;
endmodule


## RTL realization

![image](https://github.com/yazhini119/Experiment--02-Implementation-of-combinational-logic-/assets/155442058/e98a9ad9-338f-4771-987b-2def36d4340a)

Truth table :-

![image](https://github.com/yazhini119/Experiment--02-Implementation-of-combinational-logic-/assets/155442058/0c0cb102-649a-46d4-9d28-6fa0ab2135c8)

Timing Diagram :-

![image](https://github.com/yazhini119/Experiment--02-Implementation-of-combinational-logic-/assets/155442058/a3eb1313-2cd5-4860-b785-a75b5ce59c7f)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
