# Single Responsibility Principle
* The single responsibility principle states that every object should have a single responsibility, and that responsibility should be entirely encapsulated by the class.
* There should never be more than one reason for class to change

* Cohesion
  * Cohesion: how strongly-related and focused are the various responsibilities of a module
* Coupling
  * Coupling: the degree  to which each program module relies on each one of the other modules
* low coupling and high cohesion

# Open Closed Principle
* The Open/Closed Principle states that software entities( classes, modules, functions) should be open for extension and closed for modifications.
* Interfaces/Abstraction
## Three approaches to achieve OCP
* Parameters (Procedural Programming)
  * Allow client to control behavior specifics via a parameter
  * Combined with delegates/lambda, can be very powerful approach
* Inheritance / Template method pattern
  * Child types override behavior of base class(or interface)
* Composition / Strategy pattern
  * Client code depends on abstraction
  * Provides a plug-in model
  * Implementations use inheritance clients use composition

## The Liskov Substitution principle
* The Liskov substitution principle states that subtypes must be substitutable for their base types.
* child classes must not 
  * remove base class behavior
  * violates base class invariants
  * Must not require calling code to know that they are different from base types
  * Inheritance is ISA relationship
  * LISKOV suggests that ISA relationship should be replaced with IS-SUBSTITUABLE-FOR
  

