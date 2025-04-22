**Behavioural Pattern** | The Template Method Pattern defines the skeleton of an algorithm in a method, deferring some steps to subclasses. It allows subclasses to redefine certain steps of an algorithm without changing the algorithm's structure. This pattern promotes code reuse and inversion of control.

Documentation: [Template Method Pattern Reference](https://refactoring.guru/design-patterns/template-method)
___
### Overview
#### Primary Components:
- **AbstractClass**: Defines the template method and declares abstract methods for steps that need to be implemented by subclasses. It may also include concrete methods that provide default implementations or helper methods.
- **ConcreteClass**: Implements the abstract methods defined in AbstractClass. These classes provide specific implementations of the steps required by the template method.

___
### Related Patterns
- [[Strategy]]: Both Strategy and the Template Method pattern defer implementation. However, Strategy uses delegation to defer the implementation of a complete algorithm while the Template Method pattern uses inheritance to defer only specific parts of an algorithm. 
- [[Factory Method]]: Although the Factory Method is not a specialisation of the Template Method pattern, it is related to the Template Method pattern. Many of the non-virtual methods that participate as AnOperation() in solutions that apply the Factory Method pattern are often template methods that, among others, call factory methods. 
- [[Adapter]]: Both the Adapter pattern and the Template Method pattern provides an interface through which operations that are implemented in other classes are called. The difference is that Adapter provides an interface to access non-complying operations that cannot be changed while the operations accessed through the template method is expected to comply and are most likely to change. 
- [[Builder]]: Both Builder and the Template Method pattern require a process to be encapsulated in a method. In fact the method that has to be implemented by the concrete builders to assemble a product is a template method.

___