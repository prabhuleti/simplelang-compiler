# simplelang-compiler
# SimpleLang 8-Bit Compiler

## Overview
This project is an **8-bit compiler** designed to compile code written in a simple high-level language (**SimpleLang**) into assembly instructions for an 8-bit CPU simulator. The compiler supports basic arithmetic operations, variable assignments, and conditional expressions.

The main components of the compiler are:
- A **Lexer** to tokenize the input source code.
- A **Parser** to generate an Abstract Syntax Tree (AST).
- A **Code Generator** to convert the AST into assembly code for an 8-bit CPU.
- A **Test Framework** to validate the functionality of the compiler using SimpleLang programs.

## Features
- Supports arithmetic operations: `+`, `-`, `*`, `/`
- Variable assignments and usage: `let x = 5;`
- Conditional statements: `if`, `else`
- Error reporting for invalid syntax and expressions

## File Structure

