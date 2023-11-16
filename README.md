# Lexical and Syntax Analysis
<p>This assignment implements a simple programming language with lexical and syntax analysis. The analysis divides into two primary components:</p>

<ul>
  <li>Lexical Analysis (Lexer): Tokenizes the input code.</li>
  <li>Syntax Analysis (Parser): Constructs an Abstract Syntax Tree (AST) from tokenized code.</li>
</ul>

# Grammar
<p>The following grammar rules define the language syntax.</p>

  >**Program** : Stmt* <br><br>
  >**Stmt** : AdditiveExpr <br><br>
  >**AdditiveExpr** : MultiplicativeExpr((PLUS | MINUS) MultiplicativeExpr)* <br><br>
  >**MultiplicativeExpr** : Factor((MUL | DIV) Factor)* <br><br>
  >**Factor** : INTEGER <br>
  >(Open_Paren) AdditiveExpr (Close_Paren) 
<p>These rules describe the structure of valid programs in the language.</p>

# Project Structure
Here are all the program files in ***LexicalSyntax*** folder

>`lexer.py`: Lexical analysis implementation. <br><br>
>`parser.py`: Syntax analysis implementation. <br><br>
>`ast.py`: Abstract Syntax Tree (AST) classes. <br><br>
>`main.py`: Main program execution. <br><br>
>`grammar.txt`: Grammar rules define for the programming language. <br><br>
>`test.txt`: Example of input file. <br><br>

# Abstract Syntax Tree (AST)
<p>The structure of the parsed code is defined in the AST classes:</p>

>**Program**: Represents the whole program that contains a list of statements. <br><br>
>**Stmt**: Represents a generic statement in the AST. <br><br>
>**BinaryExpr**: Represents a binary expression. <br><br>
>**Factor**: Represents a generic factor in the AST. <br><br>
>**NumberFactor**: A specific type of factor holding an integer value. <br><br>
>**NodeType**: Specifying the type of each AST node. <br><br>

# Example for input data
<p>Please find the sample input file at `test.txt</p>

# Running the Program
## Using an IDE
>1. Open your preferred IDE that supports Python programming. 
>2. Load the project by opening the project folder.
>3. Run the program by navigating to the `main.py` file in the project directory.
>4. Execute the program `main.py` using your IDE.
>5. Enter code directly into the console prompt.
>6. Type _exit_ to end the program or file to input the path from a file.

How to run on text case




# Contributors
<p>This assignment was developed by the following members</p>
<ol>
  <li>Veytri A/L Yogan</li>
  <li>Lim Yong Xin</li>
  <li>Chan Yee Shuen</li>
  <li>Soh Yen San</li>
  <li>Khausaalyaah A/P Sinathurai</li>
</ol>

# License
<p>This assignment codebase is licensed under the</p>
[MIT License](https://opensource.org/licenses/MIT/)
