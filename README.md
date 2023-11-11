# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit
### Implementation-of-Half-Adder-and-Full-Adder-circuit

## AIM:

To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## Components Required:
Hardware – PCs, Cyclone II , USB flasher Software – Quartus prime

## Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

## Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

## Figure -01 HALF ADDER

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/3a52b3e4-4ac5-4301-88f7-bb8c43e59a2f)


![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/eca00c86-05ed-4de9-b7cb-900d8148374d)


## Figure -02 FULL ADDER

## Procedure
1.Create a New Project:

Open Quartus and create a new project by selecting "File" > "New Project Wizard." Follow the wizard's instructions to set up your project, including specifying the project name, location, and target device (FPGA).

2.Create a New Design File:

Once the project is created, right-click on the project name in the Project Navigator and select "Add New File." Choose "Verilog HDL File" or "VHDL File," depending on your chosen hardware description language.

3.Write the Combinational Logic Code:

Open the newly created Verilog or VHDL file and write the code for your combinational logic.

4.Compile the Project:

To compile the project, click on "Processing" > "Start Compilation" in the menu. Quartus will analyze your code, synthesize it into a netlist, and perform optimizations based on your target FPGA device.

5.Analyze and Fix Errors:

If there are any errors or warnings during the compilation process, Quartus will display them in the Messages window. Review and fix any issues in your code if necessary. View the RTL diagram.

6.Verification:

Click on "File" > "New" > "Verification/Debugging Files" > "University Program VWF". Once Waveform is created Right Click on the Input/Output Panel > " Insert Node or Bus" > Click on Node Finder > Click On "List" > Select All. Give the Input Combinations according to the Truth Table and then simulate the Output Waveform.

## Program:

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: Abdul hameed.H

RegisterNumber: 212222050001

# HALFADDER:
```
module exppp(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= a^b;
assign carry = a&b;
endmodule
```
## FULLADDER:
```
module full(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum= a^b^cin;
assign carry = (a&b)|((a^b)&cin);
endmodule
```

# OUTPUT:


# Half adder Truthtable:
![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/4fd32e44-d9cb-4277-9402-0593bcda9ffa)



# Half Adder RTL realization:

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/65040246-06f9-4efe-af82-15dd0271a415)


# Timing Diagram Half Adder:

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/0f9465e5-e021-47b1-91c2-f6ccd481cfc8)




# Full adder Truthtable:

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/3f998759-5a89-4fee-b500-27c818e7621d)

# Full Adder RTL realization:

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/b5398a74-e168-462e-8417-ec6b01816d6f)


# Timing Diagram Full Adder:

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/6dec24c9-278e-474f-bf20-a36afd70d837)








## Result:
Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.
