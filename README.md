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
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: PREETHA.S
RegisterNumber: 212222230110

1. Program to design a half adder:

module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule 

2. Program to design a full adder:

module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
```

### TRUTH TABLE
### HALF ADDER
![Screenshot 2023-09-13 233423](https://github.com/Preetha-Senthamilan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119390282/45b15cd6-ab7d-44d9-aa7d-2c2ab14bce6a)

### FULL ADDER
![Screenshot 2023-09-13 233431](https://github.com/Preetha-Senthamilan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119390282/eb06802f-0402-4a8f-bba7-4a679d498f23)


### WAVEFORM
### HALF ADDER
![Screenshot 2023-09-13 233556](https://github.com/Preetha-Senthamilan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119390282/9bc88d99-e314-4edf-bbf0-109d84c15a5d)

### FULL ADDER
![Screenshot 2023-09-13 233606](https://github.com/Preetha-Senthamilan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119390282/a702a27a-5e15-49b3-b7c0-ca23a85402b6)

### RTL DIAGRAM
### HALF ADDER
![Screenshot 2023-09-13 233239](https://github.com/Preetha-Senthamilan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119390282/151094e1-2cc5-440c-83e5-b9be3c3f6abf)

### FULL ADDER
![Screenshot 2023-09-13 233247](https://github.com/Preetha-Senthamilan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119390282/b108f1d3-dd55-4584-acfe-4f67b30b9669)




### Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

