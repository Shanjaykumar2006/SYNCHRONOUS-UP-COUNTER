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

/* write all the steps invloved */

**PROGRAM**


![Screenshot 2025-05-06 093912](https://github.com/user-attachments/assets/f81d7d7c-9129-4ebc-9444-2aebdcf35702)

**RTL DIAGRAM**

![Screenshot 2025-05-06 094049](https://github.com/user-attachments/assets/229e4682-2bbd-4361-8431-ad47f2316c32)

**WAVEFORM**

![Screenshot 2025-05-06 094125](https://github.com/user-attachments/assets/410b956f-a1bd-4d0d-8cf3-bfb22b4aa8b6)

**TRUTH TABLE**

![Screenshot 2025-05-06 094144](https://github.com/user-attachments/assets/820830d3-af65-4e39-a979-1a703b3f7ac2)

**RESULTS**
 
 4 bit synchronous up counter was implemented successfully.
