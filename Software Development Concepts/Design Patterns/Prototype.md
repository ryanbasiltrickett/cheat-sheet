**Creational Pattern** | The Prototype Pattern allows you to create new objects by copying existing ones, known as prototypes. It involves creating new objects by copying an existing object, known as the prototype, rather than creating new instances from scratch.

Documentation: [Prototype Pattern Reference](https://refactoring.guru/design-patterns/prototype)
___
### Overview
#### Primary Components:
- **Prototype**: An interface or abstract class that declares a method for cloning itself. It serves as the base for concrete prototypes.
- **ConcretePrototype**: Implements the Prototype interface and defines a method for cloning itself. It provides an implementation for cloning itself.
- **Client**: Uses the Prototype interface to clone objects without needing to know their concrete classes.

___