+++
title = 'Quantra - A Superscalar CPU in Turing Complete'
date = 2024-12-21T13:18:15-05:00
draft = false
+++

---

Quantra is a CPU that I built in the logic simulator [Turing Complete](https://turingcomplete.game).
<br/>
<image src="content/images/quantra.png" title="Quantra CPU" width="auto">

# Features:
- 32-bit instruction width
- 16-bit data width
- 16 GPRs (General Purpose Registers) with 4 write ports and 8 read ports
- Four 3-stage pipelines capable of executing instructions in parallel
- Approximately 65KB of RAM (Random Access Memory)
- Approximately 65KB of persistent SSD (Solid State Drive) storage
- The ability to load binary data from a file on my computer
- The ability to execute instructions from memory
- An ALU (Arithmetic & Logic Unit) capable of performing 10 different calculations
	- AND
	- NAND (Not AND)
	- OR
	- NOR (Not OR)
	- XOR (eXclusive OR)
	- Addition
	- Subtraction
	- Logical Shift Left (LSL)
	- Logical Shift Right (LSR)
	- Compare (Compares two numbers and stores to the flags register)
- An 80x24 character console screen capable of displaying 8-bit ASCII characters
- An 160x120 pixel screen
- A keyboard input to read keystrokes from my physical keyboard
- A time component capable of reading 64-bit UNIX time in four 16-bit segments