<details>

<summary>#1 Difference between .net and c#</summary>

<br/>

> .Net is a framework and c# is a programming language

> C# is composed of syntaxes, grammars, semantics, etc.

> .Net is collection of libraries and it has runtime

</details>

<details>

<summary>#2 Differentiate between .net framework, .net core and .net 8.0</summary>

<br/>

.Net framework runs only on Windows
.Net Core is cross platform
.Net 8.0 provides a unified experience

Performance: .Net framework is slower compared to .Net core. One of the main reasons are the libraries that were broken down to smaller parts in .net core that allows users to only select those that are needed rather than importing a whole chunk of a library.

CLI (Command Line Interface) Support: .Net Core supports Full CLI while .Net Framework is more IDE based which means more flexibility in .Net Core.

Microservice support: .Net Framework No - .Net Core Yes

Mobile Compatibility: .Net Framework No - .Net Core Xamarin

Packaging: .Net Framework packaged as one big framework while .Net core are delivered via modules using Nuget.

</details>

<details>

<summary>
  #3 What is IL (Intermediate Language) Code?
</summary>

<br/>

> Partially compiled code that served as an intermediate language between your .net human readable code to machine language with use of JIT

</details>

<details>

<summary>
  #4 What is the use of JIT (Just In Time) Compiler?
</summary>

<br/>

> Compiles Intermediate Language and converts it to Machine Language

</details>

<details>

<summary>
  #5 Is it possible to view IL Code?
</summary>

<br/>

> Yes by using disassembler apps

</details>

<details>

<summary>
  #6 What is the benefit of compiling in to IL Code?
</summary>

<br/>

> The runtime environment and development environment can be very different so depending on the runtime environment JIT compiles the best optimized code as per that environment.

</details>

<details>

<summary>
  #7 Does .Net support multiple programming languages?
</summary>

<br/>

> Yes it supports multiple language, C#, VB, JS, TS, etc. but at the end of the day it will still be compiled into IL.

</details>

<details>

<summary>
  #8 What is CLR or Common Language Runtime?
</summary>

<br/>

> It does a lot of things but two of the most important things are to invoke JIT to compile IL code into native/machine language AND runs your application while ensuring it cleans any unused objects by using garbage collector.

</details>

<details>

<summary>
  #9 What is managed and unmanaged code?
</summary>

<br/>

> All code that runs under CLR is managed code. C or C++ code that have their own compiler and environment outside CLR are unmanaged code.

</details>

<details>

<summary>
  #10 Explain the importance of Garbage Collector?
</summary>

<br/>

> Garbage Collector is a background process which cleans unused managed resources.

</details>

<details>

<summary>
  #11 Can garbage collector claim unmanaged objects?
</summary>

<br/>

> No

</details>

<details>

<summary>
  #12 Explain the importance of CTS or Common Types System
</summary>

<br/>

> CTS ensures that data types defined in two different languages get compiled to a common data type.

</details>

<details>

<summary>
  #13 Explain CLS or Common Language Specifications
</summary>

<br/>

> CLS is a specification or set of rules or guidelines. When any .Net programming language adheres to these set of rules it can be consumed by any language following .Net Specifications.

</details>

<details>

<summary>
  #14 Difference between Stack and Heap?
</summary>

<br/>

> Stack memory is used for static memory allocations such as local variables within functions. Heap memory is used for dynamic memory allocation, suitable for objects or data whose size might change at runtime or whose lifetime exceeds the scope of a single function call.

</details>

<details>

<summary>
  #15 What are value types and reference types?
</summary>

<br/>

> Value types contain actual data while reference types contain pointers that point to the actual data.
> Value types are stored in stack while reference types are stored in heap.

</details>

<details>

<summary>
  #16 Boxing vs unboxing
</summary>

<br/>

> When value type is moved to a reference type it's called boxing.

</details>

<details>

<summary>
  #17 Consequence of boxing and unboxing
</summary>

<br/>

> Performance

</details>

<details>

<summary>
  #18 Casting, implicit casting and explicit casting
</summary>

<br/>

> Casting is a mechanism where we convert one type of data to other type.
> Implicit casting is when you move from lower to higher data type
> Explicit casting is when you move from higher to lower data type

</details>

<details>

<summary>
  #19 What can happen during explicit casting?
</summary>

<br/>

> Data loss

</details>

<details>

<summary>
  #20 Array vs ArrayList
</summary>

<br/>

> Arrays are strongly typed and has fixed length. ArrayList is flexible in terms of length and is not strongly typed.

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>

</details>

<details>

<summary>
  
</summary>

<br/>

> 

</details>
