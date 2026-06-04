# C-to-Asm

This repository contains writeups documenting my analysis of self-written C/C++ programs.

## Each project includes:

The original C/C++ source code.
Static analysis performed using Ghidra.
Dynamic analysis and debugging using x64dbg and WinDbg.
Notes on program behavior, compiler optimizations, assembly output, memory inspection, breakpoints.
and reverse engineering observations.

## The purpose of this repository is to improve my understanding of:

Reverse engineering.
Low-level program execution.
Windows debugging.
Decompiled code analysis.
Compiler-generated assembly.
Binary internals and runtime behavior.

## I have writeups divided as follow :

[Optimized code](./O2-Ob2-Release/)
Code written in this section was debugged using `Release` Build mode with `O2 optimization` and `Inline function expansion` set to `OB2` to make it harder to understand the decompiled C and assembly instructions.

[Unoptimized code](./Od-Ob0-Debug/)
Code written in this section was debugged using `Debug` build mode with optimizations and Inline function expansion turned off which makes its easier to understand the decompiled C and assembly instructions.
