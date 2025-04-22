**Structural Pattern** | The Flyweight Pattern allows sharing of objects to support a large number of fine-grained objects efficiently. It aims to minimize memory usage or computational expenses by sharing as much as possible with similar objects.

Documentation: [Flyweight Pattern Reference](https://refactoring.guru/design-patterns/flyweight)
___
### Overview
#### Primary Components:
- **Flyweight**: An interface or abstract class that defines the common interface for all flyweight objects. It includes methods to receive and act on extrinsic state.
- **ConcreteFlyweight**: Implements the Flyweight interface and represents flyweight objects. It stores intrinsic state (state shared among flyweights) and provides methods to manipulate extrinsic state.
- **FlyweightFactory**: Creates and manages flyweight objects. It ensures that flyweights are shared effectively by maintaining a pool of existing flyweight objects and reusing them when requested.

___
### Related Patterns
- **[[Composite]]**: In combination with flyweights, can be used to model directed-acyclic graphs. 
- **[[State]]**: can be implemented as flyweights. 
- **[[Strategy]]**: can also be implemented as flyweights.

___