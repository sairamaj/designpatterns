# Overview
* Specify the kinds of objects to create using prototypical instance, and create new objects by copying this prototype.
*  Preserving the state.
 
.NET - ICloneable

![structure](https://github.com/sairamaj/designpatterns/blob/master/prototype/structure.png)

#Roles
* Prototype
* * Interface or abstract class ( ICloneable )
* * Define a method to clone an object

* Concrete Prototype
* * An class implementing the Prototype
* * Basically has wa way to copy itself
* * Deep or shallow copy 

# Applicability
* Construction is expensive
* State is important
* Hiding the constructor.

