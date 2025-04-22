**Behavioural Pattern** | The Visitor Pattern lets you separate algorithms from the objects on which they operate. It allows you to add new operations to existing object structures without modifying the structures themselves. This is accomplished by creating a visitor class that implements the new operations, and applying this visitor to elements of the object structure.

Documentation: [Visitor Pattern Reference](https://refactoring.guru/design-patterns/visitor)
___
### Overview
#### Primary Components:
- **Visitor**: An interface or abstract class that declares visit operations for each type of element in the object structure. Each visit operation corresponds to a concrete element class.
- **ConcreteVisitor**: Implements the Visitor interface, providing specific implementations of the visit operations for each type of element in the object structure.
- **Element**: An interface or abstract class that declares an `accept` method, which takes a visitor as an argument. This method is implemented by concrete element classes.
- **ConcreteElement**: Implements the Element interface and defines the `accept` method. In this method, it calls the appropriate visit operation on the visitor object.
- **ObjectStructure**: A class that contains a collection of elements. It can iterate over these elements and apply visitors to them.

___
### Related Patterns
- [[Composite]]: The Composite is supportive to the Visitor. Visitors can apply an operation over an object structure defined by the Composite pattern. 
- [[Iterator]]: Iterator and Visitor has similar intents. Visitor, however, is more general than Iterator. An Iterator is restricted to operations on elements of the same kind while Visitor can operate on elements of different types. 
- [[Interpreter]]: The Visitor pattern may be applied to do the interpretation. 
- [[Abstract Factory]]: Abstract Factory and Visitor has similar structure. Abstract factory applies the structure to create families of objects while Visitor applies this structure to perform a group of related operations. 
- [[Bridge]]: Both Bridge and Visitor separates state and behaviour of objects. Bridge applies single dispatch while Visitor applies double dispatch.

___