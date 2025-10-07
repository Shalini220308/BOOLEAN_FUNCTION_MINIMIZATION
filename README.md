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
 focuses on applying algebraic manipulations to reduce the complexity of the expression
 by eliminating redundant terms.
 Identity Law A ⋅ 1 = A, A + 0 = A
 Null Law A ⋅ 0 = 0, A + 1 = 1
 Idempotent Law A ⋅ A = A, A + A = A
 Complement Law A ⋅ A′ = 0, A + A' = 1
 Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C
 De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′
 Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A
 Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C
 Commutative law A B = B A,A + B = B + A

**Logic Diagram**
Identity law
<img width="776" height="417" alt="image" src="https://github.com/user-attachments/assets/a0d05f79-41c1-4980-b2d5-03041e51ffae" />
Idempotent law
<img width="299" height="192" alt="image" src="https://github.com/user-attachments/assets/c497639b-ec0c-459c-8973-eed0b0254537" />
Complement law
<img width="301" height="177" alt="image" src="https://github.com/user-attachments/assets/7885e816-9bd1-4e41-b572-b093a7b62292" />
Distributive law
<img width="675" height="194" alt="image" src="https://github.com/user-attachments/assets/19e434ee-58e9-4911-9422-7b5d37c6aeb3" />
De-Morgan's law
<img width="650" height="612" alt="image" src="https://github.com/user-attachments/assets/4271df0f-c3b3-45a4-b8f2-a5d4990179cb" />
Absorption law
<img width="567" height="119" alt="image" src="https://github.com/user-attachments/assets/1a0c0a64-3cac-4b27-a164-6fcf9039806d" />
Assosiative law
<img width="399" height="371" alt="image" src="https://github.com/user-attachments/assets/68bf194d-8ed3-44b3-a3c2-94dd66488a8e" />
Commutative law
<img width="333" height="346" alt="image" src="https://github.com/user-attachments/assets/b0332261-5ef8-4c98-b74b-001e3d561cde" />
Null law
<img width="678" height="329" alt="image" src="https://github.com/user-attachments/assets/eb426b7f-ae21-447f-aac2-0d64c3cedc8b" />




**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/25009970

MINIMIZATION OF BOOLEAN FUNCTION
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


**Output:**

i)<img width="1666" height="848" alt="Screenshot 2025-10-07 083938" src="https://github.com/user-attachments/assets/71fa1feb-6c60-45e7-a9b5-babbe6c156f5" />
ii)![WhatsApp Image 2025-10-07 at 08 59 03_1f5eabd1](https://github.com/user-attachments/assets/16d6a802-e5ce-44b2-bef2-2955ccd5fb3c)
**RTL**


**Timing Diagram**
i)<img width="1420" height="521" alt="image" src="https://github.com/user-attachments/assets/511bee5f-b50b-4d2d-97a2-9b87bae07401" />
ii)<img width="1410" height="518" alt="image" src="https://github.com/user-attachments/assets/3e232cfc-ece0-4931-9162-25437d3f076f" />


**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

