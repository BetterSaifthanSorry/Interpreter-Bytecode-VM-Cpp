# cpplox 

A C++ port of the tree-walk interpreter from Part I of Robert Nystrom's [*Crafting Interpreters*](https://craftinginterpreters.com/). 

This repository currently implements the language up to Control Flow. It successfully parses and evaluates scripts with lexical scoping, variable assignments, and loops, stopping just short of function declarations and calls.

## Current Features

* **Scanner/Lexer:** Converts raw Lox source code into recognized tokens.
* **Recursive Descent Parser:** Constructs an Abstract Syntax Tree (AST) with correct operator precedence and error synchronization.
* **Tree-Walk Evaluator:** Executes the generated AST directly.
* **Environment & Scoping:** Handles variable declarations (`var`), assignments, and lexical block scoping `{ ... }`.
* **Control Flow:** Supports `if`, `else`, `while`, `for`, and logical operators (`and`, `or`).

## Roadmap / Pending Implementation
* Functions, closures, and callables (Chapter 10)
* Static variable resolution and binding (Chapter 11)
* Classes, instances, and inheritance (Chapters 12 & 13)

## Building and Running

```bash
# Clone the repository
git clone [https://github.com/yourusername/cpplox.git](https://github.com/yourusername/cpplox.git)
cd cpplox

# Build the project (assuming standard make or CMake)
make 

# Start the interactive REPL
./cpplox

# Execute a Lox script
./cpplox path/to/script.lox
