# Experiment 02 Implementation of combinational logic:
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
 
 
## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime


## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

## Procedure:
Step 1: Create a project with required entities.

Step 2: Create a module along with respective file name.

Step 3: Run the respective programs for the given boolean equations.

Step 4: Run the module and get the respective RTL outputs.

Step 5: Create university program(VWF) for getting timing diagram.

Step 6: Give the respective inputs for timing diagram and obtain the results.
## Program:
```
Developed by: Harini.M 
RegisterNumber:212222240035

module Exp02(A,B,C,D,F1);
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
```
## RTL 
![image](https://github.com/Harinimuthu17/Experiment--02-Implementation-of-combinational-logic-/assets/130278614/775a009f-c58a-4250-80da-a893e1e87c51)

## Truth Diagram:
![image](https://github.com/Harinimuthu17/Experiment--02-Implementation-of-combinational-logic-/assets/130278614/1075aa23-91d9-433a-aec6-79a35faab8b0)
## Waveform verified:

![image](https://github.com/Harinimuthu17/Experiment--02-Implementation-of-combinational-logic-/assets/130278614/8cac7098-1126-4ab0-95e6-6e3cd14b6943)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
