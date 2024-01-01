## Name:Packiya Murugan R

## Register number:212223050034




# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

## Implementation-of-Half-Adder-and-Full-Adder-circuit
## AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher Software – Quartus prime Theory Adders are digital circuits
that carry out addition of numbers.

## Theory
Adders are digital circuits that carry out addition of numbers.

## Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

## Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

#### Figure -01 HALF ADDER:
![163552156-a13e5a56-c638-4110-97d9-8896907c8d25](https://github.com/packiyamurugan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168087/ea9e1739-c355-4203-8130-e8c9447eff8a)

#### Figure -02 FULL ADDER:
![163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d](https://github.com/packiyamurugan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168087/6ac0fd3e-27cf-4104-b108-6547adaaae76)


## Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.

## Program:

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog
programming. Developed by:Packiya murugan RegisterNumber:23014137


#### Half-adder:
module halfadder(a,b,sum,carry);

input a,b;

output sum,carry;

xor (sum,a,b);

and (carry,a,b);

endmodule

#### Full-adder:
module fulladder(a,b,c,sum,carry);

input a,b,c;

output sum,carry;

xor (sum,a,b,c);

assign carry=a&b | b&c | a&c;

endmodule

## TRUTH TABLE:
#### Half-adder:
 
![286606111-3b915795-1807-47ef-aefb-c6baedc0fa98](https://github.com/packiyamurugan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168087/346914af-6637-4b0c-9805-e0d92c6c6040)

#### Full-adder:

![286606277-d1fe435a-cf38-441c-b8d2-0421ee914b38](https://github.com/packiyamurugan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168087/1c73e201-8abb-416f-ada1-707515da6d5d)

## RTL realization:

#### Half-adder:

![286606525-ef77bab0-c8aa-42e2-8be0-b0c359fbc987](https://github.com/packiyamurugan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168087/6ac15db6-9df7-48fb-ae25-0b31b593896e)
 
#### Full-adder:

![286606657-0bc8d450-9831-49c1-a185-960faa6ee5a5](https://github.com/packiyamurugan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168087/650a3b32-04c6-4bf8-9ca6-70b572b6503a)

## TIMING DIAGRAM:

#### Half-adder:
![286607080-d14a0c56-9ab5-46ff-8253-ccfdc7d309fd](https://github.com/packiyamurugan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168087/5a9d0746-c415-4f87-b6a2-937ef93e114d)

#### Full-adder:

![286607206-db72b1d0-10da-448e-85f0-a771ee227e5c](https://github.com/packiyamurugan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168087/b0355bc7-5c11-4520-b21c-a71055f31b6d)

## Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
