# Motivation
* When you have many objects of a similar type that need to communicate with each other
* The communication between objects is complex

# Definition
    Define an object that encapsulates how a set of objects interact. Mediator promotes loose coupling by keeping objects from referring to each other explicitly, and it lets you very their interactions independently.
# Components 
* * Colleagues
* * * Individual components that need to communicate with each other
* * * Implement the same base type (abstract class or interface)
* * * Have knowledge of the Mediator component
* * Mediator
* * * The centralized component that managed communication between the colleague components.
* * * Implements an abstraction that is used by the Colleague components.

## examples
    - Aircraft (Colleague)
    - IAirTrafficControl ( Mediator)
### Advantages
* Hides all coordination between colleagues
* Decoupled colleagues
* Mediator's one-to-many relationship with colleagues is preferred to colleagues relating in a many-to-many fashion.

### Disadvantages
* The Mediator can become very large and very complicated as more colleagues are handled.


