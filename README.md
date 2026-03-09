# LinuxInternals
This repository tracks my study of UNIX internals, the C programming language, and the underlying computing model used by C and Linux to aid in my security research.

As an infosec analyst and computer engineering student, having a precise mental model of the systems I am securing (or exploiting) is mandatory.

The goal here is to focus strictly on the fundamentals. Just C and the Linux kernel, to build a proper understanding of memory, processes, and networking at the lowest software level. The end goal is to become a solid "computer understander" before eventually migrating to Rust for future low-level systems programming.

## Repository Structure
The work is split into three main fronts, aligning with my current university semester and personal studies:


### 1. C Fundamentals C/

#### 1. K.N. King Exercises (`/kn_king`)
Solutions and notes from reading "C Programming: A Modern Approach".

#### 2. Data Structures (`/data_structures`)
Implementations of core data structures and algorithms in C, developed alongside my university classes. The focus is on manual memory management and understanding how these abstract structures map to the core OS concepts, such as heap/stack memory, etc.

### 3. UNIX Systems Projects (`/projects`)
A series of standalone UNIX projects designed to interact directly with the Linux kernel. For now that list is composed of:
 Focuses on pointer arithmetic, memory alignment, and raw kernel memory requests.
* **Custom Shell:** A minimal UNIX shell to internalize process management (`fork`, `execvp`, `wait`) and I/O redirection.
* **Multithreaded HTTP Server:** A web server built from scratch using POSIX sockets and pthreads, expanding on previous IPC/UDS experience to handle TCP networking and concurrency.
* **Packet Sniffer:** A network sniffer using raw sockets. Focuses on reading raw byte arrays from the network interface, struct casting, endianness, and parsing OSI layer headers.

### 4. Reverse Engineering Projects (`/Reversing`) 
A series of projects focusing on reverse engineering many kinds of programs and hardware devices, especially malware or infected devices, focusing on utilizing static and dynamic techniques.


## Build
Each project directory contains its own instructions or Makefile. Development is done natively on a Linux environment using standard Clang toolchains and debugging tools like GDB and Valgrind.
