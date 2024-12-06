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

module ex2(a,b,c,d,o);
input a,b,c,d;
output o;
assign o=((~a & ~b & ~c & ~d)|(a & ~c & ~d)|(~b & c & ~d)|(~a & b & c & d)|(b & ~c & d));
endmodule



module ex22(w,x,y,z,o);
input w,x,y,z;
output o;
assign o=((x & ~y & z)|( ~x & ~y & z )|( ~w & x & y)|(w & ~x & y)|(w & x & y));
endmodule 


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: praveena D 
RegisterNumber: 24003392


**RTL realization**
![Screenshot 2024-11-29 154015](https://github.com/user-attachments/assets/e4ab7323-22e8-4ca3-8cb1-6fae6f018ed3)

![Screenshot 2024-12-06 104602](https://github.com/user-attachments/assets/25ac50bb-6577-4d50-b64a-e3ca0e2a04ae)



**RTL**
![Screenshot 2024-11-29 154310](https://github.com/user-attachments/assets/02666618-28e9-4d88-8020-98a5884419c2)
![image](https://github.com/user-attachments/assets/4b212a1f-aa45-4204-a981-b6055cd4fe1a)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

