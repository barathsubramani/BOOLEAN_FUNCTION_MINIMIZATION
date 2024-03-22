# BOOLEAN_FUNCTION_MINIMIZATION

## Aim:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

## Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

## Software:

Quartus prime

## Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

## Program:

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Barath S

RegisterNumber: 212222230018
```
module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
//type code for f2 as like f1
endmodule
```
## RTL realization:
![image](https://github.com/barathsubramani/BOOLEAN_FUNCTION_MINIMIZATION/assets/118542617/05991aa5-b48d-41e6-b4a3-059145cb6660)


## Truthtable:
![image](https://github.com/barathsubramani/BOOLEAN_FUNCTION_MINIMIZATION/assets/118542617/0e14e5fb-fe1d-4736-b550-f014300e7c92)


## Output:
![image](https://github.com/barathsubramani/BOOLEAN_FUNCTION_MINIMIZATION/assets/118542617/1d3ffdbf-9d87-4708-8114-acffd9e40dbe)


## Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

