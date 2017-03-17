# Overview
Behaviorial

## Motivation
* you work with objects that must be loaded from a persistent store( e.g. database)
* you want to avoid loading portions of the objects state that you don't necessarily need
* you don't want the client code to have to know if or when it needs to load additional state - the bjects themsleves should manage this
* The __lazy load pattern__ describes several strategies to achieve these goals.

## Intent
A Lazy load interrupts the object loading process for the moment leaving a marker in the object structure so that if the data is needed it can be loaded only when it is used.

## Applicability
* Fetching an object required an extra call for the data, and the data you are fetching is not used when the main object is used.
* Avoid using it unless or until you need it - use it as a tuning mechanism
* Need to balance amount of data being fetched with number of data requests being made.

### Lazy Initialization
* Every property checks to see if its backing field has been initialized
* Lazy<T>

### Virtual proxy
* Proxy looks just like the real object
 
### Value Holder
* ValueHolder and IValueLoader (similar to Lazy<T>)

### Ghosts
* a __ghost__ is a real objects in a partial state.
* whenever any property is accessed, the ghost class loads all of its state from persistence. 
