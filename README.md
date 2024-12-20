# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module exp2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&`d|(~a&b&d)|(a&b&~c)));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:praisynithisha RegisterNumber:*/


**RTL realization**
![Screenshot 2024-11-25 225847](https://github.com/user-attachments/assets/622dc0f2-550e-4a27-9c86-dcf8f9af07b0)


**Timing Diagram**
![Screenshot 2024-11-25 230214](https://github.com/user-attachments/assets/65909bf4-e682-44f2-ae98-6f1ff1f9bb6c)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

