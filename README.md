# Factory_Design_Pattern in c#
Factory Method Design Pattern:

Factory method is a design pattern which defines an interface for creating an object but let the classes that implement the interface decide which class to instantiate.

UML Diagram
The UML class diagram for the implementation of the factory design pattern is given below:


Product: It defines the interface of objects the factory method creates.
ConcreteProduct: This is a class that implements the Product interface.
Creator: This is an abstract class & declares the factory method, which returns an object of the type Product.
ConcreteCreator: This is a class that implements the Creator class & overrides the factory method to return an instance of ConcreteProduct.

Factory Pattern Example
Assume you have three different cards which are considered here as classes MoneyBack, Titanium and Platinum, all of them implement abstract class CreditCard. You need to instantiate one of these classes, but you don't know which of them, it depends on the user. This is a perfect scenario for the Factory Method design pattern.

The classes, interfaces, and objects in the above class diagram can be identified as
Product - CreditCard
ConcreteProduct- MoneyBackCreditCard, TitaniumCreditCard, PlatinumCreditCard
Creator- CardFactory
ConcreteCreator- MoneyBackCardFactory, TitaniumCardFactory, PlatinumCardFactory
