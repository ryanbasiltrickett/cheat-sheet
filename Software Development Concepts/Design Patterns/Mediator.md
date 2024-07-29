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