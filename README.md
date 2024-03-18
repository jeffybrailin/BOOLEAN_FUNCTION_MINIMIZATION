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
```
1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.
```

**Program:**
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Jeffy Brailin T
RegisterNumber:*/212223040076
module exp22(A,B,C,D,F1);
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

**Logic gate**
![e 2 2](https://github.com/jeffybrailin/BOOLEAN_FUNCTION_MINIMIZATION/assets/146911326/febb76bf-f953-4600-ab76-aa7019d82126)


**Wavwform**
![e 2 1](https://github.com/jeffybrailin/BOOLEAN_FUNCTION_MINIMIZATION/assets/146911326/aa5698df-3791-4710-a66e-ff824e96f5e7)

**Trurth table**
![e 2](https://github.com/jeffybrailin/BOOLEAN_FUNCTION_MINIMIZATION/assets/146911326/6272b0df-4edb-46e7-95fb-4fbc37340887)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

