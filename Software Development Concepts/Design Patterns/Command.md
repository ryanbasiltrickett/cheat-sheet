**Behavioural Pattern** | The Command Pattern encapsulates a request as an object, thereby allowing parameterization of clients with queues, requests, and operations. It allows the separation of the sender of a request from the receiver, providing flexibility, extensibility, and decoupling between the two.

Documentation: [Command Pattern Reference](https://refactoring.guru/design-patterns/command)
___
### Overview
#### Primary Components:
- **Command**: Defines an interface for executing an operation. It typically includes a method like `execute()`.
- **ConcreteCommand**: Implements the Command interface and encapsulates the receiver and the action to be performed.
- **Invoker**: Asks the command to carry out the request.
- **Receiver**: Knows how to perform the operation associated with the command.

___
### Related Patterns
- **[[Software Development Concepts/Design Patterns/Chain of Responsibility|Chain of Responsibility]]**: Makes use of Command to represent requests as objects.
- **[[Composite]]**: MacroCommands can be implemented when combining command with Composite. 
- **[[Memento]]**: Makes use of Command to keep state the command requires to undo its effect. Prototype: A command that must be copied before being placed on the history list acts as a Prototype.

___