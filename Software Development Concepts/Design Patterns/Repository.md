**Structural Pattern** | The Repository Pattern is a design pattern commonly used in software development to mediate between the domain and data mapping layers, providing a centralized location for data access logic. It encapsulates the set of objects stored in a data store and the operations performed over them, offering a more object-oriented view of data operations.

Documentation: [Repository Pattern Reference](https://www.geeksforgeeks.org/repository-design-pattern/)
___
### Overview
#### Primary Components:
- **Repository**: Defines a collection-like interface for accessing domain objects. It typically includes methods for adding, removing, updating, and retrieving objects.
- **ConcreteRepository**: Implements the Repository interface, providing the actual data access logic. It interacts with the data store (e.g., database) to perform CRUD (Create, Read, Update, Delete) operations.
- **Domain Model**: Represents the domain entities that the Repository manages. These are typically business objects that encapsulate business rules and data.
- **Client**: Uses the Repository to perform operations on domain objects without needing to interact directly with the data store.

___
### Related Patterns
- **[[Factory]]**: Factories can be used to create instances of repositories, especially when repositories have complex creation logic or depend on external resources like database connections.
- **[[Decorator]]**: This pattern can be used to add additional behavior to repositories. For example, you can use a decorator to add caching to a repository.
- **[[Strategy]]**: The Strategy pattern can be used to define different query strategies that can be used by a repository. This allows for flexible querying mechanisms.

___