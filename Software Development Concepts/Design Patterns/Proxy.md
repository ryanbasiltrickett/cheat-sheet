**Structural Pattern** | The Proxy Pattern provides a surrogate or placeholder for another object to control access to it. It allows for adding a level of indirection to support controlled access, lazy initialization, logging, caching, and other functionality.

Documentation: [Proxy Pattern Reference](https://refactoring.guru/design-patterns/proxy)
___
### Overview
#### Primary Components:
- **Subject**: An interface or abstract class that declares the common interface for both the RealSubject and the Proxy.
- **RealSubject**: Implements the Subject interface and defines the real object that the Proxy represents.
- **Proxy**: Implements the Subject interface and controls access to the RealSubject. It may handle additional responsibilities like lazy initialization, access control, logging, or caching.

___