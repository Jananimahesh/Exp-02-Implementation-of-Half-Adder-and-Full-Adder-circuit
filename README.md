# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: janani.m
RegisterNumber: 22006734
HALF ADDAR
module halfaddar(A,B,sum,carry);
input A,B;
output sum,carry;
xor(sum,A,B);
and(carry,A,B);
endmodule
FULL ADDAR
module fulladdar(A,B,C,sum,carry);
input A,B,C;
output sum,carry;
assign sum = ((A^B)^C);
assign carry = ((A&B)|(B&C)|(C&A));
endmodule
*/
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
 RTL realization for Half Addar
 
 ![Screenshot (9)](https://user-images.githubusercontent.com/119432417/211161114-9b72f368-827f-422b-a0b3-102b2bda337c.png)
 
 RTL realization for Full Addar
 
 ![Screenshot (10)](https://user-images.githubusercontent.com/119432417/211161645-8defa436-fbad-4ece-9dc6-ffb887cb4ee4.png)


### TIMING DIAGRAM
The timing diagram for Half Addar

![image](https://user-images.githubusercontent.com/119432417/211162222-8bc2eaf6-80c0-4f4c-9b4c-208a63442d31.png)

The timing diagram for Full Addar

![image](https://user-images.githubusercontent.com/119432417/211162314-b1110ea8-5702-4968-a94e-c6d2d7f5fd66.png)



### TRUTH TABLE 
THE TRUTH TABLE FOR HALF ADDAR

![image](https://user-images.githubusercontent.com/119432417/211161796-be6d8c6e-7a68-4e4e-9db6-730bee496ae3.png)
THE TRUTH TABLE FOR FULL ADDAR

![image](https://user-images.githubusercontent.com/119432417/211161845-d284b1b8-a597-4dcb-882e-97355cb6a7bd.png)


### Result:
Thus the Half Addar and Full Addar circuit was succesfully implemented
