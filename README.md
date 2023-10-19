# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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

Connect the supply (+5V) to the circuit Switch ON the main switch If the output is 1, then the led glows.

### 
Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Suji.G
RegisterNumber:  212222230152
## half adder
module exp3 (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

## Full adder
module exp3f (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule

````
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
## Half adder
![Screenshot 2023-09-01 084448](https://github.com/sujigunasekar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119559822/e9dc7f5e-dc70-4e29-9131-8fd59f3dd501)
## Full adder
![Screenshot 2023-09-01 093315](https://github.com/sujigunasekar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119559822/a6b454db-5835-409f-a536-b9609e37d9fb)

### TIMING DIAGRAM
## Haf adder
![Screenshot 2023-09-01 091137](https://github.com/sujigunasekar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119559822/4d087c38-297d-442a-9e41-84bc0f4e8329)
## full adder
![Screenshot 2023-09-01 093156](https://github.com/sujigunasekar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119559822/b053878e-60a3-417a-b56f-d7b72c7b3070)

### TRUTH TABLE
## Haf adder
![WhatsApp Image 2023-09-01 at 9 06 39 AM](https://github.com/sujigunasekar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119559822/ca7d6369-c68d-4ce1-a4c8-f54dae50702c)
## full adder
![WhatsApp Image 2023-09-01 at 9 06 38 AM](https://github.com/sujigunasekar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119559822/b659f9a7-4122-4b42-8ea0-da238d1b5e83)
 
### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
