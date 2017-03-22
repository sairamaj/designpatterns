# Motivation
* When one object is dependent on another object.
* When changing one object requires a change to many others
* when changes to an object should allow notification to others without any knowledge of them.

# Intent
* Adopt the principle of Separation of  Concerns
* Allows multiple observers to react to changes to a single subject

# Structure
* Subject provides a way to Register, Un register, Notify
* Observers provide a way to update.

# .NET
* Events
* IObserver<T> and IObservable<T>
