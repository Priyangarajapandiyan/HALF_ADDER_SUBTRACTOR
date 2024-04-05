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
## half adder
![half adder](https://github.com/Priyangarajapandiyan/HALF_ADDER_SUBTRACTOR/assets/144872535/05df41ae-d18e-4e4a-9348-3defd50fbb8b)

## half subractor
![half subracter](https://github.com/Priyangarajapandiyan/HALF_ADDER_SUBTRACTOR/assets/144872535/225fbf49-b177-414f-8cc6-e879a3cfb815)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: R.PRIYANGA
RegisterNumber:212223230161
## half adder
```
module exp3(sum, carry,a,b); 
input a,b; 
output sum,carry; 
xor sum1(sum,a,b); 
and carry1(carry,a,b); 
endmodule
```
## half subractor
module exp3(diff,carry,a,b);
input a,b;
output diff,carry;
xor(diff,a,b);
assign carry=(~a)&b;
endmodule

**RTL Schematic half adder**
![RTL](https://github.com/Priyangarajapandiyan/HALF_ADDER_SUBTRACTOR/assets/144872535/ebe6fff9-b087-4749-9945-d35bd3531b74)
## half subracter
![comb](https://github.com/Priyangarajapandiyan/HALF_ADDER_SUBTRACTOR/assets/144872535/8141402d-4b5e-435e-9f8f-9d5a94a5846a)


**Output/TIMING Waveform**
## hald adder:
![sum carry](https://github.com/Priyangarajapandiyan/HALF_ADDER_SUBTRACTOR/assets/144872535/e055e266-a584-4cb9-9ff5-4ee2535f6692)

## half subractor 
![xy](https://github.com/Priyangarajapandiyan/HALF_ADDER_SUBTRACTOR/assets/144872535/f199cbe8-c696-4a78-b8b3-275d73db610c)

**Result:**
thus the half subracter and half adder circuits are design and the truth tables are verified using quartus software
