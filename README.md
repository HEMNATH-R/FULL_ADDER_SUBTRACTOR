# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**


![tt 1](https://github.com/user-attachments/assets/67eb0e49-08cd-4b3e-8f0e-60e6f8b5f1e4)

![tt2](https://github.com/user-attachments/assets/40bd7bb5-60fb-4f8a-ac36-6a59008bd59d)




**Procedure**

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by:HEMNATH R

RegisterNumber:24010023

i)FULL ADDER

module fa(a,b,cin,sum,carry);

input a,b,cin;

output sum,carry;

assign sum=( (a ^ b)^c);

assign carry= ( (a & b)| ( cin &(a ^ b ));

endmodule

ii)FULL SUBTRACTOR

module fs(a,b,difference,borrow);

input a,b,bin;

output difference,borrow;

assign difference= ( (a ^ b)^bin);

assign borrow= ( ( a & b)| ( bin & ((a ^ b )));

endmodule

*/

**RTL Schematic**
![exp 4,1](https://github.com/user-attachments/assets/ea992af9-0aa3-4a6e-b2f6-3c2c1143f77d)

![exp 4,2](https://github.com/user-attachments/assets/05ec7518-9164-49a2-a40c-71b544e33995)





**Output Timing Waveform**

![exp t 4,1](https://github.com/user-attachments/assets/e8694b30-7646-4046-bdc1-6251638257d9)

![exp 4 t,2](https://github.com/user-attachments/assets/a5174d62-23bf-4804-b356-044f4d64228e)



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



