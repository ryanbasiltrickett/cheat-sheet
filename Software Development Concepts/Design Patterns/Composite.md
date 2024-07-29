**Structural Pattern** | The Composite Pattern allows clients to treat individual objects and compositions of objects uniformly. It composes objects into tree structures to represent part-whole hierarchies.

Documentation: [Composite Pattern Reference](https://refactoring.guru/design-patterns/composite)
___
### Overview
#### Primary Components:
- **Component**: An interface or abstract class that defines the common interface for all components in the composition, whether they are composite or leaf nodes.
- **Leaf**: Represents individual objects in the composition. It implements the operations defined by the Component interface.
- **Composite**: Represents a composite object that can have children. It implements operations to manage its child components, such as adding, removing, or accessing them.

___
### Related Patterns
- **[[Software Development Concepts/Design Patterns/Chain of Responsibility|Chain of Responsibility]]**: Creates a structure that defines a component-parent link.
- **[[Decorator]]**: Used in conjunction with components to add state to the components. When a decorator and a composite are combined, they usually share the same parent class. 
- **[[Flyweight]]**: Allows sharing of objects, particularly the leaf nodes Iterator and Visitor Used to traverse the composite structure.

___