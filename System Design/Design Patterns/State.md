**Behavioural Pattern** | The State Pattern allows an object to alter its behavior when its internal state changes. This pattern is particularly useful for objects that must change their behavior at runtime depending on their state. It encapsulates state-specific behavior into separate state objects and delegates the behavior to the current state object.

Documentation: [State Pattern Reference](https://refactoring.guru/design-patterns/state)
___
### Overview
#### Primary Components:
- **Context**: Maintains a reference to a State object, which represents the current state of the Context. It allows the state to be changed dynamically.
- **State**: An interface or abstract class that declares methods for handling requests, which concrete state classes will implement.
- **ConcreteState**: Classes that implement the State interface, encapsulating the behavior associated with a particular state of the Context.

___
### Related Patterns
- [[Strategy]]: The Strategy and State patterns have the same structure and both apply the PV Principle to achieve their goals. However, they differ in intent. The Strategy pattern is about having different implementations that accomplishes the same result, so that one implementation can replace the other as the Strategy requires while the State pattern is about doing different things based on the state, while relieving the caller from the burden to accommodate every possible state. 
- [[Singleton]] and [[Prototype]]: When implementing the state pattern, the programmer has to decide on how the state objects will be created. Often the application of the Prototype pattern will be ideal. State objects are also often Singletons. 
- [[Flyweight]]: State objects can be shared by applying Flyweight.

___