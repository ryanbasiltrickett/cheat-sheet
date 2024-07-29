**Behavioural Pattern** | The State Pattern allows an object to alter its behavior when its internal state changes. This pattern is particularly useful for objects that must change their behavior at runtime depending on their state. It encapsulates state-specific behavior into separate state objects and delegates the behavior to the current state object.

Documentation: [State Pattern Reference](https://refactoring.guru/design-patterns/state)
___
### Overview
#### Primary Components:
- **Context**: Maintains a reference to a State object, which represents the current state of the Context. It allows the state to be changed dynamically.
- **State**: An interface or abstract class that declares methods for handling requests, which concrete state classes will implement.
- **ConcreteState**: Classes that implement the State interface, encapsulating the behavior associated with a particular state of the Context.

___