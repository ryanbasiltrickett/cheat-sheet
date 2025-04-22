**Behavioural Pattern** | The Iterator Pattern provides a way to access the elements of an aggregate object sequentially without exposing its underlying representation. It separates the traversal of a collection from the collection itself, allowing different traversal methods to be implemented independently.

Documentation: [Iterator Pattern Reference](https://refactoring.guru/design-patterns/iterator)
___
### Overview
#### Primary Components:
- **Iterator**: An interface that provides methods for traversing elements of a collection, such as `next()`, `hasNext()`, etc.
- **ConcreteIterator**: Implements the Iterator interface and keeps track of the current position in the traversal of the collection.
- **Aggregate**: Defines an interface for creating an Iterator object.
- **ConcreteAggregate**: Implements the Aggregate interface and provides an implementation for creating an Iterator object.

___
### Related Patterns
- **[[Factory Method]]**: Both Iterator and Factory Method use a subclass to decide what object should be created. In fact createIterator() is an example of a factory method. 
- **[[Memento]]**: The memento pattern is often used in conjunction with the iterator pattern. An iterator can use a memento to capture the state of the aggregate. This memento is stored inside the iterator to be used for traversing the aggregate. 
- **[[Adapter]]**: Both patterns provides an interface through which operations are performed. They differ in the reason for providing this interface. The adapter do it because it would be otherwise impossible while the iterator do it specifically to generalise iteration of aggregates. 
- **[[Composite]]**: Recursive structures such as composites usually need iterators to traverse them sequentially. Although recursive traversal might be very easy to implement without extending the composite pattern, its is strongly advised to create a composite iterator.

___