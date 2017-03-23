# Motivation
* Model a process or algorithm of several steps
* Allow variation of the details of each step, while enforcing the structure and order of the steps themserlves
* For instance, a game engine might dictate certain steps making up a variety of games
  * SetupGame()
  * TakeTurn(Player p)
  * IsGameOver()
  * DisplayWinner()
* Given this structure, specific games like T ic-Tac-Toe, Chess, Monopoly, etc could be implemented as subclasses.

# Intent
* encapsulate and enforce the workflow or process that is not variable
* Allow subclasses to alter specific behavior via concrete implementation.
* Redefine one or more steps of an algorithm without altering its structure.

# Applicability
* Two or more classes should follow the same common algorithm or workflow
* The workflow is invariant. Subclasses may define certain steps, but may not change the algorithm's structure.
* Some workflow steps may be encapsulated in the base class with a default implementation, and only overridden if necessary, allowing code reuse.

# How it gets used
* Clients call children of base implementation
* Child types customize individual step behavior
  * might change all, many, or just one step
* Effective way to achieve Open/Closed Principle.

# Consequences
* Algorithm steps must be known and relatively inflexible at the time the pattern is applied.
* Relies on inheritance, rather than composition, which can be a limitation
  *- Strategy pattern for a composition based solution
* Single inheritance makes it difficult to merge two child algorithms in to one
  * Decorator pattern for a possible solution to this problem

# Examples
* ASP.NET Web forms
* Page life cycle

# Related
* Strategy
* Decorator
* Factory
 

![structure](https://github.com/sairamaj/designpatterns/blob/master/templatemethod/structure.png)
