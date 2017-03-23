# Motivation
* A class or method has complex and growing business logic
* Additional changes of the same nature are likely
* Examples
  * Customer discount calculations
  * Social gamification rules( badges/points)
  * Credit/Insurance rating

# Intent
* Separate individual rules from rules processing logic
* Allow new rules to be added without the need for changes in the rest of the system (O in SOLID)

# Applicability
* A system is suffering from conditional complexity, and additional changes of the same nature are anticipated.
* A system has comingled the concerns of choosing which action(s)  are applicable, and executing these actions.
* A system needs to support user-created logic for determining when and how to apply actions.

![structure](https://github.com/sairamaj/designpatterns/blob/master/rulespattern/structure.png)

[Rules Engine](https://msdn.microsoft.com/en-us/library/dd554919.aspx)