# SIC-Assembler
## What is an Assembler?
An assembler is a type of computer program that translates assembly language, which is a low-level human-readable representation of machine code instructions, into binary machine code that can be executed by a computer. The output of an assembler is called an object file. The assembly language serves as an intermediate step, allowing programmers to write code that's more understandable than raw binary code but is much closer to machine language than high-level languages like Python or Java.

## Two-Pass Assembler
A two-pass assembler goes through the assembly code twice:

### First Pass:
Read the entire source program.
Construct the symbol table that will store all literals and their values.
Determine the memory addresses of the program symbols.
### Second Pass:
Read the source program again.
Translate the assembly instructions into machine code using the symbol table constructed in the first pass.
Generate the object code by replacing symbols with their corresponding memory values.
The two-pass method ensures that the assembler has all the information it needs to correctly translate symbols to their actual memory addresses, even if they are defined later in the program than where they are used.
