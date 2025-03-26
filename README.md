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
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: saravanan sham prakash

 RegisterNumber: 212224230254 */
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```

**RTL realization**
![image](https://github.com/user-attachments/assets/3294f9d3-18ca-43c3-9516-8b4b2706f2b3)

**Output:**
![image](https://github.com/user-attachments/assets/1671a522-1bfa-4366-9379-3c02c350be86)


**Timing Diagram**
![image](https://github.com/user-attachments/assets/5430747c-4ace-43bf-aaf3-53284ed298b4)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

