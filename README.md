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

```plaintext
📂 project-root
 ├── 📂 src/                      # Source code for the compiler
 │   ├── lexer.c                  # Lexer implementation: Tokenizes input source code
 │   ├── parser.c                 # Parser implementation: Builds the Abstract Syntax Tree (AST)
 │   ├── codegen.c                # Code generation: Converts AST into 8-bit CPU assembly
 │   ├── ast.h                    # Header file defining structures used for the AST
 │   ├── tokens.h                 # Token types and definitions
 │   ├── symtab.h                 # Symbol table management (variables, types)
 │   └── main.c                   # Main driver program to execute the compiler
 ├── 📂 include/                  # Header files and common definitions
 │   ├── simplelang.h             # General header with utility functions and definitions
 │   ├── lexer.h                  # Lexer function declarations
 │   ├── parser.h                 # Parser function declarations
 │   ├── codegen.h                # Code generation function declarations
 ├── 📂 tests/                    # Sample SimpleLang programs to test the compiler
 │   ├── test1.slang              # Example program using arithmetic operations
 │   ├── test2.slang              # Example program using conditionals
 │   └── test3.slang              # Example program testing variable assignments
 ├── 📂 docs/                     # Project documentation
 │   ├── simplelang_spec.md       # Detailed specification of the SimpleLang syntax and grammar
 │   └── design_notes.md          # Internal notes on design decisions and future improvements
 ├── 📂 build/                    # Build directory for object files and binaries
 ├── 📂 output/                   # Directory for generated assembly files
 ├── Makefile                     # Build automation using Make
 ├── README.md                    # This file
 ├── simplelang_spec.md           # SimpleLang language specification
 ├── cpu_simulator.c              # 8-bit CPU simulator to execute the generated assembly code
 └── LICENSE                      # Project license (MIT License)
