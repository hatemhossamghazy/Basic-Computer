# Basic-Computer
# Basic Computer (M. Morris Mano) - Verilog Implementation
# Project Overview
- What is the Mano Basic Computer?
The Mano Basic Computer is a simplified educational model of a computer, designed by M. Morris Mano in his book “Computer System Architecture”.
It's made to teach how a basic computer works at the hardware level — step by step.
- Main Idea:
it shows how a computer:
Stores instructions
Processes data
Executes commands
All using very simple components — perfect for learning how real computers work inside.
# Architecture Features
* 16-bit Word Length

* 12-bit Address Bus (4K words of memory) // this is in mano's basic computer specifications, but in the verilog code for simplicity of the simulation we scaled the size of registers

* internal Registers: AC, DR, IR, TR, AR, PC, INPR, OUTR

* Memory: 4096x16-bit, initialized from external file

* ALU Operations: AND, ADD, LDA, CLA, etc.

* sequence counter: Implements micro-operations T0–T15 // the maximum size for instruction is 15 but this also in mano's specifications and we scale this and reduce it for simplicity

### Instruction Set:

+ Memory-Reference Instructions (AND, ADD, LDA, STA, BUN, etc.)
+ Register-Reference Instructions (CLA, INC, HLT, etc.)
+ I/O Instructions (INP, OUT)
+ I/O regs: 8-bit INPR and OUTR

* it also based on a cructial concept which is the timing and control structure which means that each microoperation has it is corresponding execuation
* The link of video : https://drive.google.com/file/d/1fRkIO8felcxEaqPWjACFy9cQKGDL5XA_/view
