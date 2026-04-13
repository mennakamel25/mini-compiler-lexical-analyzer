# 🧠 Compiler & Lexical Analysis Project

## 📌 Overview

This project is a **Compiler Design & Lexical Analysis System** that combines **C (Lex/Flex)** and **Python** to demonstrate core concepts of compilers and text processing.

It focuses on:

* 🔍 Lexical analysis (tokenization)
* 🧩 Parsing basic structures
* ⚙️ Utility functions for compiler operations
* 🐍 Python integration for testing / visualization (e.g., Pygame)

---

## 👩‍💻 Author

**Menna Kamel**

---

## 🛠️ Technologies Used

* **C Language**
* **Lex / Flex** (for lexical analysis)
* **Python**
* **Pygame** (for optional visualization/testing)

---

## 📁 Project Structure

```id="c9z812"
Compiler_Project/
│
├── README.md
│
├── GLOBALS.H              # Global definitions and shared variables
├── SCAN.H                 # Scanner (lexer) header file
├── UTIL.H                 # Utility functions header
├── UTIL.C                 # Implementation of utility functions
│
├── lexical.l              # Lex/Flex source file (token rules)
├── lex.yy.c               # Generated C file from Lex
│
├── c-.txt                 # Sample input program for testing
├── lexical_latest.zip     # Backup / archived version of lexer
│
├── project.py             # Python script for processing or integration
├── testpygame.py          # Python visualization/testing using Pygame
```

---

## 🧩 Components Description

### 🔍 Lexical Analyzer

* Defined in `lexical.l`
* Converts source code into tokens
* Uses **Flex (Lex)** to generate `lex.yy.c`

### ⚙️ Core C Modules

* `GLOBALS.H` → Global variables and definitions
* `SCAN.H` → Scanner interface
* `UTIL.H / UTIL.C` → Helper functions for processing

### 🧪 Input File

* `c-.txt` → Sample source code used for testing the lexer

### 🐍 Python Integration

* `project.py` → إضافات أو معالجة إضافية
* `testpygame.py` → Visualization or testing using Pygame

---

## ▶️ How to Run

### 1️⃣ Generate Lexer (if needed)

```bash id="cmd101"
flex lexical.l
```

### 2️⃣ Compile C Code

```bash id="cmd102"
gcc lex.yy.c util.c -o lexer
```

### 3️⃣ Run the Program

```bash id="cmd103"
./lexer < c-.txt
```

---

## 🧪 Python Execution (Optional)

```bash id="cmd104"
python project.py
```

or

```bash id="cmd105"
python testpygame.py
```

---

## 🎯 Features

* Tokenizes input source code
* Demonstrates compiler front-end basics
* Modular C design using headers and utilities
* Integration with Python for extended functionality

---

## ⚠️ Notes

* `lex.yy.c` is auto-generated → do not edit manually
* Ensure **Flex** and **GCC** are installed
* File names are case-sensitive on Linux

---

## 🚀 Future Improvements

* Add syntax analysis (Parser)
* Build Abstract Syntax Tree (AST)
* Add semantic analysis
* Improve error handling
* Create full compiler pipeline

---

## 🤝 Contributions

This is a personal educational project. Suggestions and improvements are welcome.

---

## 📄 License

This project is for educational purposes and can be modified freely.
