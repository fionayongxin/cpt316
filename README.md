# Lexical and Syntax Analysis
This assignment implements a simple programming language with lexical and syntax analysis. The analysis divides into two primary components:

Lexical Analysis (Lexer): Tokenizes the input code.
Syntax Analysis (Parser): Constructs an Abstract Syntax Tree (AST) from tokenized code.

# Grammar
The following grammar rules define the language syntax.

Program : Stmt*
Stmt : AdditiveExpr
AdditiveExpr : MultiplicativeExpr((PLUS | MINUS) MultiplicativeExpr)*
MultiplicativeExpr : Factor((MUL | DIV) Factor)*
Factor : INTEGER

These rules describe the structure of valid programs in the language.

# Project Structure
Here are all the program files in LexicalSyntax folder

lexer.py: Lexical analysis implementation.
parser.py: Syntax analysis implementation.
ast.py: Abstract Syntax Tree (AST) classes.
main.py: Main program execution.
grammar.txt: Grammar rules define for the programming language.
test.txt: Example of input file.

# Abstract Syntax Tree (AST)
The structure of the parsed code is defined in the AST classes:

Program: Represents the whole program that contains a list of statements.
Stmt: Represents a generic statement in the AST.
BinaryExpr: Represents a binary expression
Factor: Represents a generic factor in the AST.
NumberFactor: A specific type of factor holding an integer value.
NodeType: Specifying the type of each AST node.

# Example for input data
Please find the sample input file at test.txt

# Running the Program
## Using an IDE
1. Open your preferred IDE that supports Python programming.
2. Load the project by opening the project folder.
3. Run the program by navigating to the main.py file in the project directory.
4. Execute the program main.py using your IDE.
5. Enter code directly into the console prompt.
6. Type exit to end the program or file to input the path from a file.

How to run on text case




# Contributors
This assignment was developed by the following members
1. Veytri A/L Yogan
2. Lim Yong Xin
3. Chan Yee Shuen
4. Soh Yen San
5. Khausaalyaah A/P Sinathurai

# License
This assignment codebase is licensed under the [MIT License](https://opensource.org/licenses/MIT/).
