**Behavioural Pattern** | The Strategy Pattern defines a family of algorithms, encapsulates each one, and makes them interchangeable. The pattern lets the algorithm vary independently from clients that use it. It allows a client to choose an algorithm from a family of algorithms at runtime.

Documentation: [State Pattern Reference](https://refactoring.guru/design-patterns/state)
___
### Overview
#### Primary Components:
- **Strategy**: An interface or abstract class that defines a common method for all supported algorithms. This method is implemented by all concrete strategies.
- **ConcreteStrategy**: Classes that implement the Strategy interface and provide specific implementations of the algorithm.
- **Context**: Maintains a reference to a Strategy object and is configured with a ConcreteStrategy. The Context delegates the execution of the algorithm to the Strategy object.

___