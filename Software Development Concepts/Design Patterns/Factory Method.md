**Creational Pattern** | The Factory Method Pattern defines an interface for creating an object but allows subclasses to alter the type of objects that will be created. It promotes loose coupling by eliminating the need to bind application-specific classes into the code.

Documentation: [Factory Method Pattern Reference](https://refactoring.guru/design-patterns/factory-method)
___
### Overview
#### Primary Components:
- **Product**: Defines the interface of objects the factory method creates.
- **ConcreteProduct**: Implements the Product interface.
- **Creator**: Declares the factory method, which returns an object of type Product. The Creator may also define a default implementation of the factory method that returns a default ConcreteProduct object.
- **ConcreteCreator**: Overrides the factory method to return an instance of ConcreteProduct.

___
### Related Patterns
- **[[Template Method]]**: The Factory Method may make use of Template Method in both the Product and the Creator hierarchies. 
- **[[Abstract Factory]]**: The Factory Method may be used in the implementation of the Abstract Factory design pattern. 
- **[[Prototype]]**: Factory Methods can be used to initialise prototypical objects. The prototype also can be used instead of the factory method to avoid large parallel hierarchies. Singleton In only one instance of a concrete factory is required, the concrete factory can be made a Singleton.

___