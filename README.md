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

i)
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule



**RTL realization**


<img width="690" height="337" alt="image" src="https://github.com/user-attachments/assets/ee7d2fc5-c4bf-4601-ac39-e4cf741a55c7" />

**Output:**


<img width="698" height="713" alt="image" src="https://github.com/user-attachments/assets/47f0ec1b-ae2e-4527-816f-1e1658253cb9" />

**RTL**


<img width="942" height="495" alt="image" src="https://github.com/user-attachments/assets/a10fdc45-f40c-4c9b-9f4e-d0715d549927" />


**Timing Diagram**

<img width="942" height="507" alt="image" src="https://github.com/user-attachments/assets/c274fc5e-25ee-4eeb-aea0-aafc13112197" />


**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

