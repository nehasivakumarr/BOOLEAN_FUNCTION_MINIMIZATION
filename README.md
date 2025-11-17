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
assign f2=((~y & z)|( w & y )|(x & y));
endmodule




**RTL realization**

**Output:**
1.<img width="1920" height="1080" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/b33a63f2-4116-43b5-8fac-63aa5c0f217b" />
2.<img width="1920" height="1080" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/208bff76-0b19-4a81-acd5-e58fa5040359" />


**RTL**

**Timing Diagram**
1.<img width="1920" height="1080" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/eeb90e2a-0666-46b5-9ca9-d8ad7f65f2db" />
2.<img width="1920" height="1080" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/19abb72e-dc7a-4eb3-b284-670e4e7ea12e" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

