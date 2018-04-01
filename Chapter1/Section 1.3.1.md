*1.3.1 Process Management*
process management describes the methodology of initiation, pausing & resuming and the termination of processes
On many modern systems, processes appears to run at the same time. However, it is NOT the case.
Let's take a 1 core CPU system.
many process can use it but there can only be one process running at a time.
each process use the CPU for a fraction of a sec
it is then switched to another process
the act for one process to give up the control of the CPU to another process is call _Context Switch_
the time it takes for a process to perform significant calculation (or make significant progress) on a process is call _Time Slice_
the slices are so small that the system appears to be doing multiple tasks at the same time. (multitasking)
Here is an example of how a context switch is done
1. CPU interrupts the current process with an internel timer. enters kernel mode and give kernel control of the system.
2. Kernel records the state of the CPU and the RAM upon gaining control of the system
3. kernel prepares a new time slice by performing some preliminary actions like collect data from input/output
4. Time slice is set up, Kernel analyzes the list of process in queue and chose one based on priority

5. Kernel prepares RAM and CPU
6. Kernel nstruct the duration of the time slice to the CPU.
7. Kernel switch CPU to user mode and gave control back to the CPU.