# OOP Principles

Below is some important principles to keep in mind when developing object-orientated code.

## SOLID

### Single responsibility

> A class should have one and only one reason to change, meaning a class should have only one job.

### Open-closed principle

> Classes should be open for extension, but closed for modification.

### Liskov substitution principle

> Classes that hold references to base classes, should be able to use derived classes for those references.

### Interface segregation

> A class should never be forced to implement an interface it never uses

### Dependency inversion

> High-level classes should not depend on low-level classes. Both should depend on abstractions.

## Constructing Classes

### Make invalid states non-representable

> Classes should have all the necessary information to exist in a valid state immediately after construction. A class should **not** be in a state after contruction that may lead to consumers of that class experiencing unexpected behaviour.

Enforce this by:
- Ensuring the contructor is defined with required parameters that contain all information the class needs to be valid
- Implementing guard clauses in the constructor that will throw if insufficient information is provided

## Postel's Law

> Be consevative in what you do, be liberal in what you accept from others.

The original context for Postel's law was the interaction of devices over networks ([link](https://tools.ietf.org/html/rfc761)). It has direct application during the construction and consumption of software services, i.e., *as designers of client software we should try our best to allow the service being consumed to change without requiring us to change.*
