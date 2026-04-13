# Multi-Container Runtime in C

## Project Description
This project implements a lightweight Linux container runtime in C. It uses low-level system calls such as `clone()`, `chroot()`, and `mount()` to create isolated environments similar to containers.

Each container runs as a separate process with its own filesystem, process space, and hostname. The runtime also supports basic logging and execution of workloads inside the container.

---

## Features

- Process isolation using Linux namespaces (PID, UTS, Mount)
- Filesystem isolation using `chroot`
- Container creation using `clone()` system call
- Execution of commands inside containers
- Log handling using pipes
- Support for multiple containers

---

## Technologies Used

- C Programming
- Linux System Calls (`clone`, `chroot`, `mount`)
- Ubuntu Virtual Machine
- GCC Compiler

---

##  Setup Instructions

```bash
git clone https://github.com/Shreya-rd25/OS-Jackfruit.git
cd OS-Jackfruit/boilerplate
make

---

## Output

The container runtime was successfully tested. Below is a sample execution:


Container started with PID: 20838
ls
bin dev etc home ...
echo hello
hello
exit
Container stopped
