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
