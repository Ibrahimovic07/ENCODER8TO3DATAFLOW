### ENCODER 8TO3 DATAFLOW Modelling

```
Developed by: mohammed ibrahim mm
RegisterNumber:21222310034

```
**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

1. Open Quartus Prime and create a new Verilog project.
2. Write the Verilog code for Encoder 8 to 3 using Dataflow Modeling.
3. Compile and check for syntax errors.
4. Create a testbench to validate the encoder's functionality.
5. Simulate and verify the output against the truth table.
6. Analyze the RTL and timing diagrams.

**PROGRAM**

Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 


```verilog
// Program for Encoder 8 To 3 in Dataflow Modelling

module encoder8to3 (
    input [7:0] D,
    output A0, A1, A2
);

assign A0 = D[1] | D[3] | D[5] | D[7];
assign A1 = D[2] | D[3] | D[6] | D[7];
assign A2 = D[4] | D[5] | D[6] | D[7];

```


**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

The RTL schematic can be viewed in Quartus Prime after successful compilation using the RTL Viewer tool.

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

Simulate the design to generate timing diagrams and confirm the outputs align with the expected truth table values.

**RESULTS**

 The Encoder 8 To 3 was successfully implemented using Dataflow Modelling in Verilog. The functionality was verified against the truth table using simulation, and the outputs matched as expected.
            



