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
Developed by: JAGANNIVASH U M
RegisterNumber:212224240059
```
```
module BFM(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module BFM1(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```


**TRUTH TABLE**
![image](https://github.com/user-attachments/assets/bce45391-4932-40bd-b78b-a91646c7736c)
![image](https://github.com/user-attachments/assets/02b58b3b-d970-4ae5-9efa-560d385c5ffe)


**RTL**
![image](https://github.com/user-attachments/assets/3ae9b87c-e823-4b47-9e44-d08b90665afa)

![image](https://github.com/user-attachments/assets/67a218d2-49e3-4faa-8ff6-2d41993219e2)

**Timing Diagram**
![image](https://github.com/user-attachments/assets/1d42a2f9-8532-46db-a17f-25b52953fbb9)
![image](https://github.com/user-attachments/assets/8d4dc75f-a6a7-46d5-9c0f-235f94ede008)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

