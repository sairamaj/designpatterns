Known as wrapper

Intent
   - Convert the interface of a class in to another interface client expect
   - Allow classes to work together that couldn't otherwise due to incompatible interfaces.
   - Future-proff client implementations by having them depend on adapter interfaces, rather than concrete classes directly.	
Applicability
   - You want to use an existing class, but its interface does not match the one you require
   - you need to use several existing subclasses, but it's impractical to adapt their interface by subclassing every one.
How it gets Used
   - Client dpeend on the adapter interface, rather than a particular implementation
   - Atleast one concret adapter class is created to allow the client to work with a particular clas that it requires.
   - Future lcient needs for alternatie implementations can be satisfied through the creation of additional concrete adapter classes.
   - Effective way to achieve Open/Closed Principle.
Collaboration
   - Client call operations on an Adapter instance
   - Adapte rinstance calls Adaptee operations that carry out the request.
Examples
    - IDataAdapter
          DbDataAdapter
              	- OdbcDataAdapter
	      	- OleDbDataAdapter
	    	- SqlClientDataAdapter
Related
    - Repository
    - Strategy
    - Facade (Adapter and Facade are both wrappers). The facade pattern attempts to simplify the interface and often wraps many classes, while the Adapter typically wraps a single Adaptee, and is not generally concerned with simplifying the interface ( both client and interfacs are fixed and just works in the middle.)
Open/Closed Principle:
    Modules should be open to extension ,but closed to modification
    
