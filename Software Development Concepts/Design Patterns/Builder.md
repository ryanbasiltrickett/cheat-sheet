**Creational Pattern** | The Builder Pattern separates the construction of a complex object from its representation, allowing the same construction process to create different representations. It aims to solve the problem of telescoping constructors, where the number of constructor parameters grows rapidly with the complexity of the object.

Documentation: [Builder Pattern Reference](https://refactoring.guru/design-patterns/builder)
___
### Overview
#### Primary Components:
- **Director**: Responsible for orchestrating the construction of the complex object. It interacts with the Builder to define the steps of construction.
- **Builder**: Defines an abstract interface for creating parts of a complex object. It provides methods for constructing individual parts and for retrieving the final object. There can be different concrete builders implementing this interface to create different representations of the product.
- **ConcreteBuilder**: Implements the Builder interface to construct and assemble parts of the complex object. It defines methods for building each part of the product.
- **Product**: Represents the complex object under construction. It's the object that is being built.

___
### Related Patterns
- **[[Composite]]**: Builder usually construct composite objects. 
- **[[Abstract Factory]]**: Abstract Factory is similar to Builder in that it too may construct complex objects. The primary difference is that the Builder pattern focuses on constructing a complex object step by step. Abstract Factory’s emphasis is on families of product objects (either simple or complex). Builder returns the product as a final step, but as far as the Abstract Factory pattern is concerned, the product gets returned immediately

___