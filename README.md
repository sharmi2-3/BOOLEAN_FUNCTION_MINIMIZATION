# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. Itis fundamental to digital logic design and computer science, providing a mathematicalframework for describing logical operations and expressions

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:SHARMILA .P                   RegisterNumber:24900072*/
```
module fun2a(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule;
```
```
module fun2b(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(w&y)|(x&y));
endmodule;
```

**Output:**

![WhatsApp Image 2024-12-10 at 12 58 31_ba3d0f0d](https://github.com/user-attachments/assets/ea66cad0-b722-4f81-a0c4-aa5c7e15ee59)
![WhatsApp Image 2024-12-10 at 13 00 16_fc1222e6](https://github.com/user-attachments/assets/0e1d4fe5-1e8d-4578-b596-e3cc195fab69)

**RTL**

![WhatsApp Image 2024-12-10 at 12 59 55_6917ca07](https://github.com/user-attachments/assets/738d3e47-342a-4268-a4fa-57401e901a49)
![WhatsApp Image 2024-12-10 at 13 00 35_6fa28494](https://github.com/user-attachments/assets/d8a4392f-d37f-4ece-b2a5-3054def1d0e9)

**Timing Diagram**

![WhatsApp Image 2024-12-02 at 19 14 08_d536c8cb](https://github.com/user-attachments/assets/85e1ba27-4c66-4240-93ce-9ae9cc379af4)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

