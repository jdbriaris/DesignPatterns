## Decorator

>Attach additional responsibilities to an object dynamically. Decorators provide a flexible alternative to subclassing for extending functionality.

![](http://yuml.me/diagram/scruffy/class/[Component|+Operation()]-^[ConcreteComponent|+Operation()],[Component|+Operation()]^-[Decorator],[Decorator|Operation()]+->[Component|+Operation()],[Decorator|Operation()]^-[ConcreteDecoratorA|-addedState|+Operation()],[Decorator|Operation()]^-[ConcreteDecoratorB|-addedState|+Operation();+AddedBehaviour()] "yUML")
