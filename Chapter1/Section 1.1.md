Abstraction splits the entire system into smaller pieces which makes the user easier to understand. These smaller parts are organized into different levels.
A level dictates how close that part of the system is to the system hardware itself.
-- top level consists: games, web browser.

-- low level consists: memory, CPU, HDD
At this point, I will have to introduce an important software called KERNEL.
Kernel manages and interact directly with the hardware.
-- it can tell the CPU what to do.
-- it can also act as an interface between top level apps with the hardware.
Kernel also manages MOST of the programs at the higher levels. (ie, games, web servers)
The domain which the higher level programs occupies within a system is called user space.
Here is a simple hierarchy of the different levels of the system.
High level: GUI, Servers, Shell
Kernel: system calls, process management, RAM, device drivers
Hardware (lowest level): CPU, HDD, ODD
All processes are ran in two modes: Kernel  mode and user mode.
as the name suggests, kernel run in kernal mode.
it has full control on the CPU and RAM.
The domain which kernel operates in is called kernel space.
It is very easy to cause system crashes if errors occur in this mode. As kernel processes can affect other processes from running properly because of total control over the hardwares.
User mode on the other end only owns a portion of the RAM and other hardware.
User process only owns that part of the hardware, meaning it can NOT access other part of the hardware nor can other user process can view your process.
IF there is a process crash, it is easily cleaned up.  and the crashes area does not affect other user processes.
NOTE: IT IS POSSIBLE FOR A USER PROCESS TO CRASH THE WHOLE SYSTEM.
IF THE PROCESS HAS ENOUGH PERMISSION.