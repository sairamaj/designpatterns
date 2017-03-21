# Motivation
* It would be  useful to rollback one or more objects within your application toa previous state( for example, to implement Undo)
* Providing undo functionality within one or more classes would violate the Single Responsibility Principle
* Providing full access to object's internal state violates the encapsulation principle.
* The __memento pattern__ describes a way of capture object's internal state without violating encapsulation or SRP.

# Intent
* Without violating encapsulation, capture and externalize an object's internal state so that the object can be restored to this state later.
* The __memento pattern__ involves two objects: the __originator__ and the __caretaker__. The originator represents the object whose state is being tracked. The caretaker performs operations on the originator, bu needs to be able to undo the operations.

# Applicability
* You need to be able to track the state of an object or your application and restore previous state as needed.
* You want to abstract and reuse the Undo/Redo functionality
* * follow SRP and Don't Repeat Yourself(DRY)
* You do not wish to break encapsulation and expose your classes, internal state globally.

![structure](https://github.com/sairamaj/designpatterns/blob/master/memento/structure.png)