### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

**PROGRAM**

Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by: MERIL GOLDLINA A   RegisterNumber: 24007299

![image](https://github.com/user-attachments/assets/dd7cd9f5-33c7-4d83-9a8d-39079d57a9b0)


**RTL LOGIC UP COUNTER**

![image](https://github.com/user-attachments/assets/6cd58fcf-30d6-4565-93de-27200b526442)

**TIMING DIAGRAM FOR IP COUNTER**

![398536078-0bce2bd5-2b91-4971-b1e0-a4a52945a493](https://github.com/user-attachments/assets/7876595a-c3fb-4dee-98ae-7dbb3129b788)


**TRUTH TABLE**

![398781957-b5dc43b9-bdc7-491f-a8a9-54a28ee50b97](https://github.com/user-attachments/assets/37adf731-161f-4e1a-8014-50caa87f29fd)


**RESULTS**

Thus the 4 bit synchronus up counter using verilog and it's functionality is calculated using the functional table is ecexuted successfully.
