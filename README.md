# SERIAL-IN-SERIAL-OUT-SHIFTREGISTER

**AIM:**

To implement  SISO Shift Register using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**SISO shift Register**

A Serial-In Serial-Out shift register is a sequential logic circuit that allows data to be shifted in and out one bit at a time in a serial manner. It consists of a cascade of flip-flops connected in series, forming a chain. The input data is applied to the first flip-flop in the chain, and as the clock pulses, the data propagates through the flip-flops, ultimately appearing at the output.

The logic circuit provided below demonstrates a serial-in serial-out (SISO) shift register. It comprises four D flip-flops that are interconnected in a sequential manner. These flip-flops operate synchronously with one another, as they all receive the same clock signal.

![image](https://github.com/naavaneetha/SERIAL-IN-SERIAL-OUT-SHIFTREGISTER/assets/154305477/e81c4072-37f9-46c6-8145-566764b74c3a)

Figure 01 4 Bit SISO Register

The synchronous nature of the flip-flops ensures that the shifting of data occurs in a coordinated manner. When the clock signal rises, the input data is sampled and stored in the first flip-flop. On subsequent clock pulses, the stored data propagates through the flip-flops, moving from one flip-flop to the next.
Each D flip-flop in the circuit has a Data (D) input, a Clock (CLK) input, and an output (Q). The D input represents the data to be loaded into the flip-flop, while the CLK input is connected to the common clock signal. The output (Q) of each flip-flop is connected to the D input of the next flip-flop, forming a cascade.

**Procedure**

/* write all the steps invloved */

TYPE THE CODE IN THE QUARTUS SOFTWARE
COMPILE AND RUN THE CODE
GENERATE THE RTL VIEWER
CREATE NODES FOR INPUT AND OUTPUT NODES TO GENERATE TIMING DIAGRAM
FOR DIFFERENT COMBINATIONS OF INPUT GENERATE THE TIMING DIAGRAM

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming.

<img width="265" height="239" alt="image" src="https://github.com/user-attachments/assets/1679fb9e-0838-4ab1-9d7f-2a8cf3b0c55a" />


Developed by:PARAVEZHAA M RegisterNumber:212225220070
*/
**TRUTH TABLE**
| Clock Pulse | sin | q3 q2 q1 q0 | sout |
| ----------- | --- | ----------- | ---- |
| Reset       | X   | 0000        | 0    |
| 1           | 1   | 0001        | 0    |
| 2           | 0   | 0010        | 0    |
| 3           | 1   | 0101        | 0    |
| 4           | 1   | 1011        | 1    |
| 5           | 0   | 0110        | 0    |

**RTL LOGIC FOR SISO Shift Register**
<img width="458" height="332" alt="image" src="https://github.com/user-attachments/assets/f5d40556-1307-430e-a62f-410cc846eee0" />

**TIMING DIGRAMS FOR SISO Shift Register**
<img width="1409" height="790" alt="image" src="https://github.com/user-attachments/assets/1a3c16c8-b62c-4fcb-acfe-4616c37ec0a2" />

**RESULTS**
