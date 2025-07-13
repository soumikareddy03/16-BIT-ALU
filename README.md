# 🧮 16-bit ALU on FPGA

This project implements a **16-bit Arithmetic Logic Unit (ALU)** using **Verilog HDL**, designed and simulated on an FPGA platform. It performs a variety of arithmetic and logical operations based on a control signal and showcases the fundamentals of digital computation.

---

## 📌 What is an ALU?

An **Arithmetic Logic Unit (ALU)** is the core component of a CPU that performs all arithmetic and logical operations. In this project, the ALU operates on **16-bit binary numbers** and supports various essential operations like **Addition**, **Subtraction**, **Bitwise AND/OR/XOR**, **Shift**, and **NOT**.

---

## 🎯 Features

* **16-bit input operands**
* Supports **10+ operations**
* Status flags: **Zero**, **CarryOut**, **Overflow**
* Designed using **Verilog**
* Fully **synthesizable** and tested on **FPGA**

---

## ⚙️ Supported Operations

| ALU\_Sel | Operation   | Description        |     |
| -------- | ----------- | ------------------ | --- |
| `0000`   | ADD         | `A + B`            |     |
| `0001`   | SUB         | `A - B`            |     |
| `0010`   | AND         | `A & B`            |     |
| `0011`   | OR          | \`A                | B\` |
| `0100`   | XOR         | `A ^ B`            |     |
| `0101`   | NOT         | `~A`               |     |
| `0110`   | Shift Left  | `A << 1`           |     |
| `0111`   | Shift Right | `A >> 1`           |     |
| `1000`   | Increment   | `A + 1`            |     |
| `1001`   | Decrement   | `A - 1`            |     |
| ...      | Extendable  | Add more if needed |     |

---

## 🧠 Architecture

The ALU is composed of:

* A **combinational logic block** to perform selected operations
* **Status flag outputs**:

  * `Zero` – Result is zero
  * `CarryOut` – For addition/subtraction overflow
  * `Overflow` – Two's complement overflow detection

---

## 🧪 Simulation

* Simulated using **ModelSim** or **Vivado Simulator**
* Testbench included to verify all operations
* Results checked for accuracy and flag outputs

---

## 📁 File Structure

```
├── alu.v              # Core ALU module
├── alu_tb.v           # Testbench to verify ALU behavior
├── README.md          # Project documentation
```

---

## 🔧 How to Use

1. Clone this repository
2. Open in **Vivado** or any Verilog IDE
3. Add `alu.v` and `alu_tb.v`
4. Run simulation to verify output
5. Synthesize and implement on FPGA (optional)

---

## 🖥️ Tools & Requirements

* Language: **Verilog HDL**
* Simulator: **ModelSim / Vivado Simulator**
* FPGA Board: (Optional) **Basys 3 / Spartan-6 / Artix-7**
* Design Suite: **Xilinx Vivado / ISE**

---

## 🧩 Possible Extensions

* Add signed/unsigned operation support
* Interface with 7-segment displays
* UART or switch-based operand inputs
* Include multiplication and division



