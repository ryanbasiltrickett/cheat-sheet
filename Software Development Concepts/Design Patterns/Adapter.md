**Structural Pattern** | The Adapter Pattern allows incompatible interfaces to work together. It acts as a bridge between two incompatible interfaces by converting the interface of a class into another interface that a client expects. This pattern is especially useful when integrating with legacy code or third-party libraries.

Documentation: [Adapter Pattern Reference](https://refactoring.guru/design-patterns/adapter)
___
### Overview
#### Primary Components:
- **Target**: Defines the domain-specific interface that the client uses.
- **Client**: Collaborates with objects conforming to the Target interface.
- **Adaptee**: Defines an existing interface that needs to be adapted.
- **Adapter**: Implements the Target interface and adapts the interface of the Adaptee to the Target interface.
#### Types of Adapters:
- **Class Adapter**: Uses inheritance to adapt one interface to another. This involves multiple inheritance, where the adapter inherits from both the Target and the Adaptee.
- **Object Adapter**: Uses composition to adapt one interface to another. The adapter holds an instance of the Adaptee and implements the Target interface by delegating calls to the Adaptee instance.

___
### Related Patterns
- **[[Bridge]]**: Structurally they are similar. However their intent is different, the Adapter changes the interface while the Bridge separates the implementation from the interface. 
- **[[Decorator]]**: Enhances an object without changing the interface. 
- **[[Proxy]]**: Defines a surrogate of to an object without changing its interface.

___