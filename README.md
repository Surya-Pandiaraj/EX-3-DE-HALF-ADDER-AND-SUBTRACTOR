### NAME: SURYA P <br>
### REG NO: 212224230280

# EX 3 : HALF ADDER AND SUBTRACTOR

## AIM : 

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

## EQUIPMENTS REQUIRED :

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

## HALF ADDER :

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

## HALF SUBTRACTOR :

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF SUBTRACTOR

## TRUTH TABLE : 

![Screenshot 2025-04-07 134322](https://github.com/user-attachments/assets/30766049-961a-4226-82fb-b56333e06775)

![Screenshot 2025-04-07 134256](https://github.com/user-attachments/assets/6206bb78-6d6b-448e-8a50-f8e991a3e49f)


## PROCEDURE : 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

## PROGRAM :

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by : Surya P 

Register Number : 212224230280 */

```
module exp3(a,b,C,D,S,B);
input a,b;
assign S=a^b;
assign C=a&b;
assign D=a^b;
assign B=~a^b;
endmodule
```


## RTL SCHEMATIC : 

![image](https://github.com/user-attachments/assets/d73515c2-c84f-4734-96bd-da03861d7771)


## OUTPUT / TIMING WAVEFORM :

![Screenshot 2025-04-07 133712](https://github.com/user-attachments/assets/4a49afcb-f466-4d76-b0ac-35d14fb02cdd)

## RESULT : 

Half adder and Half subtractor circuits and its truth tables is verified using Verilog programming.
