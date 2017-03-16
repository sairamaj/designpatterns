# Overview
  Creational

# When to use
*  Unsure which concrete implementation of an interface I want to return
*  Creation should be separated from representation of an object
*  Lots of if/else blocks when deciding which concrete class to create
*  Switch statements when deciding which concrete class to create

# Intent
* separate object creation from the decision of which object to create
* Add new classes and functionality without breaking OCP (open close principle)
* Store which object to create outside of the program
* * in a database
* * in a configuration

# Simple Factory ( no interface )
``` csharp
    class Autofactory
    {
        IAuto CreateInstance(string name);
    }
    var factory = new AutoFactory();
    factory.CreateInstance(carname);
```
# Factory Method ( through interface but one creation)
   Define an interface for creating an object, but let the subclasses decide which class to instantiate. Factory method lets a class defer instantiation to subclasses.
* Adds a interface to the factory itself from Simple Factory
* Defers object creation to mu lt i ple factories that share an interface.
* Derived classes implement to override the factory method of base
``` csharp
    interface IAutoFactory
    {
        ICar CreateAutomobile();
    }
```
# Abstract Factory
   Provide an interface for creating families of related or dependent objects without specifying their concrete classes.
   * Factories create different types of concreate objects
   * A factory now represents a "family" of objects that it can create
   * Factories may have more than one factory method.
   
   Below creates families of cars (related)
   ``` csharp
   interface IAutoFactory
   {
       IAutomobile CreateSportsCar();
       IAutomobile CreateLuxaryCar();
       IAutomobile CreateEcomoyCar();
   }
```

