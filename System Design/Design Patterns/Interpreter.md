**Behavioural Pattern** | The Interpreter Pattern defines a grammar for interpreting a language and provides a way to evaluate sentences in that language. It involves creating an interpreter that parses and interprets expressions in a specific language or notation.

Documentation: [Interpreter Pattern Reference](https://sourcemaking.com/design_patterns/interpreter#:~:text=The%20Interpreter%20pattern%20defines%20a,provides%20the%20language%20of%20music.)
___
### Overview
#### Primary Components:
- **AbstractExpression**: An interface or abstract class that declares an interpret operation. It defines a method for interpreting expressions.
- **TerminalExpression**: Represents terminal expressions in the language grammar. It implements the interpret operation for terminal expressions.
- **NonterminalExpression**: Represents nonterminal expressions in the language grammar. It implements the interpret operation for nonterminal expressions by combining the interpretation of multiple expressions.
- **Context**: Contains information that is global to the interpreter and is passed to individual expressions during interpretation.

___
### Related Patterns
- **[[Template Method]]**: The template method and the interpreter design patterns are the only two Gamma:1995 behavioural patterns that uses inheritance as its basic strategy to achieve its purpose. All other Gamma:1995 behavioural patterns uses delegation. 
- **[[Composite]]**: Interpreter is an application of the Composite pattern. It ads specific behaviour to the composite structure namely to interpret the elements of the composite structure. Note that is more specific than just an operation distributed over a class hierarchy that uses the Composite pattern. It is specifically aimed at dealing with problems that are specified in terms of grammars. 
- **[[Flyweight]]**: Both Flyweight and Interpreter share symbols. Interpreter share terminal symbols within the abstract syntax tree. 
- **[[Visitor]]**: Both Interpreter and Visitor adds behaviour to a composite structure. Where interpreter adds a simplistic behaviour, visitor allows for more generic and adaptable behaviour. The similarity between these patterns is deep. The operations of an interpreter can always be refactored into interpreter visitors. 
- **[[State]]**: The interpreter design pattern and the state design pattern are different ways to solve interpretation. Where the interpreter pattern provide a way to interpret parse trees directly while it is possible to first transform a parse three into a state machine and then applying the state pattern to solve the same problem

___