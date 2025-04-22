**Behavioural Pattern** | The Mediator Pattern defines an object that encapsulates how objects interact with each other, thus promoting loose coupling between them. It centralizes complex communication and control logic between related objects by encapsulating it within a mediator object.

Documentation: [Mediator Pattern Reference](https://refactoring.guru/design-patterns/mediator)
___
### Overview
#### Primary Components:
- **Mediator**: An interface or abstract class that defines methods for communication between Colleague objects.
- **ConcreteMediator**: Implements the Mediator interface and coordinates communication between Colleague objects. It maintains references to all Colleague objects and facilitates their interaction.
- **Colleague**: Defines an interface for interacting with other Colleague objects through the Mediator.
- **ConcreteColleague**: Implements the Colleague interface and communicates with other Colleague objects through the Mediator. It sends and receives messages through the Mediator rather than directly communicating with other Colleagues.

___
### Related Patterns
- [[Façade]]: Differs from Mediator in that it abstracts a subsystem of objects to provides more convenient interface. Its protocol is unidirectional; that is, Façade objects make requests of the subsystem classes but not vice versa. In contrast, Mediator enables cooperative behaviour that colleague objects don’t or can’t provide, and the protocol is multidirectional. 
- [[Observer]]: Colleagues can communicate with the mediator using the Observer pattern.

___