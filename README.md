<p align="center">
  <img src="https://img.shields.io/badge/Built%20With-Python-blue?style=for-the-badge" alt="Python Badge"/>
  <img src="https://img.shields.io/badge/Target-C%20Code-green?style=for-the-badge" alt="C Code Badge"/>
</p>

# 🧠 Mini NLP-to-C Compiler

> Convert simple natural language programming instructions into **valid C code** — all in one Python-powered compiler pipeline.

---

## 🚀 Overview

This project is a **mini-compiler** built in Python that:
- Accepts a **Natural Language Programming (NLP-style)** input.
- Translates it into **valid, executable C code**.
- Follows the complete compiler pipeline:
  1. **Lexical Analysis** (via PLY)
  2. **Parsing** (CFG-based)
  3. **Semantic Analysis**
  4. **IR Generation**
  5. **Optimization**
  6. **C Code Generation**
  7. **Execution**

---

## 📁 Project Structure

```
mini-compiler/
├── lexer.py               # Lexical analyzer using PLY
├── parser.py              # Grammar rules and AST definitions
├── semantic.py            # Semantic analyzer to validate logic
├── ir_generator.py        # Converts AST to Intermediate Representation
├── optimizer.py           # Optimizes the IR
├── codegen.py             # Generates final C code
├── executor.py            # Compiles and runs C code
├── targetcode_runner.py   # Ties all components together
```

---

## 🧩 Sample Input

```text
Declare integer x
Set x to 5
Print x
```

🔁 **Becomes:**

```c
#include <stdio.h>

int main() {
    int x;
    x = 5;
    printf("%d\n", x);
    return 0;
}
```
---

## 🧠 Technologies Used

- Python 3
- [PLY (Python Lex-Yacc)](http://www.dabeaz.com/ply/)

---

<p align="center"><b>Transform your thoughts into C code — the compiler understands you!</b></p>
