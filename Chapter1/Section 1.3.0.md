*1.3 Kernel*
the main job of the kernel is to split the RAM into smaller pieces of which can be used to allocated different kinds of user processes.
each subdivision of the memory must maintain a specific state
and each process MUST operate within that subdivision and keep its share inside that domain.
Kernel is in charge of 4 (but not limited to) general tasks within a system
1. process: kernel determines which process can use the CPU
2. Memory: kernel keep track of the memory as to what is shared between processes &the part of the memory which was designate to the process.
3. device drivers: kernel is the interface of the process and the hardware. Kernel is usually the one operating the hardware.
4. system call and support: process uses system calls to communicate with the kernel.