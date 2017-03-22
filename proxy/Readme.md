# Intent
* Provide a surrogate or placeholder for another object to control access to it.
* Also known as: Surrogate

# Motivation
* You need a place holder for an actual object tat is expensive to create
* * A placeholder image to show and allow for screen to lay out while actual image is being rendered
* You need to provie a local object that stands in place of a remote object and acts as an intermediary
* * You need to interact with a remove service over the network, but want to keep your coded decoupled from networking details.

# Applicability
* A __remote proxy__ local representation of a remote object
* A __virtual proxy__ expensive objects on demand.
* A __protection proxy__ to control access to an object.

Decorator has a similar implementation of Proxy, but its intent is different. A Decorator adds responsibility to an object, while the proxy controls access to an object.

![structure](https://github.com/sairamaj/designpatterns/blob/master/proxy/structure.png)    
![alernative](https://github.com/sairamaj/designpatterns/blob/master/proxy/structure2.png)   

