# Binary to Gray Code Converter – Verilog

A parameterized **Binary-to-Gray Code Converter** designed using Verilog HDL. The design converts an N-bit binary input into its corresponding Gray code using XOR logic, with a default width of 8 bits.

### Features
- Parameterized N-bit design
- Default data width: 8 bits
- Uses XOR logic for binary-to-Gray conversion
- Generate loop for scalable hardware implementation
- Testbench verifies all possible input combinations
- Expected Gray-code values are generated in the testbench
- Error counter included for verification

### Files
- `bi.v` – Parameterized Binary-to-Gray Code Converter
- `tb.v` – Testbench for functional verification

### Conversion Logic
For an N-bit binary input:

```text
Gray[N-1] = Binary[N-1]
Gray[i]   = Binary[i] XOR Binary[i+1]
```

### Tools
- Verilog HDL
- Xilinx Vivado

This project demonstrates **combinational RTL design, parameterization, generate constructs, and self-verification using a Verilog testbench**.
