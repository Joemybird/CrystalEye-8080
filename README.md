# CrystalEye-8080

A see-through recreation of the Intel 8080 using digital logic

![Current state of the CPU wiring](Current%20CPU.png)

# Description

CrystalEye-8080 is a project with the goal of re-creating an 8-bit 
CPU using nothing but raw logic. Every component of the CPU can be 
broken down into further components. ALUs turn into collections of 
adders, shifters, and XOR gates, and those components also break 
down into more simplier peices.

In total, all components of the CPU are built down to 4 elemental 
logic units.

One of the goals of this project is to provide an easy and simple 
way to let people easily 'look inside' the workings of a CPU and 
see how every single piece of their device can be broken down into 
simplier logic.

Elemental logic components:
- AND gates
- OR gates
- NOT gates
- Buffers

# Usage

All .circ files found in this project are designed to be opened via 
Logisim Evolved

A download of Logisim Evolved can be found here: 
https://github.com/logisim-evolution/

# Unfinished

Project is currently still uncomplete. However, all 
components other than the Instruction Encoder and
the Timing and Control circuit should be functional