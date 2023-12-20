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


Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Mario Viofer.J
RegisterNumber:  212223100032

Program:
/*
Half adder:
module halfadder(sum,a,b,carry);
input a,b;
output sum,carry;
xor (sum,a,b);
and (carry ,a,b);
endmodule

Full adder:
module fulladder(a,b,c,sum,carry);
input a,b,c;
output sum, carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c;
endmodule

Logic symbol & Truthtable
RTL realization

### Output:
### RTL
Half adder:

![image](https://github.com/Mario-Viofer-J/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979232/73fe3092-5778-4b45-a055-2415e097ed44)

Full adder:

![image](https://github.com/Mario-Viofer-J/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979232/d70cc2be-d4b8-467c-b056-ec576e1681ff)

### TIMING DIAGRAM
Half adder:

![image](https://github.com/Mario-Viofer-J/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979232/1a2b560c-7cbb-4e52-bf83-70cefedf24ff)

Fulladder:

![image](https://github.com/Mario-Viofer-J/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979232/b44e4539-90e8-4b81-aa72-eb12b12f4443)

### TRUTH TABLE 
Half adder:

![image](https://github.com/Mario-Viofer-J/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979232/6ba3dfb6-d6e1-4620-9edb-722b3d8255cd)

Full adder:

![image](https://github.com/Mario-Viofer-J/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979232/c4630770-a88b-40d5-807c-00203f12e640)

### Result:
Thus the given full adder and half adder are verified using verilog programming.
