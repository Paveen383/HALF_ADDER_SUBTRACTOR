
Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/user-attachments/assets/03875678-819e-45a7-bff5-e0c788478b48)


Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/user-attachments/assets/250d992d-7f35-4643-9537-abc8567ef497)


Figure -02 HALF Subtractor

**Truthtable**

![image](https://github.com/user-attachments/assets/8089d2a9-f73c-47ac-b753-3bc61307918b)

![image](https://github.com/user-attachments/assets/66b95bea-0dff-493a-b8c8-c071aa5f58f8)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:Paveen Kumaran SV

RegisterNumber:24000025

module halfadder (a,b,sum, carry);

input a,b;

output sum, carry;

assign sum= (a^b);

assign carry= ( a & b);

endmodule


module halfsubtractor(a,b,difference, borrow);

input a,b;

output difference, borrow;

assign difference= (a^b);

assign borrow= ( ~a & b);

endmodule

**RTL Schematic**

**Output/TIMING Waveform**

![image](https://github.com/user-attachments/assets/8519c469-9dc3-49eb-aa08-d6bda7acc95c)
![image](https://github.com/user-attachments/assets/dc44becd-bf02-4bbd-b804-e99528acb917)

**Result:**

 Thus the truth table of Half Adder & Subtractor in Quartus || using Verilog programming are studied, verified and executed successfully.
