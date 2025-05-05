<details>

<summary>
  #41 Explain Inheritance
</summary>

<br/>

> Defines a parent child relationship. Example: sedan extends car (sedan : car)

</details>

<details>

<summary>
  #42 Explain virtual keyword
</summary>

<br/>

> Helps us to define some logic in the parent class which can be overridden in the child class.

</details>

<details>

<summary>
  #43 What is overriding?
</summary>

<br/>

> Occurs when a subclass or child class provides a specific implementation for a method from the parent class that is virtual.
> BONUS QUESTION: what's the purpose of new keyword
>> New modifier's purpose in a child class is to acknowledge that the virtual method from the base class will be hidden.

</details>

<details>

<summary>
  #44 Explain overloading
</summary>

<br/>

> Same method name but different signature in the same class.

</details>

<details>

<summary>
  #45 Overloading and overriding
</summary>

<br/>

> Overloading: same method name but different signature in the same class.
> Overriding: using virtual keyword in parent and overriding it in the child class to have its own implementation.

</details>

<details>

<summary>
  #46 What is polymorphism?
</summary>

<br/>

> Ability of an object to act differently under different conditions.
> Example: Object1 is declared as a car, but in next line it will be a sedan and in next line it will be a pickup. This is due to inheritance.

</details>

<details>

<summary>
  #47 Can polymorphism work without inheritance?
</summary>

<br/>

> No

</details>

<details>

<summary>
  #48 Explain static vs dynamic polymorphism
</summary>

<br/>

> Static polymorphism = method overloading
> Dynamic polymorphism = method overriding

</details>

<details>

<summary>
  #49 Explain operator overloading
</summary>

<br/>

> Helps to redefine additional functionalities for operators (+, -, *, / etc.)
> You may create your own operator overload by using the operator keyword and implement your own logic.

</details>

<details>

<summary>
  #50 Why do we need abstract classes?
</summary>

<br/>

> Abstract class is a partially defined parent class
> Normal classes cannot create partially defined parent class
> Usage: use abstract keyword in class and property that's partially defined

</details>

<details>

<summary>
  #51 Are abstract methods virtual?
</summary>

<br/>

> Yes because abstract methods can be overridden by child classes

</details>

<details>

<summary>
  #52 Can we create an instance of an abstract class?
</summary>

<br/>

> No

</details>

<details>

<summary>
  #52 Is it compulsory to implement abstract methods?
</summary>

<br/>

> Yes, any abstract methods declared in the parent class then it should be implemented in child classes

</details>

<details>

<summary>
  #53 Why can't simple base class replace abstractclass?
</summary>

<br/>

> Because simple base classes cannot be defined partially.

</details>

<details>

<summary>
  #54 Explain interface and why do we need it?
</summary>

<br/>

> Interface is a contract, by having this contract we have better control on impact analysis, change management and breaking changes.
> All classes that inherits this interface, all properties and methods must be followed.
> Any changes to the class inheriting the interface is not possible due to this "contract" which limits issues that might impact child classes unintentionally.TLDR: better change management.
> Usage: use interface keyword and usually starts name with an I. Properties doesn’t have access modifiers and are only signatures no implementation.

</details>

<details>

<summary>
  #55 Can we write logic in an interface?
</summary>

<br/>

> No

</details>

<details>

<summary>
  #56 Can we define methods as private in interface?
</summary>

<br/>

> No all are public

</details>

<details>

<summary>
  #57 If I want to change interface what's the best practice?
</summary>

<br/>

> Create a new interface and implement multiple inheritance

</details>

<details>

<summary>
  #58 Explain Multi Inheritance in Interface
</summary>

<br/>

> Helps to add new methods (and properties?) without affecting old interfaces.
> Since you shouldn't be modifying the original interface, you can create a new interface by extending the existing one. And then, those places that needs the modification can inherit the two new interfaces. Existing ones that do not need the modification, will still work as expected.
> Typical usage: versioning; change management

</details>

<details>

<summary>
  #59 Explain Interface Segregation Principle
</summary>

<br/>

> Do not force users of the interface to use unneeded methods or properties. Interface segregation principle is the correct approach and you achieve this thru multiple inheritance in interfaces.

</details>

<details>

<summary>
  #60 Can we create an instance of an interface?
</summary>

<br/>

> No

</details>

<details>

<summary>
  #61 Can we do multiple inheritance with abstract classes?
</summary>

<br/>

> No, multiple inheritance can only be achieved through interfaces

</details>

<details>

<summary>
  #62 Abstract Class vs Interface
</summary>

<br/>

> Interface is a contract. Abstract class is a partially defined parent class.
> Interface is where you plan abstraction. Abstract class shares common logic in child classes.
> Interfaces are implemented. Abstract classes are inherited.
> Multiple inheritance can only be achieved through interfaces

</details>

<details>

<summary>
  #63 Why do we need constructors?
</summary>

<br/>

> A constructor is a special method of a class which gets automatically invoked whenever an instance of that class is created.
> Constructors are used to initialize things, assign default values etc.

</details>

<details>

<summary>
  #64 In parent child which constructor fires first?
</summary>

<br/>

> Parent

</details>

<details>

<summary>
  #65 How are initializers executed?
</summary>

<br/>

> Child initializers run first, then parent, then parent constructors, then child constructors

</details>

<details>

<summary>
  #66 How are static constructors executed in parent child?
</summary>

<br/>

> Child static constructor runs, parent static constructor

</details>

<details>

<summary>
  #67 When does static constructor fires?
</summary>

<br/>

> When you access the class for the first time

</details>

<details>

<summary>
  #68 What is shadowing?
</summary>

<br/>

> Is a process where child functions or properties will be hidden from the parent during polymorphism.
> Replace override with new keyword in child class

</details>

<details>

<summary>
  #69 Explain method hiding
</summary>

<br/>

> It's a C# Parlance (specific word) equivalent to Shadowing of VB.

</details>

<details>

<summary>
  #70 Shadowing vs overriding
</summary>

<br/>

> Overriding occurs when a subclass or child class provides a specific implementation for a method from the parent class that is virtual.
> Shadowing occurs when the child functions or properties will be hidden from the parent during polymorphism.

</details>

<details>

<summary>
  #71 When should you use shadowing?
</summary>

<br/>

> Shadowing is a reactive measure which developers implement when the child classes do not implement all the methods of the parent.
> This is also termed as LISKOV problem and it happens due to wrong abstraction

</details>

<details>

<summary>
  #72 Explain sealed classes
</summary>

<br/>

> Sealed class is a class which cannot be inherited any further.

</details>

<details>

<summary>
  #73 Can we create instance of a sealed class?
</summary>

<br/>

> Yes

</details>

<details>

<summary>
  #74 What are nested classes and when to use them?
</summary>

<br/>

> Nested class is a class within a class
> For logically grouping classes especially used when creating private class inside the implementing class.

</details>

<details>

<summary>
  #75 Can nested class access outer class variables?
</summary>

<br/>

> No you cannot access it directly, you have to pass via instance

</details>

<details>

<summary>
  #76 Can we have public, protected access modifiers innested class?
</summary>

<br/>

> Technically yes but should be logically correct

</details>

<details>

<summary>
  #77 Explain partial classes
</summary>

<br/>

> Classes that can be written in two different physical files but during compile it compiles to only one class.

</details>

<details>

<summary>
  #78 In what scenarios do we use partial classes?
</summary>

<br/>

> Code generation and rapid application development
> To organize complex code into different files

</details>
