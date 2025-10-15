# SMT Solver Testing Framework

This repository contains two complementary tools for testing and fuzzing SMT solvers:

## 🎯 Projects

### 1. TypeFuzz Prototype
A C++ implementation of type-directed fuzzing using the cvc5 API pattern. Generates random type-consistent SMT constraints and tests solver satisfiability.

**Key Features:**
- Type-directed expression generation (integers, booleans)
- Depth-controlled recursive generation
- Arithmetic and logical operation support
- Mock cvc5 API demonstrating real integration patterns

### 2. SMT Bug Hunter
A comprehensive framework for systematically discovering bugs in SMT solvers (cvc5, Z3, Yices, etc.).

**Test Categories:**
- Integer overflow scenarios
- Division edge cases  
- Deeply nested expressions
- Type system corner cases
- Memory stress testing

## 🚀 Quick Start

```bash
# Compile TypeFuzz
g++ -std=c++17 -o typefuzz tyfusi-prototype.cpp

# Compile Bug Hunter
g++ -std=c++11 -o bug-hunter smt-bug-hunter.cpp
