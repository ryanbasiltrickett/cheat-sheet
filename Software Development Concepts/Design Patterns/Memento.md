**Behavioural Pattern** | The Memento Pattern is used in software development to capture and externalize an object's internal state so that the object can be restored to this state later, without violating encapsulation.

Documentation: [Memento Pattern Reference](https://refactoring.guru/design-patterns/memento)
___
### Overview
#### Primary Components
- **Originator**: The object whose state needs to be saved and restored. It creates a memento containing a snapshot of its current state and can use the memento to restore its state.
- **Memento**: A value object that acts as a snapshot of the Originator's state. It stores the internal state of the Originator and is typically immutable. The Memento does not expose the Originator's internal details to other objects.
- **Caretaker**: Manages the memento. It keeps track of the memento(s) but does not modify or inspect their content. The Caretaker requests a memento from the Originator, saves it, and can later provide it back to the Originator for state restoration.

___