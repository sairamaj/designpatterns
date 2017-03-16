# Overview
Behaviorial

Also known as __Cursor__

## Motivation
* Yo work with a variety of collection types
* Yo want to be able to traverse various kinds of collections without knowing about their internal structures.
* You don't want to bloat every collection's interface with traversal operations
* The __iterator pattern__ describes a way to access collection's members sequentially without violating encapsulations or SRP

## Intent
* Provide a way to access the elements of an aggregate object sequentially without exposing its underlying representation
* The __iterator pattern__ defines interfaces for the aggregate and the __iterator__, each of which must be implemented for each collection that is to support the pattern.

## Applicability
* you need to traverse a collection
* you want to abstract the collection iteration logic
* * Follow SRP and DRY
* you do not wish to break encapsulation and expose your collections internal organization/design globally

![structure](https://github.com/sairamaj/designpatterns/blob/master/iterator/structure.png)

#.NET examples
IEnumerable ( aggregate interface)
IEnumerator ( iterator interface)

 