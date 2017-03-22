# Motivation
* Some classes should have exactly one instance

# Intent
* Ensure a class has only one instance
* Make the class itself responsible for keeping track of its sole instance
* There can be only one

![structure](https://github.com/sairamaj/designpatterns/blob/master/singleton/structure.png)

# Consequences
* Default implementation of the single pattern is not thread safe
* Singletons introduce tight coupling among collaborating classes.
* Singletons are notoriously difficult to test
* * commonly regarded as an anti-pattern
* * using an IOC container it is straightforward to avoid the coupling and testability issues

# Related
* Abstract Factory
* Factory Method
* Builder

