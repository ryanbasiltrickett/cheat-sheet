**Behavioural Pattern** | The Event Aggregator Pattern provides a mechanism for loosely coupling objects within a system by allowing them to communicate through a centralized event dispatcher. It enables objects to publish and subscribe to events without needing direct references to each other, promoting better separation of concerns and easier maintenance.

Documentation: [Event Aggregator Reference](https://developer.confluent.io/patterns/stream-processing/event-aggregator/)
___
### Overview
#### Primary Components:
- **Event Aggregator**: A class or service responsible for managing the communication between different parts of the system by allowing them to publish and subscribe to events.
- **Publisher**: An object that generates or publishes events. It sends events to the event aggregator for distribution.
- **Subscriber**: An object that listens for events. It registers with the event aggregator to receive notifications when specific events occur.
- **Event**: An object representing a specific occurrence or action within the system. It contains data relevant to the event and is passed between publishers and subscribers.

___
### Related Patterns
- **[[Mediator]]**: The Mediator and Event Aggregator patterns both communicate between multiple connected objects. However, the Mediator has logic to send messages to specific objects and Event Aggregator sends all messages to all connected objects.

___