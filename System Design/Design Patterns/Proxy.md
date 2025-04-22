**Structural Pattern** | The Proxy Pattern provides a surrogate or placeholder for another object to control access to it. It allows for adding a level of indirection to support controlled access, lazy initialization, logging, caching, and other functionality.

Documentation: [Proxy Pattern Reference](https://refactoring.guru/design-patterns/proxy)
___
### Overview
#### Primary Components:
- **Subject**: An interface or abstract class that declares the common interface for both the RealSubject and the Proxy.
- **RealSubject**: Implements the Subject interface and defines the real object that the Proxy represents.
- **Proxy**: Implements the Subject interface and controls access to the RealSubject. It may handle additional responsibilities like lazy initialization, access control, logging, or caching.

___
### Related Patterns
- [[Adapter]]: Adapter and Proxy both provide an interface to access another object. However, the reasons for doing this are different. Adapter a different interface to the object it adapts. Proxy provides the same, or diminished interface to its subject. 
- [[Decorator]]: Decorator and Proxy both describe how to provide a level of indirection to an object and forward requests to it. However, they have a different purpose. Decorator provides a dynamic attach or detachment of an object through recursive composition. The component provides only part of the functionality. One or more decorators provide furnish the rest. Proxy provides a stand-in win it is inconvenient of undesirable to access the subject directly. With the proxy, the subject provides the key functionality. The proxy provides (or refuses) access to this functionality. 
- [[Prototype]]: Prototype and Proxy both offer a solution to a problem related to an object that is expensive to create. However, the solutions are different. Prototype keeps a copy of the object handy and clones it on demand. Proxy creates a stub for the object and created it on demand. 
- [[Flyweight]]: Flyweight and Proxy both apply a smart reference to manage access to an object. However, the purpose of the reference is quite different. Flyweight controls multiple pointers to a shared instance. It can be related back to a C++11 share ptr. A proxy controls single access to a specific object. This relates to a C++11 unique ptr.

___