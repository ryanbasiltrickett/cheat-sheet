**Behavioural Pattern** | The Observer Pattern defines a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically. It promotes loose coupling between objects by ensuring that changes to one object can trigger updates in multiple other objects.

Documentation: [Observer Pattern Reference](https://refactoring.guru/design-patterns/observer)
___
### Overview
#### Primary Components:
- **Subject**: An interface or abstract class that defines methods for attaching, detaching, and notifying observers. It also includes a method to get or set the subject's state.
- **ConcreteSubject**: Implements the Subject interface and maintains the state of interest. It notifies observers when its state changes.
- **Observer**: Defines an interface for objects that should be notified of changes in the subject's state.
- **ConcreteObserver**: Implements the Observer interface and receives notifications from the subject when its state changes. It updates itself based on the state changes of the subject.

___