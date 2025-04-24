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
module boolean(A,B,C,D,F1,w,x,y,z,F2);
input A,B,C,D,w,x,y,z;
output F1,F2;
wire x1,x2,x3,x4,x5,x6;
assign x1=(~B)&(~D);
assign x2=A&B&(~C);
assign x3=(~A)&(B)&(D);
assign x4=(~x)&(z);
assign x5=(x)&(y);
assign x6=(w)&(y);
assign F1=x1|x2|x3;
assign F2=x4|x5|x6;
endmodule
/*
```

**RTL realization**
![image](https://github.com/user-attachments/assets/09bb3675-f14a-4024-8734-e075a0d771bf)

**Output:**
![WhatsApp Image 2025-04-24 at 10 55 14_f980eb0e](https://github.com/user-attachments/assets/f7bbc77f-b483-406a-a04a-739496dd1573)



**Timing Diagram**

![image](https://github.com/user-attachments/assets/ab479ca2-b340-41bf-aba7-e62674f18446)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

