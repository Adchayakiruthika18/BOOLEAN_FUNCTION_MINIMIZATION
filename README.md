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

Developed by: Adcahayakiruthika M S

RegisterNumber: 212223230005
```
module combinationalcircuit(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```

**RTL realization**

![image](https://github.com/Adchayakiruthika18/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139995/24c987ff-f7a7-4416-8b33-c7b8f488d380)

**Timetable**

![image](https://github.com/Adchayakiruthika18/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139995/0e5bb7e2-0035-44eb-ac54-de1087708a01)

**Timing Diagram**

![image](https://github.com/Adchayakiruthika18/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139995/3f87a322-8dd5-4460-9cb8-392acb26434c)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

