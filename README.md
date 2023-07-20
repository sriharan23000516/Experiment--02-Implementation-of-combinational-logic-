# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
## NAME : J V SRIHARAN
## REGISTERNUMBER : 23000516
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
module combinationalcircuits(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire Abar,Bbar,Cbar,Dbar,A1,A2,A3,A4,A5;
assign Abar=~A;
assign Bbar=~B;
assign Cbar=~C;
assign Dbar=~D;
assign A1=Abar&Bbar&Cbar&Dbar;
assign A2=A&Cbar&Dbar;
assign A3=Bbar&C&Dbar;
assign A4=Abar&B&C&D;
assign A5=Bbar&Cbar&D;
assign F1=A1|A2|A3|A4|A5;
endmodule
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: 
RegisterNumber:  
*/
## RTL realization

## Output:
## RTL
## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
