# 🧪 Digital Logic Design using Logisim – Lab Activities

This repository contains the implementation and verification of basic and intermediate digital circuits using **Logisim** as part of the Computer Organization & Architecture / Digital Logic laboratory.

---

## 🧩 Software Used

- **Logisim / Logisim-evolution**
- Platform: Windows  
- Simulation mode with gate delay enabled (for delay analysis experiment)

---

# ✅ Experiment – 1 : Half Adder


::contentReference[oaicite:0]{index=0}


### 🎯 Aim
To design and simulate a Half Adder using Logisim.

### 📘 Theory
A Half Adder is a combinational logic circuit that adds two single-bit binary numbers. It produces two outputs:
- **Sum (S)**
- **Carry (C)**

The Sum is obtained using XOR operation and Carry is obtained using AND operation.

### 📋 Truth Table

| A | B | Sum | Carry |
|---|---|-----|-------|
| 0 | 0 |  0  |   0   |
| 0 | 1 |  1  |   0   |
| 1 | 0 |  1  |   0   |
| 1 | 1 |  0  |   1   |

### 🧪 Procedure
1. Open Logisim and create a new project.
2. Place two input pins A and B.
3. Place one XOR gate for Sum and one AND gate for Carry.
4. Connect inputs to both gates.
5. Connect the outputs to output pins.
6. Simulate by changing the input values.

### 🧾 Conclusion
We have successfully designed and simulated a Half Adder using Logisim and verified its functionality using the truth table.

---

# ✅ Experiment – 2 : Full Adder


::contentReference[oaicite:1]{index=1}


### 🎯 Aim
To design and simulate a Full Adder using Logisim.

### 📘 Theory
A Full Adder adds three one-bit inputs:
- A
- B
- Carry-in (Cin)

It produces:
- Sum
- Carry-out (Cout)

It can be constructed using two Half Adders and one OR gate.

### 📋 Truth Table

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
| 0 | 0 |  0  |  0  |  0   |
| 0 | 0 |  1  |  1  |  0   |
| 0 | 1 |  0  |  1  |  0   |
| 0 | 1 |  1  |  0  |  1   |
| 1 | 0 |  0  |  1  |  0   |
| 1 | 0 |  1  |  0  |  1   |
| 1 | 1 |  0  |  0  |  1   |
| 1 | 1 |  1  |  1  |  1   |

### 🧪 Procedure
1. Place three input pins (A, B, Cin).
2. Construct two Half Adders using XOR and AND gates.
3. Connect the carry outputs through an OR gate.
4. Observe Sum and Cout at output pins.

### 🧾 Conclusion
We have successfully designed and verified the operation of a Full Adder using Logisim.

---

# ✅ Experiment – 3 : 8 : 1 Multiplexer


::contentReference[oaicite:2]{index=2}


### 🎯 Aim
To design and simulate an 8:1 Multiplexer using Logisim.

### 📘 Theory
An 8:1 multiplexer selects one of eight input lines and forwards it to the output based on three select lines.

Inputs: D0 – D7  
Select lines: S2, S1, S0

### 📋 Truth Table

| S2 | S1 | S0 | Output |
|----|----|----|--------|
| 0  | 0  | 0  | D0     |
| 0  | 0  | 1  | D1     |
| 0  | 1  | 0  | D2     |
| 0  | 1  | 1  | D3     |
| 1  | 0  | 0  | D4     |
| 1  | 0  | 1  | D5     |
| 1  | 1  | 0  | D6     |
| 1  | 1  | 1  | D7     |

### 🧪 Procedure
1. Place eight data input pins and three select pins.
2. Use the built-in multiplexer or construct using logic gates.
3. Connect all inputs and select lines properly.
4. Observe the output for different select combinations.

### 🧾 Conclusion
We have successfully implemented and verified the working of an 8:1 multiplexer using Logisim.

---

# ✅ Experiment – 4 : 8 : 3 Encoder


::contentReference[oaicite:3]{index=3}


### 🎯 Aim
To design and simulate an 8:3 encoder using Logisim.

### 📘 Theory
An 8:3 encoder converts one active input out of eight into a 3-bit binary code.

Only one input should be active at a time.

### 📋 Truth Table

| Active Input | Y2 | Y1 | Y0 |
|--------------|----|----|----|
| D0           | 0  | 0  | 0  |
| D1           | 0  | 0  | 1  |
| D2           | 0  | 1  | 0  |
| D3           | 0  | 1  | 1  |
| D4           | 1  | 0  | 0  |
| D5           | 1  | 0  | 1  |
| D6           | 1  | 1  | 0  |
| D7           | 1  | 1  | 1  |

### 🧪 Procedure
1. Place eight input pins and three output pins.
2. Implement the required logic using OR gates.
3. Apply only one high input at a time.
4. Verify the encoded output.

### 🧾 Conclusion
We have successfully designed and tested an 8:3 encoder using Logisim.

---

# ✅ Experiment – 5 : 4-bit Ripple Carry Adder


::contentReference[oaicite:4]{index=4}


### 🎯 Aim
To design and simulate a 4-bit Ripple Carry Adder using Logisim.

### 📘 Theory
A Ripple Carry Adder (RCA) is constructed by cascading multiple Full Adders.  
The carry output of each stage is connected to the carry input of the next stage.  
The carry propagates sequentially from the least significant bit to the most significant bit.

### 📋 Truth Table
The truth table of a 4-bit adder is very large.  
Hence, verification is done by testing multiple combinations of two 4-bit numbers and observing correct sum and carry outputs.

### 🧪 Procedure
1. Place four Full Adder blocks.
2. Connect the carry output of each stage to the carry input of the next stage.
3. Provide two 4-bit inputs A and B and an initial carry input.
4. Observe the 4-bit sum and final carry output.

### 🧾 Conclusion
We have successfully designed and simulated a 4-bit Ripple Carry Adder using Logisim and verified its correctness.

---

# ✅ Experiment – 6 : Delay in Ripple Carry Adder


::contentReference[oaicite:5]{index=5}


### 🎯 Aim
To observe and analyze the propagation delay in a 4-bit Ripple Carry Adder using Logisim.

### 📘 Theory
In a ripple carry adder, the carry signal must pass through every full adder stage before the final sum and carry are produced.  
This results in cumulative propagation delay, which increases linearly with the number of bits.

The total delay is approximately equal to the number of stages multiplied by the carry propagation delay of a single full adder.

### 📋 Truth Table
The logical functionality remains identical to the 4-bit Ripple Carry Adder.  
The experiment focuses on timing behavior rather than functional correctness.

### 🧪 Procedure
1. Use the previously designed 4-bit Ripple Carry Adder.
2. Enable gate delay in Logisim simulation settings.
3. Reduce the tick frequency to clearly observe signal transitions.
4. Change the input values and observe how the carry propagates through each full adder stage.
5. Monitor the time difference between input change and final output stabilization.

### 🧾 Conclusion
We have successfully observed the propagation delay in a Ripple Carry Adder using Logisim and analyzed the carry ripple effect across successive full adder stages.

---

## 📌 Summary

This repository demonstrates the design, simulation, and verification of basic combinational circuits and adders using Logisim, including functional and timing analysis.
