**Creational Pattern** | The Singleton Pattern ensures a class has only one instance and provides a global point of access to that instance. It is useful for managing shared resources or configurations that need to be accessed throughout an application.

Documentation: [Singleton Pattern Reference](https://refactoring.guru/design-patterns/singleton)
___
### Overview
#### Primary Components:
- **Singleton**: The class that is designed to have only one instance. It includes a method for obtaining the instance and ensures that no additional instances can be created.

___
### Related Patterns
- [[Prototype]]: Sometimes apply lazy instantiation. Singleton does this to save memory while Prototype uses it to save processing power. 
- [[Abstract Factory]] and [[Builder]]: Can use Singleton in their implementation. 
- [[Façade]]: Are often Singletons because only one Façade object is required. 
- [[State]]: Are often Singletons.

___