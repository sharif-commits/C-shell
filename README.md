# Custom Shell (C)

A lightweight Unix-like custom shell built in C that supports command execution, job control, logging, and custom built-in utilities. Designed with modular architecture to demonstrate core operating system concepts and process management.

---

## Features

* **Command Execution**

  * Runs standard system commands
  * Supports foreground and background processes

* **Custom Built-in Commands**

  * `hop` → directory navigation (cd-like functionality)
  * `reveal` → display file or directory information
  * `log` → command history tracking
  * `ping` → utility command

* **Job Control**

  * Background & foreground job handling
  * Process tracking
  * Signal handling (Ctrl+C, Ctrl+Z)

* **Shell Prompt**

  * Dynamic and interactive prompt display

* **Parsing & Tokenization**

  * Custom tokenizer for breaking input
  * Parser for command validation and structure

* **Logging System**

  * Maintains command history
  * Cleanup handled on exit

---

##  Project Structure

```
Custom-Shell/
│
├── include/        # Header files
│   ├── executor.h
│   ├── parser.h
│   ├── tokenizer.h
│   ├── jobs.h
│   └── ...
│
├── src/            # Source files
│   ├── main.c
│   ├── executor.c
│   ├── parser.c
│   ├── tokenizer.c
│   ├── jobs.c
│   └── ...
│
├── Makefile        # Build configuration
└── README.md
```

---

##  Compilation

Ensure `gcc` is installed, then run:

```bash
make
```

---

##  Running the Shell

```bash
./shell
```

##  Workflow Overview

1. **Input Handling**
   Reads user input from terminal

2. **Tokenization**
   Breaks input into meaningful tokens

3. **Parsing**
   Validates syntax and command structure

4. **Execution**
   Executes built-in or system-level commands

5. **Job Management**
   Tracks and manages background processes

---

##  Key Concepts

* POSIX system calls (`fork`, `exec`, `wait`)
* Process and job control
* Signal handling
* Modular C programming
* Command parsing techniques

---
