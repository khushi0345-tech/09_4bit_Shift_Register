# 4-bit Shift Register using Verilog HDL

## 📖 Overview

This project implements a **4-bit Serial-In Shift Register** using **Verilog HDL**. The register shifts data by one position on every positive edge of the clock while accepting a new serial input bit. An asynchronous active-high reset initializes the register to zero. The design is implemented using synthesizable RTL and verified through simulation using a dedicated Verilog testbench.

---

## ✨ Features

- Verilog HDL implementation
- Synthesizable RTL design
- Positive edge-triggered operation
- Serial-In shift operation
- Asynchronous active-high reset
- Dedicated Verilog testbench
- Functional verification through simulation

---

## 📂 Project Structure

```
09_4bit_Shift_Register

├── shift_register.v
├── shift_register_tb.v
├── shift_register_waveform.png
└── README.md
```

---

## ⚙️ Inputs and Outputs

### Inputs

| Signal | Width | Description |
|--------|------|-------------|
| clk | 1 bit | Clock input |
| reset | 1 bit | Asynchronous active-high reset |
| serial_in | 1 bit | Serial input data |

### Outputs

| Signal | Width | Description |
|--------|------|-------------|
| q | 4 bits | Shift register output |

---

## 📊 Functional Description

The shift register stores 4 bits of data and shifts all bits one position to the left on every rising edge of the clock. The new serial input bit is inserted into the least significant bit (LSB). When the reset signal is asserted, the register is cleared to `0000`.

---

## 🧪 Simulation

The testbench verifies the shift operation by applying a sequence of serial input bits while generating clock pulses. The simulation waveform confirms correct shifting of data and proper reset functionality.

Simulation waveform:

**shift_register_waveform.png**

---

## 🛠️ Tools Used

- Verilog HDL
- Xilinx Vivado Simulator

---

## 📚 Concepts Used

- RTL Design
- Sequential Logic
- Shift Register
- Flip-Flops
- Testbench Development

---

## 🚀 Future Improvements

- Add parallel load capability
- Support left and right shifting
- Parameterize register width
- Add shift enable control

---

## 👩‍💻 Author

Khushi Garg
