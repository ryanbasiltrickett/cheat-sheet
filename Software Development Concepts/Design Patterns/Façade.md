**Structural Pattern** | The Facade Pattern is a structural design pattern that provides a simplified interface to a set of interfaces in a subsystem. It encapsulates a complex subsystem behind a single interface, making it easier to use and understand.

Documentation: [Façade Pattern Reference](https://refactoring.guru/design-patterns/facade)
___
### Overview
#### Primary Components:
- **Facade**: A class or interface that provides a simplified interface to a complex subsystem. It shields clients from the complexities of the subsystem by providing a unified interface.
- **Subsystem Classes**: Classes that implement the functionality of the subsystem. These classes are not directly accessible to clients but are used internally by the façade to fulfil client requests.

___
### Related Patterns
- **[[Adapter]]**: Façade is in a sense a huge object adapter that simultaneously adapts a number of classes with the intent to simplify communication with those classes. While both the façade and the adapter my wrap any number of classes, their intent is different. The adapter wraps to provide the expected interface, while the façade wraps to provide a simplified interface. 
- **[[Template Method]]**: Façade is in a sense a huge template method that defines the skeleton of an algorithm for a process that is automated. However, instead of deferring some steps to subclasses, it delegates steps to the different classes comprising a system. 
- **[[Mediator]]**: Mediator is similar to Façade in that it abstracts functionality of existing classes. However, Mediator’s purpose is to abstract arbitrary communication between colleague objects, often centralizing functionality that doesn’t belong in any one of them. A mediator’s colleagues are aware of and communicate with the mediator instead of communicating with each other directly. In contrast, a façade merely abstracts the interface to subsystem objects to make them easier to use; it doesn’t define new functionality, and subsystem classes don’t know about it.

___