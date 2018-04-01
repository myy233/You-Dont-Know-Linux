1.2 Memory
All hardware is just a big storage of 1s and 0s, indicating a logical gate to be ON or OFF.
Those 1s and 0s flow through the main memory.
Each 1 and 0 is called a bit.
It is kernel and process's job to manipulate these bits.
All hardware operates in bits to form various inputs and outputs.
CPU just rewrites these bits in the main memory which  is located in the RAM.
The CPU reads the instruction (its hardware instruction set) and data from the main memory, then writes out the data block back to the memory.
At this point, it very important to talk about state (which many sound familiar to most of you)
A state strictly speaking is a particular arrangement and combination of bits.
for example: 0110, 0001, 1001 represent 3 different form of states.
However, a single process can be describes by millions of bits
Reading a process is a daunting task. Therefore abstraction is used to simplify the description of a process state.

for example: process is waiting for input, process is paused/terminated.