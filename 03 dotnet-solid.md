<details>

<summary>
#1 What is SOLID?
</summary>

<br/>

> Represents principles that help developers create more maintainable, flexible, and scalable software by promoting modularity and reducing code complexity. 

</details>

<details>

<summary>
#2 What is the full form of SOLID?
</summary>

<br/>

> SOLID represents 5 design principles:
>> S: Single Responsibility Principle
>>
>> O: Open Close Principle
>> 
>> L: LISKOV Substitution Principle
>> 
>> I: Interface Segregation Principle
>> 
>> D: Dependency Inversion

</details>

<details>

<summary>
#3 What is the goal of SOLID?
</summary>

<br/>

> To minimize dependencies thus making code easy to understand, maintain and extend.
> To minimize impact of a code change

</details>

<details>

<summary>
#4 Explain SRP with an example
</summary>

<br/>

> A class should have only one purpose and everything inside it should all be related.
> Example: Car class should not be responsible for anything about Sales so we can create a separate class about sales.

</details>

<details>

<summary>
#5 What is the benefit of SRP?
</summary>

<br/>

> Creates modular and focused classes which improves the quality of code.

</details>

<details>

<summary>
#6 Explain OCP with an example
</summary>

<br/>

> A class should be open for extension and closed for modification.

</details>

<details>

<summary>
#7 What is the benefit of OCP
</summary>

<br/>

> Minimize impact and less regression.
> By extending class, you can use the new class in areas that it's only needed.

</details>

<details>

<summary>
#8 Can you explain LISKOV Principle and its violation?
</summary>

<br/>

> Liskov principle says that child class should be able to substitute the parent class seamlessly during object polymorphism. 
> In inheritance, child class cannot remove methods of the parent. If child class do not implement any parent method, this is where the violation lies. 
> Liskov problems stems when requirements are not fully understood. 

</details>

<details>

<summary>
#9 How can we fix LISKOV Problem?
</summary>

<br/>

> Refactoring

</details>

<details>

<summary>
#10 Explain Interface Segregation Principle
</summary>

<br/>

> Code/clients should not be forced to implement methods they do not need.

</details>

<details>

<summary>
#11 Is there a connection between LISKOV and ISP?
</summary>

<br/>

> Yes and no. Yes but very thin line. No because it deals with two different issues.
> Liskov is more related to inheritance where we have grouped class in a wrong family due to which the child class is forced to implement methods it should not.
> ISP is more broad and deals with interfaces. Clients which consumes the classes, when classes are forced to implement interface methods or when classes are put in wrong family.

</details>

<details>

<summary>
#12 Define dependency inversion
</summary>

<br/>

> Higher level modules should not depend on lower level modules and both should depend on abstraction.
> If a higher level module is dependent on a lower level module -- it creates tight coupling. Any change in the lower module will impact the higher module.

</details>

<details>

<summary>
#13 What is higher level module and lower levelmodule?
</summary>

<br/>

> Module that calls the other module is termed as higher level module
> The module which gets consumed is termed as lower level module

</details>

<details>

<summary>
#14 How does dependency inversion benefit? Show with an example
</summary>

<br/>

> Any change in lower level module impacts the higher module
> Example: use an interface rather than using concrete classes

</details>

<details>

<summary>
#15 Will only dependency inversion solve decouplingproblem?
</summary>

<br/>

> No, we still need to move the object creation process outside the higher level module

</details>

<details>

<summary>
#16 Why do developers move object creation outsidehigh level module?
</summary>

<br/>

> To prevent tight coupling.

</details>

<details>

<summary>
#17 Explain IOC (Inversion of Control)
</summary>

<br/>

> We invert the object creation control outside the higher module. Just focus on what is the responsibility of the class which is connected to SRP as well.

</details>

<details>

<summary>
#18 Explain Dependency Injection with an example
</summary>

<br/>

> Dependency injection is a process where we inject dependent object from the outside.
> Combination of dependency inversion and dependency injection resolves tight coupling
> Example:
```public class Product : ProductBase {      private IDiscount discount = null;      Public Product(IDiscount _discount)      {           discount = _discount;      } } Client: Static void Main(string[] args) {      var product1 = new Product(new Discount()) }```

</details>

<details>

<summary>
#19 Is SOLID, IOC and DI design pattern or principle?
</summary>

<br/>

> SOLID is a principle
> IOC is a principle
> Dependency Injection is a technique

</details>

<details>

<summary>
#20 Is only SOLID enough for good code/architecture?
</summary>

<br/>

> No

</details>
