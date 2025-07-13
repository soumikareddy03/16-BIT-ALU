# 16-BIT-ALU
## 🟢 Project Overview
This project implements a **4-bit Arithmetic Logic Unit (ALU)** using Verilog HDL. The ALU supports 16 different operations, including arithmetic, logical, shift, rotate, and comparison operations.
It also includes a Verilog testbench to verify its functionality through simulation.

---

## ⚙️ Features
- **Arithmetic operations**: Addition, subtraction, multiplication, division
- **Logical operations**: AND, OR, XOR, NAND, NOR, XNOR
- **Shift operations**: Logical left shift, logical right shift
- **Rotate operations**: Left rotate, right rotate
- **Comparison operations**: Greater than, equality check

---

## 💡 ALU Inputs & Outputs
- **Inputs**:
  - `A`: 4-bit operand
  - `B`: 4-bit operand
  - `Sel`: 4-bit selector to choose the operation
- **Output**:
  - `out`: 7-bit result

---

## 🧪 Testbench
A dedicated testbench (`alu.v`) is included to simulate and verify all operations. The testbench sets different values of `Sel`, `A`, and `B`, and monitors the corresponding outputs.

---

## 🛠️ How to Run Simulation
1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/alu-verilog-project.git
    cd alu-verilog-project
    ```
2. **Compile and simulate using ModelSim or any Verilog simulator**:
    ```
    vlog alu.v 
    vsim work.TB
    ```
3. **View waveforms**:
    - Use `add wave *` and run the simulation in GUI mode.
    - Analyze the waveforms to verify different operations.

---



