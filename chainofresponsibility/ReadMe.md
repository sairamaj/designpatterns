* Behavioral 

# Steps
* Sender is aware of only one receiver
* Each receiver is only aware of the next receiver
* Receivers process the message or send it down the chain
* The sender does not know who received the message
* The first receiver to handler the message terminates the chain
* The order of the receiver list matters

![usage](https://github.com/sairamaj/designpatterns/blob/master/chainofresponsibility/usage.png)
 
 ## Use the Chain of Responsibility when..
 * More than one message handler for a message
 * The appropriate handler is not explicitly known by the sender
 * The set of handlers can be dynamically defined

## Benefits
* Reduced coupling
* Dynamically manage the message handlers
* End of chain behavior can be defined appropriately
