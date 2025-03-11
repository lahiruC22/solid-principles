# SOLID Principles

## SOLID Principles Overview

The SOLID principles are a set of five design guidelines in software architecture and object-oriented programming that aim to create systems that are more maintainable, scalable, and easier to understand. These principles were introduced by Robert C. Martin (Uncle Bob) and form a foundation for writing clean and modular code.

* S – Single Responsibility Principle
* O – Open/Closed Principle
* L – Liskov Substitution Principle
* I – Interface Segregation Principle
* D – Dependency Inversion Principle

### Benefits of SOLID Principles

* Maintainability – The code is easier to understand and modify.
* Scalability – Adding new features is simpler and less error-prone.
* Testability – The code becomes modular and easier to test.
* Re usability – Classes and components can be reused across project.

You can apply SOLID Principles in any object oriented programming language.

### Single Responsibility Principle (SRP):
**Definition:**

“*A Class should have only one reason to change*”

In simple terms, this means that a class, module, or function should focus on a single task or responsibility. Each class should be narrowly focused and encapsulate functionality related to one specific aspect of the system.

**Key Concept of SRP:**

* **Responsibility** – A reason for change. If a class has more than one responsibility, it means it can have multiple reason to change, which can make the class unstable and difficult to maintain.

* **Cohesion** – SRP encourages high cohesion i.e the class should group closely related functionalities. A high cohesive class performs one well-defined task and nothing else.

* **Separation of Concerns** – The different aspects of the system are handled in separate classes. This reduces complexity and makes the system easier to understand.

**What Cohesion means?**

The degree to which the elements inside a module belong together or a measure of the strength of relationship between the methods and data of a class and some unifying purpose or concept served by that class. A measure of the strength of relationship between the class’s methods and data. It is a ordinal value and has two types high cohesion and low cohesion.
Link: https://en.wikipedia.org/wiki/Cohesion_(computer_science)

**What is Separation of Concerns?**

A design principle for separating a computer program into distinct sections. Each section addresses a separate concern, a set of information that affects the code of a computer program.
Link: https://en.wikipedia.org/wiki/Separation_of_concerns

**Why SRP is needed?**

* Ease of Maintenance – Simpler to understand and update. Changes in one responsibility won’t affect others.

* Reduced Coupling – Keeping responsibilities separate ensures that classes don’t depend on unrelated logic, making them less intertwined.

* Better Testability – Smaller focused classes are easier to test because they perform one task, and tests can isolate specific behaviors.

**Real world Analogy:**

Think of a restaurant:

* The chef is responsible for cooking.
* The waiter is responsible for serving food to customers.
* The cashier is responsible for handling payments.

If one person tries to handle all these tasks, the process becomes inefficient, error-prone, and hard to manage. Separating responsibilities ensures smooth operations.

**Violating SRP: Signs and Symptoms**

* Classes with too many methods or fields often indicate multiple responsibilities.
* If you struggle to describe a class in a single sentence, it likely has more than one responsibility.
* If you modify a class often because of changes in different functionalities, it’s a sign that violates SRP.


**How to Implement SRP?**

1. Analyze your code and determine what tasks each class or function performs.
2. Split classes that handle multiple responsibilities into smaller, cohesive classes,
3. Ensure the name of the class reflects its single responsibility.
4. Patterns like Factory, Strategy or Observer can help maintain single responsibility.
