# Why?
* Efficient data access
* Manage concurrency problems
* Mange transactions

# Intent
* Multiple components contribute work

# Applicability
* Anytime you need data persistence
* Commonly implemented by persistence frameworks
  * ORM(NHibernate, Entity Framework) 
  * ADO.NET (DataSets & DataAdapters)

# Advantages
* Keep business logic free of data access code
* Keep business logic free from tracking changes
* Allow business logic to work with logical transactions

# Example
* .NET DataTable
* .NET ObjectContext (Entity framework)

