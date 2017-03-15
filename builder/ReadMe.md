# Overview
* Creational
* Separates the construction of a complex object from its representation so that same construction process can create different representations.
* construction is _process_ and representation is _data_  (separating logic and data)
[gist: reuse logic to work with different set of data to build the same thing and only difference is the data]
[some example is building a sandwich at a subway ]
* Too many parameters
* Order dependent
* Different constructions
  
![builder](https://github.com/sairamaj/designpatterns/blob/master/builder/builder.png)
## Director
* Uses the concrete builder
* knows ho to build
* client code calls directly

## Builder
* Abstract interface or class
* Define steps
* Holds instance of _product_

## Concrete Builder
* Should be more than one of these
* Provides an implementation for interface defined by the Builder
* A recipe

## Product
* What is being built
* Not a different type, but different data

## 
## Examples
 StringBuilder, FluentAPI is not builder patterns ( no element of patterns exists here.)
