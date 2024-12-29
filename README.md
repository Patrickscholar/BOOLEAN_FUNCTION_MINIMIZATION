 # BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
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

assign f2=((~y & z)|( w & y )|(x & y));

endmodule


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:V.Patrick alex emmanuel

RegisterNumber: 24900019

```
**RTL realization**
<img width="1456" alt="Screenshot 2024-11-29 at 6 27 08 PM" src="https://github.com/user-attachments/assets/70e2fbc0-4479-43c7-bc7d-888e7658619f">



<img width="1449" alt="Screenshot 2024-11-29 at 9 30 16 PM" src="https://github.com/user-attachments/assets/9ea49f12-a8bc-4e54-88d9-7fa095c0ea37">



**RTL**
![image](https://github.com/user-attachments/assets/c6081c2a-33ae-4e8a-9229-41e99e9a083e)

![Screenshot 2024-12-29 185306](https://github.com/user-attachments/assets/bae7e351-85dd-4977-8d97-b50bddea353b)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

