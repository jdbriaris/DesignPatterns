# Abstract Factory

Use the abstract factory pattern to decouple the client from the concrete creation of objects.

![](http://yuml.me/diagram/scruffy/class/[Client]-.->[Abstract Factory], [Abstract Factory]-.->[Abstract Entity], [Concrete Factory A]->[Abstract Factory], [Concrete Entity A]->[Abstract Entity], [Concrete Factory A]-.->[Concrete Entity A], [Concrete Factory B]->[Abstract Factory], [Concrete Entity B]->[Abstract Entity], [Concrete Factory B]-.->[Concrete Entity B]  "yUML") 

## When to use

Use the abstract factory when the client requires no information defined on the concrete class of an abstract entity, i.e., the abstract factory is 100% abstract. The abstract facory is limited by **contravariance**, i.e., the concrete factory will ultimately be dependent on concrete entities. This presents the following complications when using the abstract factory pattern:

- The abstract entity layer can only contain features common to **ALL** concrete entities
- Argumenets passed to the create entity method of the factory must satisfy all concrete entities
