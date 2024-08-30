# RISC-MIPS32-Microprocessor
This repository includes the implementation of a 5-stage pipelined RISC (Reduced Instruction Set Computer) processor based on the MIPS32 architecture. The pipelined design allows for the simultaneous execution of multiple instructions, significantly enhancing throughput compared to a single-cycle processor.

Table of Contents
Introduction
Features
Architecture
Pipeline Stages
Instruction Set
Installation
Usage
Testing
Contributing
License
Introduction
MIPS32 is a widely studied RISC architecture in computer architecture courses. This project implements a 5-stage pipelined processor following the MIPS32 instruction set, enhancing CPU throughput by allowing multiple instructions to be processed simultaneously across different stages.

Features
5-Stage Pipeline: Comprises Instruction Fetch (IF), Decode (ID), Execute (EX), Memory Access (MEM), and Write-back (WB).
Hazard Detection: Techniques to manage data, control, and structural hazards.
Data Forwarding: Resolves data hazards to maintain pipeline efficiency.
Branch Prediction: A basic mechanism to minimize control hazard penalties.
MIPS32 Instruction Support: Supports a subset of the MIPS32 instruction set.
Architecture
The processor's architecture is based on a 5-stage pipeline, with each stage handling a specific part of instruction processing:

Instruction Fetch (IF): Retrieves instructions from memory using the Program Counter (PC).
Instruction Decode (ID): Decodes instructions and reads operands from the register file; performs sign extension if needed.
Execute (EX): Performs ALU operations and computes memory addresses for access instructions.
Memory Access (MEM): Manages data memory operations for load and store instructions.
Write-back (WB): Writes results back to the destination register in the register file.
