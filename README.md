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

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
```
module exp2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```
```
module exp2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

**RTL realization**
<img width="1436" height="757" alt="image" src="https://github.com/user-attachments/assets/0addd87b-d8eb-4482-b32a-4d6f5d4b1a7f" />



<img width="1522" height="738" alt="image" src="https://github.com/user-attachments/assets/7a5a43da-30b5-4891-b4c7-8588f5bc897b" />

**Output:**

**RTL**
<img width="1909" height="669" alt="image" src="https://github.com/user-attachments/assets/f7f83eb2-54f7-4dbf-a0fa-06da9c710357" />


<img width="1909" height="790" alt="image" src="https://github.com/user-attachments/assets/19f0202c-aa75-43f1-a361-922c474116af" />


**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

