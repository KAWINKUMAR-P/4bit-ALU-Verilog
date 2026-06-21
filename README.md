# 4-bit ALU — Verilog / Vivado

A 4-bit Arithmetic Logic Unit (ALU) implemented in Verilog, supporting 16 operations.

## Operations

| ALU_Sel | Operation |
|---------|-----------|
| 0000    | ADD       |
| 0001    | SUB       |
| 0010    | MUL       |
| 0011    | DIV       |
| 0100    | Shift Left  |
| 0101    | Shift Right |
| 0110    | Rotate Left |
| 0111    | Rotate Right |
| 1000    | AND       |
| 1001    | OR        |
| 1010    | XOR       |
| 1011    | NOR       |
| 1100    | NAND      |
| 1101    | XNOR      |
| 1110    | Greater Than |
| 1111    | Equal     |

## Files
- `src/alu.v` — ALU module
- `sim/tb_alu.v` — Testbench
- `constraints/alu.xdc` — FPGA pin constraints (Basys3/Artix-7)

## Simulation (Vivado)
1. Add `src/alu.v` and `sim/tb_alu.v` to your Vivado project
2. Set `tb_alu` as the simulation top module
3. Run Behavioral Simulation

## Notes
- XDC constraints target the **Basys3 board** (Artix-7 FPGA)
- For simulation only, the XDC file is not needed
