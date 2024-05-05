## Description

This is a program designed to trace system calls of a specified process on a Linux system. It utilizes the ptrace system call to attach to the target process, monitor its system calls, and log them to a file using a custom logger.


## Usage:

Compile the program:
```bash
g++ -o audit main.cc Logger.cc -O3
```
Run the program with root privileges, specifying the process ID to trace:
```bash
sudo ./audit <pid>
```
Replace <pid> with the process ID of the target process.
The program will attach to the specified process, trace its system calls, and log them to a file named audit_log_<pid>.txt.
