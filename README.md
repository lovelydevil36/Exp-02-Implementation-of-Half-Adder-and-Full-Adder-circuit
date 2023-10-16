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
Connect the supply (+5V) to the circuit Switch ON the main switch If the output is 1, then the led glows.

## Program:

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: Abdul hameed.H

RegisterNumber: 212222050001
HALFADDER:
```
module HalfAdder(A,B,sum,carry);
input A,B;
output sum,carry;
assign sum= A^B;
assign carry = A&B;
endmodule
```
## FULLADDER:
```
module FullAdder(A,B,Cin,sum,carry);
input A,B,Cin;
output sum,carry;
assign sum= A^B^Cin;
assign carry = (A&B)|((A^B)&Cin);
endmodule
```
## RTL diagram:

## HALFADDER

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/9fb1bea1-66f4-486f-9ade-9b36888a0725)


## FULLADDER

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/c98f6daf-d3aa-43cb-87e6-7d8549319e2d)


## Truth table:

## HALFADDER

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/23f416cb-4142-4125-ae74-2d5d899e2fe7)


## FULLADDER

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/a50ccde2-9e86-41d1-ab76-7fdaf67243f6)


## Output waveform:

## HALFADDER

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/6c51f6e8-1484-4b76-bb0a-f759489d7679)

## FULLADDER

![image](https://github.com/lovelydevil36/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/123564624/3edb8922-8f41-4e22-8dd3-ae22987524bd)


## Result:
Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.
