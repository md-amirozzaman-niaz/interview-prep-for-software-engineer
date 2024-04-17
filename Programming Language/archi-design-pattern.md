# Architectural Design Patterns

## 1. Model-View-Controller (MVC)

- **Pattern**: MVC separates an application into three interconnected components: Model (data), View (user interface), and Controller (logic). It promotes separation of concerns, modularity, and maintainability.

## 2. Model-View-ViewModel (MVVM)

- **Pattern**: MVVM is a variation of MVC that separates the UI logic (View) from the business logic (Model) using a ViewModel. It is commonly used in modern client-side applications, such as web and mobile apps.

## 3. Layered Architecture

- **Pattern**: Layered architecture divides an application into multiple layers, each responsible for a specific aspect of functionality (e.g., presentation, business logic, data access). It promotes separation of concerns, scalability, and reusability.

## 4. Microservices Architecture

- **Pattern**: Microservices architecture decomposes an application into a set of loosely coupled, independently deployable services, each responsible for a specific business function. It enables flexibility, scalability, and rapid development of distributed systems.

## 5. Event-Driven Architecture (EDA)

- **Pattern**: EDA is an architectural style that emphasizes the production, detection, consumption, and reaction to events. It promotes loose coupling, scalability, and responsiveness by allowing components to communicate asynchronously through events.

## 6. Hexagonal Architecture (Ports and Adapters)

- **Pattern**: Hexagonal architecture separates the core business logic (hexagon) from external dependencies (ports and adapters). It enables easy integration with external systems, testing, and maintenance by isolating the core logic from external concerns.

## 7. Service-Oriented Architecture (SOA)

- **Pattern**: SOA is an architectural style that structures an application as a collection of loosely coupled, interoperable services. It promotes reusability, scalability, and flexibility by exposing functionality as services that can be consumed by other applications.

## 8. CQRS (Command Query Responsibility Segregation)

- **Pattern**: CQRS separates the responsibility for handling read and write operations into separate components. It allows for optimization of read and write operations independently, leading to improved scalability, performance, and maintainability.

## 9. Event Sourcing

- **Pattern**: Event sourcing persists the state of an application as a sequence of events rather than the current state. It enables auditability, versioning, and replayability of state changes, making it suitable for complex, event-driven systems.

## 10. Domain-Driven Design (DDD)

- **Pattern**: DDD is an approach to software development that focuses on modeling the core domain of a problem space. It emphasizes collaboration between domain experts and developers, ubiquitous language, and building software that reflects real-world concepts.

## Conclusion

Architectural design patterns provide blueprints and guidelines for designing software systems at the architectural level. By understanding and applying these patterns, architects and developers can create systems that are scalable, maintainable, and flexible.
