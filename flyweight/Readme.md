# Intent
  * Structural 
  *  shared objects pattern
* Reduce storage costs for large number of objects
* Share objects to be used in multiple contexts simultaneously
* Retail object oriented granularity and flexibility

# States
* intrinsic ( shared - state does not change with context)
* extrinsic ( cannot be shared - state has to be supplied)

![structure](https://github.com/sairamaj/designpatterns/blob/master/flyweight/structure.png)

# Consequences
* Group of objects are replaced by a few shared objects once extrinsic state is removed
* Storage savings are derived from 
* * Reduced instances
* * Amount of intrinsic state per object
* * Whether extrinsic state is computed or stored.

* Application can no longer depend on object's identity
* .NET string.Intern is flyweight

