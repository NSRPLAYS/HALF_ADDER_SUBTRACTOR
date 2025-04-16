# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-//Half Subtractor-circuit
dd
**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**
///////////////
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
half adder
![half adder trurth](https://github.com/user-attachments/assets/610de5b8-9336-44dd-8a58-694af93f727d)

half sub
![half sub truth](https://github.com/user-attachments/assets/d7d7ae1e-610e-4786-9720-74f201620242)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: 
RegisterNumber: 212224240103
Name:B.Naveen sairam
```
*half subractor:
 module ex3halfsub(A,B,D,BO);
 input A,B;
 output D,BO;
 xor(D,A,B);
 and(BO,~A,B);
 endmodule
*half adder:
 module experiment(A,B,C,S)
 input A,B
 output S,C
 xor (S,A,B);
 and (C,A,B);
 endmodule
```
**RTL Schematic**
# half adder
![half adder](https://github.com/user-attachments/assets/f4ff7e04-95e4-4e14-997f-583e866591ca)

# half subractor
![half sub](https://github.com/user-attachments/assets/a3016de9-c652-470e-96a6-2e58c1dba5da)


**Output/TIMING Waveform**
half adder wave
![half add wave](https://github.com/user-attachments/assets/48870abf-0b8a-46bb-8f12-91cc8cd3bbb3)

half subractor
![half sub wave](https://github.com/user-attachments/assets/6408d763-92dd-46c1-85e9-f203aab169a9)

**Result:**
The code is excecuted successfully.

