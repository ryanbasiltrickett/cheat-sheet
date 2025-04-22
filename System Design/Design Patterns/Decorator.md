**Structural Pattern** | The Decorator Pattern allows behavior to be added to individual objects dynamically, without affecting the behavior of other objects from the same class. It is used to extend or alter the functionality of objects at runtime by wrapping them with a decorator object.

Documentation: [Decorator Pattern Reference](https://refactoring.guru/design-patterns/decorator)
___
### Overview
#### Primary Components:
- **Component**: An interface or abstract class that defines the interface for objects that can be decorated. It specifies the operations that can be modified or extended by decorators.
- **ConcreteComponent**: Represents the basic object to which additional responsibilities can be added. It implements the Component interface.
- **Decorator**: Maintains a reference to a Component object and defines an interface that conforms to the Component's interface. It can also include additional state or behavior.
- **ConcreteDecorator**: Adds new responsibilities to the component by extending or modifying its behavior. It implements the Decorator interface and adds its own behavior either before or after delegating to the component.

___
### Related Patterns
- **[[Adapter]]**: Changes the interface to an object while the Decorator only changes responsibilities. 
- **[[Composite]]**: A Decorator can be seen as a Composite with only one component that has added responsibility. 
- **[[Strategy]]**: The Strategy pattern changes the inner workings of an object while the Decorator changes the object's properties.

___