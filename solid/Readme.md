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

# Interface Segregation
* Clients should not be forced to depend on methods they do not use.
* Prfer small, cohesive interfaces to "fat" interfaces
* Refactor large interfaces so that they inherit small interfaces
* ISP Smells
  * Unimplemented interface methods (NotImplementedException)
  * Client references a class but only uses small portions of it.

# Dependency Inversion Principle
* High level modules should not depend on low level modules. Both should depend on abstractions
* Abstractions should not depend on details. detail should depend on abstractions.
* Is a technique that is used to allow calling code to inject the dependencies a class needs when it is instantiated.
* Hollywood principle
  * Don't calls us. we'll call you.
* Three primary techniques
  * Constructor Injection
  * Property Injection
  * Parameter Injection
* DIP Smell
  * use of new keyword
  * use of static methods/properties
  

# DRY
* Every piece of knowledge must have a single, unambiguous representation in the system
* Repetition in logic calls for abstraction. Repetition in process calls for automation
* Once and Only Once
* Duplication is Evil(DIE)
  * Magic Strings/Values
  * Duplicate Logic in several methods
  * Repeated if then logic
  * conditionals instead of polymorphism
  * Repeated execution patterns
  * Lots of duplicate, probably copy-pated, code
  * only manual tests
  * static methods everywhere.
  

