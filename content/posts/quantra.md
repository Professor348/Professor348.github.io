+++
title = 'Quantra - A Superscalar CPU in Turing Complete'
date = 2024-12-21T13:18:15-05:00
draft = false
+++

---

Quantra is a CPU that I built in the logic simulator [Turing Complete](https://turingcomplete.game).
It is based on the Allegro architecture that the campaign teaches you, but is heavily modified from this baseline.
<br/>

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

# Layout:
![Quantra 16-bit CPU](/posts/quantra.png)
1. Assembly component (this is the in-game code editor)
2. Program counter
3. Hazard detection circuit
4. Console screen
5. Pixel screen
6. Keyboard component
7. Instruction decoding
8. Register file
9. ALUs (One per pipeline)
10. Execution control circuit (controls executing from RAM/Assembly component)
11. Condition circuit
12. RAM
13. Miscallaneous I/O devices
14. SSD
15. File loader