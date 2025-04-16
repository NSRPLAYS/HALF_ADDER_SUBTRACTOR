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

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
# half adder:
![half adder trurth](https://github.com/user-attachments/assets/9b5aa9d6-480f-4a31-9f63-f56242a84495)

# half subractor:
![half subrac](https://github.com/user-attachments/assets/1bcdd7cd-6dbd-468b-b21e-34072ee158ba)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:
RegisterNumber:212224240103
Name:B.Naveen sairam
```
* half adder
  module experiment(A,B,C,S)
  input A,B
  output S,C
  xor (S,A,B);
  and (C,A,B);
  endmodule
*half subractor
 module ex3halfsub(A,B,D,BO);
 input A,B;
 output D,BO;
 xor(D,A,B);
 and(BO,~A,B);
 endmodule
```
**RTL Schematic**
# half adder:
![half adder](https://github.com/user-attachments/assets/c8965f49-0e91-4f8b-8ade-6646be07ef60)
# half subractor:
![half sub](https://github.com/user-attachments/assets/8dd7e17b-1ab1-458d-a92a-83eec0c95d8e)

**Output/TIMING Waveform**
# half adder:
![half add wave](https://github.com/user-attachments/assets/2ffb79e4-2d7c-4b8d-a6ff-2af6b5ad51a7)
# half subractor:
![half sub wave](https://github.com/user-attachments/assets/996486c6-aa59-4867-bb81-85fea16cc748)


**Result:**
The code is excecuted successfully.
