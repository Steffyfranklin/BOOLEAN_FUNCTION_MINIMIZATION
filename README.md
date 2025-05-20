# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values-true and false.It is fundamental to digital logic design and computer science,providing a mathamatical framework for describing logical operation and expressions.

**Logic Diagram**
1.F1
![image](https://github.com/user-attachments/assets/019e3e00-5446-408a-9ff3-dd17208d122c)

2.F2
![image](https://github.com/user-attachments/assets/b7dbf593-10bf-4540-8b90-b62900848cc8)

**Boolean Function Minimization**
1.F1
![image](https://github.com/user-attachments/assets/f7fe52fb-2abe-43c8-870b-78b8d9abaff7)

2.F2
![image](https://github.com/user-attachments/assets/301a7bd3-7845-4c83-871c-687be577caae)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

1.F1
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```

2.F2
```
module funct2(w,x,y,z,f2);
intput w,x,y,z;
output f2;
assign f2=((~y & z)|(w & y)|(x &y));
endmodule
```

Developed by:Steffy Aavlin Raj.F.S RegisterNumber: 212224040330

**RTL**
1.F1
![image](https://github.com/user-attachments/assets/18badee7-6755-4179-b35d-47f714d41d3f)

2.F2
![image](https://github.com/user-attachments/assets/4b022185-8cf1-49b1-a86a-8f7bddae8a4a)

**Timing Diagram**
1.F1
![image](https://github.com/user-attachments/assets/5fc8879d-b15d-47d6-9f9d-d8fbca1cc55e)

2.F2
![image](https://github.com/user-attachments/assets/988f89cf-1801-46f1-8989-558ef9d69c78)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

