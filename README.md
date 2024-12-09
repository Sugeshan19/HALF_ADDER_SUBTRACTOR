# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![experiment3 half adder logic diagram](https://github.com/user-attachments/assets/3c80950b-f046-42ff-bb92-a4ed16c12394)


Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

![experiment3 half subractor logic diagram](https://github.com/user-attachments/assets/fcaf0380-7265-42e1-9575-7c16a6f30110)

Figure -02 HALF Subtractor

**Truthtable**
![half adder truth table](https://github.com/user-attachments/assets/990364b4-f353-4d7b-a7bd-95d89dd97af6)

![half subtractor truth table](https://github.com/user-attachments/assets/ed7421ba-cf5f-44cd-ba77-33a83801af86)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:sugeshan
RegisterNumber:24007573

i)HALF ADDER

module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule

ii)HALF SUBTRACTOR

module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule


**RTL Schematic**
![experiment3 half adder waveform](https://github.com/user-attachments/assets/c4618a8f-395f-4683-8984-1eddf7863857)
![experiment3 half subractor waveform](https://github.com/user-attachments/assets/55b38c2a-5287-4ab8-84f7-d1dc19a78ed6)

**Output/TIMING Waveform**

**Result:**
The truth table of the specified half adder and half subtractor was successfully implemented and verified using Verilog
programming in Quartus II.

