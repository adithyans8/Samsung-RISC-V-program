# RV32I Verilog Simulation Project Summary

## Overview
This project involves the simulation and analysis of a simplified RV32I processor design using Verilog. The design was tested using Icarus Verilog and the results were visualized using GTKWave.

## Objectives
1. To develop and simulate a Verilog-based implementation of the RV32I processor.
2. To verify the functionality of the processor through a testbench.
3. To analyze signal behavior over time using waveform visualization.

## Tools Used
- *Icarus Verilog*: For compiling and simulating the Verilog design and testbench.
- *GTKWave*: For viewing waveform outputs.
- *Ubuntu Linux*: Development and testing environment.

## Key Components
1. *RV32I Processor*:
   - Implements a simplified version of the RISC-V 32-bit Instruction Set Architecture.
   - Includes pipeline stages for instruction fetch (IF), decode (ID), execute (EX), memory access (MEM), and write-back (WB).
2. *Testbench*:
   - Validates processor functionality by applying test inputs and observing outputs.
   - Includes $dumpfile and $dumpvars directives to generate waveform data.
3. *Waveform Analysis*:
   - Output signals include control, data, and clock signals.
   - Observed using GTKWave to verify correctness and debug issues.



## Workflow
1. *Design and Implementation*:
   - The RV32I processor design was implemented in Verilog in wave_rv32i.v.
   - The testbench for the design was written in wave_rv32i_tb.v.
2. *Compilation*:
   ```bash
   iverilog -o wave_rv32i wave_rv32i.v wave_rv32i_tb.v
