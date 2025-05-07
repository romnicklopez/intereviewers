<details>

<summary>
#1 What are design patterns?
</summary>

<br/>

> Design Patterns are time tested solutions for recurring architectural problems.

</details>

<details>

<summary>
#2 What are the different types of design patterns?
</summary>

<br/>

> 3 Categories of Design Pattern:
>
> Creational
> 
>> Prototype
>> 
>> Singleton
>> 
> Behavioral
> 
>> Chain of responsibility
>>
>> Command
>>
>> Mediator
>>
>> Memento
>>
>> Template Method
>>
> Structural
> 
>> Adapter
>>
>> Composite
>>
>> Decorator

</details>

<details>

<summary>
#3 Explain Structural, Behavioral and Creational design pattern
</summary>

<br/>

> Creational: problems and solutions around object creation issues
>
>> Prototype Pattern: a fully initialized instance to be copied or cloned
>>
>>> Example: implementing this.clone
>>> 
>>> Usage: resolves the issue of using new keyword in cases when you need to have a record of the class being overwritten
>>>
> Behavioral: problems and solutions around communication between objects
>
>> Template Method: defer the exact steps of an algorithm to a subclass
>>
>>> Example: Parent class: createFile; Sub classes: createDoc, createCSV, createPdf --- these subclasses override specific steps of the algorithm without changing its structure
>>>
>>> Usage: when you want to let clients extend only particular steps of an algorithm but not the whole algorithm or its structure.
>>>
> Structural: solving concerns around class structure and object composition
>
>> Adapter Pattern: match interfaces of different classes:
>>
>>> Example: implementing different method implementation in an inherited class
>>>
>>> Usage: implement different export method per file type, suddenly all MS Office files are okay but suddenly PDF is not supported due to license issues which forced you to change library. Adapter Pattern helped in this case since you've created a same interface for all file types, then you can do changes only in the PDF class. 

</details>

<details>

<summary>
#4 Explain Singleton Pattern and its use
</summary>

<br/>

> Singleton Pattern helps create a single instance of an object
>
> Usage:
>
>> Caching of data like countries, states, currencies, languages etc.
>>
>> Global sharing of data like common themes, hit counters, etc.

</details>

<details>

<summary>
#5 How do youimplement Singleton Pattern?
</summary>

<br/>

> Step 1: Create a single wrapper class. Instance of that class will be created inside the class itself.
>
> Step 2: Implement thread safety
>
> Step 3: Private constructor
>
> Step 4: Lazy loading
>
> Step 5: Double NULL check Step 6: Lock performance

</details>
