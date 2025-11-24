# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean function minimization is the process of simplifying Boolean algebraic
expressions to reduce the number of logic gates and complexity in a digital circuit,
leading to more efficient, faster, and less costly hardware

For minimizing Boolean expressions,we can use a set of rules and laws (like distributive,
associative, and complement laws) to simplify Boolean expressions. This method
focuses on applying algebraic manipulations to reduce the complexity of the expression

Identity Law A ⋅ 1 = A, A + 0 = A

Null Law A ⋅ 0 = 0, A + 1 = 1

Idempotent Law A ⋅ A = A, A + A = A

Complement Law A ⋅ A′ = 0, A + A' = 1

Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C

De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′

Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A

Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C

Commutative law A B = B A,A + B = B + A


**Logic Diagram**

IDENTITY LAW 

<img width="809" height="402" alt="image" src="https://github.com/user-attachments/assets/f692c216-c8f6-42d3-aca8-965fca58ef08" />

NULL LAW

<img width="647" height="306" alt="image" src="https://github.com/user-attachments/assets/b7830db5-8b3d-42b1-864c-f9884fbb2fcb" />


IDEMPOTENT LAW 

<img width="299" height="177" alt="image" src="https://github.com/user-attachments/assets/f6d33d53-7396-4340-a45a-a5675fe1d03d" />

COMPLEMENT LAW 

<img width="298" height="170" alt="image" src="https://github.com/user-attachments/assets/01e19260-434d-4dfa-ae69-f4c8a37ab4e7" />

DISTRIBUTIVE LAW

<img width="639" height="192" alt="image" src="https://github.com/user-attachments/assets/86dabb89-0c73-4218-af04-5dcf3222eff7" />

DEMORGAN'S LAW

<img width="671" height="573" alt="image" src="https://github.com/user-attachments/assets/e1446159-b348-44a7-a6f6-b30470af839a" />

ABSORPTION LAW

<img width="486" height="116" alt="image" src="https://github.com/user-attachments/assets/fdcb9d5c-1990-45aa-85d7-59c20b768a4a" />

ASSOCIATIVE LAW

<img width="329" height="353" alt="image" src="https://github.com/user-attachments/assets/0d82b6da-d51f-4999-9de9-4af31ac4b3cd" />

COMMUTATIVE LAW

<img width="345" height="336" alt="image" src="https://github.com/user-attachments/assets/654573c6-2759-4ee7-b343-da9b9fe8337f" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
```
1.module funct1(a,b,c,d,f1);
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
```



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

