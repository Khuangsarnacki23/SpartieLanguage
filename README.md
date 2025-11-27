Spartie is a custom programming language that I am building an interpreter for.
The interpreter reads Spartie code and converts (interprets) it into Java.
For an overview of the language syntax, see: [Spartie Syntax Overview (PDF)](Spartie%20Syntax%20Overview.pdf)

Main Program
- Reads a source file, then runs scanning → parsing → interpreting in order.
- Handles errors like missing files or invalid usage.

Scanner (Lexing)
- Converts raw text into tokens (keywords, identifiers, numbers, strings, operators).
- Skips whitespace/comments and recognizes if, while, var, print, etc.

Parser (AST Builder)
- Builds Statements and Expressions from tokens (variables, prints, if/else, while, for, blocks).
- Implements full expression grammar: arithmetic, comparisons, logical operators.

Interpreter (Executor)
- Maintains a variable environment and evaluates expressions.
- Executes statements (print, assignments, conditionals, loops, blocks) directly.
