**Structural Pattern** | The Bridge Pattern decouples an abstraction from its implementation so that the two can vary independently. This pattern is useful for designing systems with complex and changing requirements, as it allows the abstraction and the implementation to be developed and evolved separately.

Documentation: [Bridge Pattern Reference](https://refactoring.guru/design-patterns/bridge)
___
### Overview
#### Primary Components:
- **Abstraction**: Defines the abstraction's interface and maintains a reference to an object of type Implementor.
- **RefinedAbstraction**: Extends the interface defined by Abstraction.
- **Implementor**: Defines the interface for implementation classes. This interface does not need to correspond directly to the Abstraction's interface; the two interfaces can be quite different.
- **ConcreteImplementor**: Implements the Implementor interface and defines the concrete implementation.

___
### Related Patterns
- **[[Adapter]]**: Both Adapter and Bridge use delegation to implement cooperation between classes. However, the Adapter is more often implemented.
- **[[Strategy]]**: Both Strategy and Bridge use delegation through an abstract interface to concrete implementations performing operations. However, the operations performed by the strategy pattern are interchangeable algorithms while the operations performed by the bridge pattern are common operations acting on interchangeable implementations such as different data structures or different operating systems.

___