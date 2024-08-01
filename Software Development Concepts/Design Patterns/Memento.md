**Behavioural Pattern** | The Memento Pattern is used in software development to capture and externalize an object's internal state so that the object can be restored to this state later, without violating encapsulation.

Documentation: [Memento Pattern Reference](https://refactoring.guru/design-patterns/memento)
___
### Overview
#### Primary Components
- **Originator**: The object whose state needs to be saved and restored. It creates a memento containing a snapshot of its current state and can use the memento to restore its state.
- **Memento**: A value object that acts as a snapshot of the Originator's state. It stores the internal state of the Originator and is typically immutable. The Memento does not expose the Originator's internal details to other objects.
- **Caretaker**: Manages the memento. It keeps track of the memento(s) but does not modify or inspect their content. The Caretaker requests a memento from the Originator, saves it, and can later provide it back to the Originator for state restoration.

___
### Related Patterns
- [[Command]]: Makes use of mementos to maintain the state of commands, in the order they were issued, in order to support undoable operations. 
- [[Iterator]]: Mementos can be used for iteration to maintain the state of the iterator.
- [[Bridge]]: Can be applied in order to separate the interface from the implementation of the memento in order to provide the wide interface between the originator and the memento without using the friend technique which violates object oriented encapsulation.

___