 # Intent
 * Rid program logic of null checks where possible
 * Provide a non-functional object in place of a null reference
 * Allow methods to be called on Null objects, unlike a null reference.


 # Applicability
 * When handling of null should be abstracted from the client
 * When an object required a collaborator
 * Examples
 * * Implementing a Null strategy object when we don't want work actually be done by the strategy executor.
 * * Implementing a Null command object when we want the command executor to do nothing.

![structure](https://github.com/sairamaj/designpatterns/blob/master/nullobject/structure.png)

# Consequences
* Code is cleaner and more concise
* Fewer null checks needed.
* Less branching in the code means lower complexity
* Callers don't need to care whether they have a NullObject or a RealObject
* Unless developers are aware of the NullObject implementation exists, they may still do null checks.
