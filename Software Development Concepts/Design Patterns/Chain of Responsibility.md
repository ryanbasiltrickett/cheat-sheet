**Behavioural Pattern** | The Chain of Responsibility Pattern allows an object to pass a request along a chain of potential handlers until one of them handles the request. It decouples senders and receivers of requests by giving multiple objects the chance to handle the request.

Documentation: [Chain of Responsibility Reference](https://refactoring.guru/design-patterns/chain-of-responsibility)
___
### Overview
#### Primary Components:
- **Handler**: Defines an interface for handling requests and optionally implements the successor link (reference to the next handler in the chain).
- **ConcreteHandler**: Implements the Handler interface and handles requests it is responsible for. It can also delegate requests to the next handler in the chain.
- **Client**: Initiates requests to the first handler in the chain.

___
### Related Patterns
- **[[Composite]]**: Chain of Responsibility is often applied in conjunction with Composite. For instance a component’s parent can act as its successor.

___