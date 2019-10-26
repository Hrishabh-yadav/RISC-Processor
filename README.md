# RISC-Processor
This is a simulation of 4 out of 5 stages (except Fetch) in the RISC processor pipeline:
  1. Decode
  1. Execute
  1. Memory
  1. Write-Back

## Block Diagram

![Image of RISC Pipeline](https://github.com/Hrishabh-yadav/RISC-Processor/blob/master/risc.jpeg)

## Specifications

* 32-bit inpit instructions
* 32 registers in register file
* 32-bit data
* Operations possible: Addition, Subtraction, Comparison, OR, AND, NOR, LOAD(memory->register), STORE(register->memory), MOVE(register->register)

## Instructions

The syntax of any instruction(except STORE) is: ***operation destination source1 source2/immediate***
<br>
For STORE: **STORE *source destination offset***

<br>

![Image of RISC Instruction](https://github.com/Hrishabh-yadav/RISC-Processor/blob/master/InstructionsRISC.PNG)

<br>

Any instruction Y can be converted to YI(Y immediate) by changing the 5th bit from the left from 1 to 0. <br>
Example: SUBI = 000100 Ri Rj X
