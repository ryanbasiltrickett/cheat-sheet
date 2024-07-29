**Creational Pattern** | The Abstract Factory Pattern provides an interface for creating families of related or dependent objects without specifying their concrete classes. This pattern is useful when a system needs to be independent of how its products are created, composed, and represented.

Documentation: [Abstract Factory Pattern Reference](https://refactoring.guru/design-patterns/abstract-factory)
___
### Overview
#### Primary Components:
- **AbstractFactory**: Declares an interface for operations that create abstract products.
- **ConcreteFactory**: Implements the operations to create concrete products.
- **AbstractProduct**: Declares an interface for a type of product object.
- **ConcreteProduct**: Implements the AbstractProduct interface.
- **Client**: Uses only interfaces declared by AbstractFactory and AbstractProduct classes.

___
### Related Patterns
- **[[Factory Method]] or [[Prototype]]**: The Abstract Factory makes use of the Factory Method or the Prototype for the creation of product. 
- **[[Template Method]]**: May be used within the abstract factory and product hierarchies. 
- **[[Singleton]]**: Concrete factories may be implemented as Singletons.

___