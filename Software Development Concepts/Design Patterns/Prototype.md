**Creational Pattern** | The Prototype Pattern allows you to create new objects by copying existing ones, known as prototypes. It involves creating new objects by copying an existing object, known as the prototype, rather than creating new instances from scratch.

Documentation: [Prototype Pattern Reference](https://refactoring.guru/design-patterns/prototype)
___
### Overview
#### Primary Components:
- **Prototype**: An interface or abstract class that declares a method for cloning itself. It serves as the base for concrete prototypes.
- **ConcretePrototype**: Implements the Prototype interface and defines a method for cloning itself. It provides an implementation for cloning itself.
- **Client**: Uses the Prototype interface to clone objects without needing to know their concrete classes.

___
### Related Patterns
- [[Factory Method]]: Both Prototype and Factory Method are creational patterns. However, Prototype use delegation to create while Factory Method uses inheritance. They can also be used together. One can design a factory method that accept arguments and uses these arguments to find the correct prototype object, calls clone() on that object, and returns the result. The client replaces all references to the new operator with calls to the factory method. 
- [[Abstract Factory]]: Prototype and Abstract Factory are competing patterns in some ways. Prototype define new types simply by creating new prototypes while Abstract Factory requires the creation of new classes for defining new types. However, they can also be used together. An Abstract Factory might store a set of prototypes from which to clone and return product objects. 
- [[Abstract Factory]] and [[Builder]]: Similar to the prototype design pattern, these patterns hides the concrete product classes from the client, thereby reducing the number of names clients know about. 
- [[Composite]] and [[Decorator]]: Designs that make heavy use of the Composite and Decorator patterns often can benefit from Prototype. 
- [[Singleton]] and [[Abstract Factory]]: Prototype, Singleton and Abstract Factory are all creational patterns where you don’t use the new keyword to create a product but you call a method that will create the specific product and return a pointer to it. 
- [[Singleton]], [[Memento]] and [[Flyweight]]: These patterns administrate access to specific object instances similar to how Prototype administrates it. All of them offer factory methods to clients and share a create-on-demand strategy.

___