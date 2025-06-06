# ⚙️ 32-bit RISC-V Processor – Verilog HDL Implementation  
A single-cycle RISC-V processor core designed and simulated using Verilog and ModelSim.

---

## 🧠 Overview

This repository contains the **Verilog HDL implementation of a 32-bit single-cycle RISC-V processor**, developed from scratch based on the **RISC-V Instruction Set Architecture (RV32I)**. The processor is designed to perform fundamental arithmetic, logical, control flow, and memory operations in a single clock cycle per instruction.

The design is built and simulated using **ModelSim** and is intended as an educational tool for learning computer architecture and hardware design using Verilog.

---

## 🚀 Features

- ✅ **32-bit Single-Cycle Architecture**
- 📦 Supports a basic subset of **RISC-V RV32I instructions**
- 🧠 Implements key datapath components: **ALU, Register File, Control Unit, Memory**
- 🧪 Functional verification using **ModelSim testbenches**
- 🔧 Modular design for ease of readability and extension
- 💻 Synthesizable and can be mapped to FPGAs for prototyping

---

## 🔧 Key Components

- **ALU.v** – Performs arithmetic and logical operations  
- **Control.v** – Generates control signals based on instruction opcode  
- **Instrc_read.v** – Instruction memory block  
- **regfile.v** – 32-register file with synchronous write  
- **datacache.v** – Data memory (RAM) module  
- **Processor.v** – Top-level module connecting datapath components  
- **nextInstrc.v** – Calculates PC update logic  
- **testbench.v** – Test environment for simulation and instruction execution validation

---

## 🛠 Tools Used

| Tool             | Purpose                              |
|------------------|--------------------------------------|
| **Verilog HDL**  | RTL design of the processor          |
| **ModelSim**     | Simulation and waveform debugging    |
| **Quartus**      | Optional synthesis and FPGA mapping  |

---

## 🧪 Instruction Support (Subset)

| Category        | Instructions                          |
|-----------------|----------------------------------------|
| Arithmetic      | `ADD`, `SUB`, `AND`, `OR`, `XOR`, `SLL`, `SRL`, `SRA`  
| Immediate       | `ADDI`, `ANDI`, `ORI`  
| Load/Store      | `LW`, `SW`  
| Control Flow    | `BEQ`, `BNE`, `JAL`, `JALR`  

---
