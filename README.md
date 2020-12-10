# Principles_of_Programming_Languages

# Calculator 
calc.l:
A lexical scanner to recognize numbers, symbols and the EQ
operator.  When a NUMBER is found, its value is set is set to the
appropriate float.  When a NAME is found, an entry in symbol table is
created (with initial value 0.0) and the token's value is a pointer to
this entry.  If a '==' sequence is seen, it is returned as a token
EQ.  Spaces and tabs are ignored. Any other characters, including
a newline, are passed on as their own tokens.

calc.y:
* Defines a yacc grammar for a simple calculator using infix
* notation.  WHen executed, the calculator enters a loop in
* which it prints the prompt >>, reads a toplevel expression
* terminated by a newline, and prints its value.  Operators
* include +, -, *, and = (assignment). Note that all
* expressions return values, even assignment.  Parentheses
* can be used to override operator precedence and
* associativity rules.
