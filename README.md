# SimpleLang 8-Bit Compiler

## Overview
This project is an **8-bit compiler** designed to compile code written in a simple high-level language (**SimpleLang**) into assembly instructions for an 8-bit CPU simulator. The compiler supports basic arithmetic operations, variable assignments, and conditional expressions.

The main components of the compiler are:
- A **Lexer** to tokenize the input source code.
- A **Parser** to generate an Abstract Syntax Tree (AST).
- A **Code Generator** to convert the AST into assembly code for an 8-bit CPU.
- A **Test Framework** to validate the functionality of the compiler using SimpleLang programs.

The project serves educational purposes and can be extended with additional features or optimizations.

## Features
- **Arithmetic operations**: Supports addition (`+`), subtraction (`-`), multiplication (`*`), and division (`/`).
- **Variable assignment**: Simple assignment and usage: `let x = 10;`.
- **Conditional statements**: Supports `if` and `else`.
- **Error handling**: Basic error reporting for syntax and expression errors.
- **Modular structure**: Easy to extend with more language features or optimization techniques.

## File Structure

📂 project-root
 ├── 📂 src/                      # Source files for the compiler
 │   ├── lexer.cpp                # Tokenizes the input source code
 │   ├── parser.cpp               # Parses the tokens into an AST
 │   ├── parser.h                 # Header file for the parser functions and AST structures
 │   ├── main.cpp                 # Main driver program to execute the compiler
 ├── 📂 include/                  # Common definitions and headers
 │   └── compiler.h               # Compiler-related definitions, constants, and utility functions
 ├── 📂 input/                    # Input source files
 │   └── input.txt                # Example SimpleLang source code for testing the compiler
 ├── Makefile                     # Build automation using Make
 ├── README.md                    # This file
 └── LICENSE                      # License file for the project (MIT License)
