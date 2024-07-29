**Behavioural Pattern** | The Template Method Pattern defines the skeleton of an algorithm in a method, deferring some steps to subclasses. It allows subclasses to redefine certain steps of an algorithm without changing the algorithm's structure. This pattern promotes code reuse and inversion of control.

Documentation: [Template Method Pattern Reference](https://refactoring.guru/design-patterns/template-method)
___
### Overview
#### Primary Components:
- **AbstractClass**: Defines the template method and declares abstract methods for steps that need to be implemented by subclasses. It may also include concrete methods that provide default implementations or helper methods.
- **ConcreteClass**: Implements the abstract methods defined in AbstractClass. These classes provide specific implementations of the steps required by the template method.

___