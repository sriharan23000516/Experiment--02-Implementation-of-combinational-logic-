### Name: SRIHARAN J V
### Reg-no:23000516

# Experiment--02-Implementation-of-combinational-logic
 
## AIM:-
To implement the given logic function verify its operation in Quartus using Verilog programming.
#### F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
 
## Equipments Required:-
#### Hardware – 
PCs, Cyclone II , USB flasher
#### Software – 
Quartus prime

## Theory:-
A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.
 
## Procedure:-

### Create a New Project:-
   - Open Quartus and create a new project by selecting "File" > "New Project Wizard."
   - Follow the wizard's instructions to set up your project, including specifying the project name, location, and target device (FPGA).

### Create a New Design File:-
   - Once the project is created, right-click on the project name in the Project Navigator and select "Add New File."
   - Choose "Verilog HDL File" or "VHDL File," depending on your chosen hardware description language.

### Write the Combinational Logic Code:-
   - Open the newly created Verilog HDL file and write the code for your combinational logic.
     
### Compile the Project:-
   - To compile the project, click on "Processing" > "Start Compilation" in the menu.
   - Quartus will analyze your code, synthesize it into a netlist, and perform optimizations based on your target FPGA device.

### Analyze and Fix Errors:-
   - If there are any errors or warnings during the compilation process, Quartus will display them in the Messages window.
   - Review and fix any issues in your code if necessary.
   - view the RTL diagram. 

### Verification:-
   -  Click on "file" > "new" in the file.
   -  Choose the Univeristy Program VWF under the verification/debugging files.
   -  once waveform is created Right click on the blank space at left column . Choose insert nodes or bus... option in the tab .
   -  Now open the list and select all and click ok.
   -  Give the input combination according to truth table and stimulate the output waveform.  

## Program:-
![WhatsApp Image 2023-07-20 at 09 45 24](https://github.com/Shilo-05/Experiment--02-Implementation-of-combinational-logic-/assets/139841664/d3b53505-ba69-4890-bf0c-bfb8b92fff4b)
## RTL realization:-
![WhatsApp Image 2023-07-20 at 09 45 12](https://github.com/Shilo-05/Experiment--02-Implementation-of-combinational-logic-/assets/139841664/24f98cd7-2ad2-4506-8478-0d77f6ebfb02)
## Truth Table:-
![WhatsApp Image 2023-07-20 at 09 44 28](https://github.com/Shilo-05/Experiment--02-Implementation-of-combinational-logic-/assets/139841664/2a81e37c-a572-4584-b567-6b32dc982b9d)
## Timing Diagram:-
![WhatsApp Image 2023-07-20 at 09 44 43](https://github.com/Shilo-05/Experiment--02-Implementation-of-combinational-logic-/assets/139841664/daa9659f-a49a-4d49-a1e3-aad8706d04e2)
## Result:-
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming
