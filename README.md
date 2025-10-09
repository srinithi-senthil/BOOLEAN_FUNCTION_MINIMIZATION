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
1)
module logic_function(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a&b&d)|(a&b&~c));
endmodule
2)
module EXP2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:S .Srinithi
RegisterNumber:25018743
date:13/09/2025


**RTL realization**
<img width="1398" height="827" alt="image" src="https://github.com/user-attachments/assets/9957b993-e2e0-4e15-a3c1-637cafa03d18" />
<img width="1427" height="802" alt="image" src="https://github.com/user-attachments/assets/f7b33053-8870-4893-aa7d-edf3cf289fb5" />

**Output:**

**RTL**
<img width="1690" height="308" alt="image" src="https://github.com/user-attachments/assets/5c5280c8-f180-42fa-a912-14ddd311a58a" />
<img width="1714" height="412" alt="image" src="https://github.com/user-attachments/assets/f9bdbc20-b1ee-45b6-b318-7162dada4464" />

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

