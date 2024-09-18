# shellcode injection by C++
This repo is created for sharing experience of shellcode injection techniques with the community.

If you do use any of the code in these repositories **keep it legal!**

The Windows environment is addressed since most maldev tools and techniques are designed to target Windows OS.

## Processes

At its core, a process can be defined as an instance of a program that is being executed. When you start a program in Windows, the operating system allocates resources such as memory, CPU time, and I/O devices to execute that program. This allocation is done by creating a process for the program. 

1. User Processes: These are initiated by users and typically include applications such as web browsers, word processors, and media players.

2. System Processes: System processes, also known as kernel processes, are initiated and managed by the Windows kernel.

3. Service Processes: Services are background processes that run without user intervention, providing various system functionalities such as network communication, printing, and system monitoring.

4. Child Processes: A process can create additional processes known as child processes. These processes inherit certain attributes from their parent process and can perform tasks independently. 

## Threads

A thread can be defined as the smallest unit of execution within a process. Unlike processes, which are independent entities with their own memory space, threads exist within processes and share the same memory space. Each thread within a process has its own program counter, stack, and execution state, but they can access shared data and resources within the process.

Threads can execute independently or cooperatively, depending on the programming paradigm and **synchronization** mechanisms employed. 