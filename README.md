# System Programming in C++

This repository contains hands-on implementations of core **system programming concepts** using **C++**.  
It is designed to demonstrate a practical understanding of operating system internals, inter-process communication (IPC), process management, and synchronization mechanisms on Unix/Linux systems.

The focus is on **how things work under the hood**, not just on producing output.

---

## 🧠 Key Concepts Covered

- Process creation and execution (`fork`, `exec`)
- Inter-process communication (Pipes, FIFOs)
- Synchronization problems (Producer–Consumer, Reader–Writer)
- File system and low-level file handling
- Shell internals and command execution
- Performance-conscious, low-level C++ programming

---

## 🛠️ Technology Stack

- **Language:** C++
- **Platform:** Linux / Unix-based systems
- **Standards & APIs:** POSIX system calls

---

## 📁 Project Structure

### 1. Shell Implementation
A basic Unix-like shell that:
- Accepts user commands
- Spawns child processes using `fork()`
- Executes commands using the `exec()` family
- Demonstrates process lifecycle and command execution flow

**Concepts:** process management, system calls, command parsing

---

### 2. Pipe Implementation
Implementation of unnamed pipes:
- Enables communication between parent and child processes
- Demonstrates unidirectional data flow
- Manages file descriptors correctly

**Concepts:** IPC, pipes, file descriptor handling

---

### 3. Named Pipe (FIFO) Implementation
Implements communication between unrelated processes:
- Creates and uses named pipes (FIFOs)
- Demonstrates blocking behavior and synchronization
- Useful for producer–consumer style communication

**Concepts:** FIFO, IPC across independent processes

---

### 4. Producer–Consumer Problem
Classic synchronization problem implementation:
- Manages shared resources safely
- Demonstrates race conditions and coordination logic

**Concepts:** shared variables, synchronization fundamentals

---

### 5. Reader–Writer Problem
Implementation of the reader–writer synchronization problem:
- Allows concurrent readers
- Ensures exclusive access for writers
- Focuses on correctness and access control

**Concepts:** concurrency, synchronization strategies

---

### 6. File Entry Finder
Utility for file inspection and analysis:
- Reads file metadata
- Demonstrates low-level file system operations

**Concepts:** file handling, OS-level file APIs

---

## 🚀 How to Compile and Run

Use `g++` to compile individual programs:

```bash
g++ filename.cpp -o output
./output
