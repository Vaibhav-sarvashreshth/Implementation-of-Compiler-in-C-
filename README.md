# If-Else-While Compiler for C in Yacc

This project is a simulation of the front-end phase of a C compiler that handles If-Else and While constructs. It's a comprehensive implementation that includes several stages of a typical compiler pipeline.

## Features

- **Lexical Analysis**: This stage involves tokenizing the input and entering it into an Input Table.
- **Syntactic Analysis**: The compiler creates an Abstract Syntax Tree (AST) during this phase.
- **Semantic Analysis**: This stage involves verifying type compatibility and generating Intermediate Code.
- **Machine Independent Code Optimization**: The compiler performs optimizations such as Constant Folding and Common Sub-Expression Elimination.

## How to Run

To run the program, follow these steps:

1. Place all files in the same directory.
2. Run `lex lexer.l` to generate the lexical analyzer.
3. Run `yacc -d -v parser.y` to generate the parser. The `-d` option creates `y.tab.h` and the `-v` option creates `y.output` (debugger for parser).
4. Compile the generated code with `gcc y.tab.c -ll`.
5. Run the compiled program with `./a.out < input.txt`.

## Files

- `lexer.l`: This is the lexical analyzer.
- `parser.y`: This is the parser, written in Yacc.
- `input.txt`, `input2.txt`, `input3.txt`, `input4.txt`, `input5.txt`: These are sample input files you can use to test the compiler.

## Language

The project is primarily written in Yacc (94.0%) and Lex (6.0%).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

