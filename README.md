# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit

## AIM:

To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

## Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

## Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

## Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

## Figure -02 FULL ADDER 

## Procedure

1.Connect the supply (+5V) to the circuit

2.Switch ON the main switch

3.
If the output is 1, then the led glows.
## Program:

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:Leann Joby Mathew
RegisterNumber:212222230074

# Half Adder
```
module halfadd(A,B,C,S);
input A,B;
output S,C;
xor(S,A,B);
and(C,A,B);
endmodule
```

# Full Adder
```
module fulladd(a,b,ci,s,co);
input a,b,ci;
output s,co;
wire d,e,f;
xor(d,a,b);
xor(s,d,ci);
and(e,ci,d);
and(f,a,b);
or(co,e,f);
endmodule

```

# Output:

## Half Adder
![Screenshot (56)](https://user-images.githubusercontent.com/119218812/229302815-e30936b9-c351-4e02-82e4-b91bd0b13994.png)
## Full Adder
![Screenshot (54)](https://user-images.githubusercontent.com/119218812/229302832-6e4030af-ea23-4d6e-a453-59164ff731d8.png)

## RTL REALIZATION
## Half Adder
![Screenshot (57)](https://user-images.githubusercontent.com/119218812/229302747-b9939b2e-7658-4cc4-9d63-2b3ff67d0ea3.png)
## Full Adder
![Screenshot (55)](https://user-images.githubusercontent.com/119218812/229302777-473f33e3-5a94-403c-a50f-c464de365bf5.png)

## TIMING DIAGRAM
## Half Adder
![image](https://user-images.githubusercontent.com/119218812/229303311-4cc97f7e-268f-4c02-b242-5540955099dc.png)


## Full Adder
![image](https://user-images.githubusercontent.com/119218812/229303026-e913d413-300c-4f6b-9bb7-81e976000a64.png)

## TRUTH TABLE 

## Half Adder
![image](https://user-images.githubusercontent.com/119218812/229302913-5c91df89-6238-4ecc-ba6e-6ba0dc2861bd.png)
## Full Adder
![image](https://user-images.githubusercontent.com/119218812/229302934-b0e96b9b-0719-4838-a617-41eb4f50a3f8.png)

### Result:

Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
