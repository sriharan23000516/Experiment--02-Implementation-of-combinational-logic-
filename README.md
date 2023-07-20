# Experiment--02-Implementation-of-combinational-logic
IMPLEMENTATION OF COMBINATIONAL LOGICAL GATES
## NAME : J V SRIHARAN
## REGISTERNUMBER : 23000516
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime


## Theory:

A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.
 

## Procedure:

1. Create a New Project:
   - Open Quartus and create a new project by selecting "File" > "New Project Wizard."
   - Follow the wizard's instructions to set up your project, including specifying the project name, location, and target device (FPGA).

2. Create a New Design File:
   - Once the project is created, right-click on the project name in the Project Navigator and select "Add New File."
   - Choose "Verilog HDL File" or "VHDL File," depending on your chosen hardware description language.

3. Write the Combinational Logic Code:
   - Open the newly created Verilog or VHDL file and write the code for your combinational logic.
     
4. Compile the Project:
   - To compile the project, click on "Processing" > "Start Compilation" in the menu.
   - Quartus will analyze your code, synthesize it into a netlist, and perform optimizations based on your target FPGA device.

5. Analyze and Fix Errors:*
   - If there are any errors or warnings during the compilation process, Quartus will display them in the Messages window.
   - Review and fix any issues in your code if necessary.
   - View the RTL diagram.

6.*Verification:
   - Click on "File" > "New" > "Verification/Debugging Files" > "University Program VWF".
   - Once Waveform is created Right Click on the Input/Output Panel > " Insert Node or Bus" > Click on Node Finder > Click On "List" > Select All.
   - Give the Input Combinations according to the Truth Table amd then simulate the Output Waveform.
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

## RTL realization:

![image](https://github.com/sriharan23000516/Experiment--02-Implementation-of-combinational-logic-/assets/139841769/802d6cb3-a930-4485-9aab-39ed6e9bf0c9)


TRUTH TABLE:











![image](https://github.com/sriharan23000516/Experiment--02-Implementation-of-combinational-logic-/assets/139841769/51ee5a1b-1a49-4b85-a0b1-b5d5f6f1fa6d)





## Timing Diagram:


![image](https://github.com/sriharan23000516/Experiment--02-Implementation-of-combinational-logic-/assets/139841769/5a49a2e2-1a59-4198-899f-92f0017846d1)



## Result:
Thus the given logic function is implemented using and or and not gate and their operations are verified using Verilog programming.
