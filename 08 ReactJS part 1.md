<details>

<summary>
#1 What is React and what is its role in software development?
</summary>

<br/>

> React is an open source JS library for building UI and simplifies the creation of SPA by using reusable components

</details>

<details>

<summary>
#2 What are the key features of React?
</summary>

<br/>

> Virtual DOM
>
>> visual representation of DOM, allowing efficient updates by minimizing direct manipulation of actual DOM resulting in improved performance
>> 
> Component based architecture
>
>> modular and reusable components promotes a more maintainable and scalable approach to building applications
>> 
> Reusability and composition
>
>> creation of reusable components that can be composed together fostering modular and efficient development process
>>
> JSX or JavaScript XML
>
>> syntax extension for JS used in React that allows developers to write HTML-like code with JS, enhancing readability and maintainability
>> 
> Declarative Syntax
>
>> JSX lets developers focus on what the UI should look like and React handles the how behind the scene hence simplifying the code
>> 
> Community and ecosystem
>
>> vibrant and extensive community that contributes to a rich ecosystem of libraries, tools and resources fostering collaboration and innovation
>> 
> React Hooks
>
>> functions that enable functional components to manage state and lifecycle features, proving a more concise and expressive way to handle component logic
>> 

</details>

<details>

<summary>
#3 What is DOM? What is the difference between HTML and DOM?
</summary>

<br/>

> DOM or Document Object Model represents the web page as a tree-like structure which allows JS to dynamically access and manipulate the content and structure of a web page
>
> HTML is a markup language responsible for the UI
> 

</details>

<details>

<summary>
#4 What is Virtual DOM? Difference between DOM and Virtual DOM?
</summary>

<br/>

> Virtual DOM is used only in React and is an exact copy of the actual DOM
>
> Virtual DOM solves the problem of the actual DOM that when something gets updated, the whole DOM/page re-renders
>
> React is responsible for these updates using the virtual DOM and is also responsible for reconciling the virtual DOM with the actual DOM
> 

</details>

<details>

<summary>
#5 What are React Components? What are the main elements of it?
</summary>

<br/>

> Components are the reusable building blocks of React for creating UI
> 
> Elements: import, function(class) with a JSX return and export
> 

</details>

<details>

<summary>
#6 What is SPA or Single Page Application?
</summary>

<br/>

> A web application that has only one single web page
>
> It is a concept that allows updating of the content of the page without reloading and re-rendering the whole page
> 

</details>

<details>

<summary>
#7 What are the 5 advantages of React?
</summary>

<br/>

> Simple to build SPA using reusable components
>
> Cross platform and open source
>
> Lightweight and very fast because of virtual DOM
>
> Large community and ecosystem
>
> Testing is easy
> 

</details>

<details>

<summary>
#8 What are the disadvantages of React?
</summary>

<br/>

> React is not a good choice for a very small application with a lot of static contents
> 

</details>

<details>

<summary>
#9 What is the role of JSX in React?
</summary>

<br/>

> JSX or JavaScript XML is used by React to write HTML-like code which will then be converted to JavaScript via libraries like Babel

</details>

<details>

<summary>
#10 What is the difference between Declarative and Imperative syntax?
</summary>

<br/>

> Declarative syntax focuses on describing the desired result without specifying the step by step process
>
> Imperative syntax involves step by step process to achieve a goal
>
> JSX is declarative; JS is imperative
>

</details>

<details>

<summary>
#11 What is Arrow Function Expression in JSX?
</summary>

<br/>

> It is an expression syntax that's a concise way of defining functions
>
> Compared to regular function declaration, it assigns the function to a variable and uses the arrow operator
> 

</details>

<details>

<summary>
#12 How to set up React's first project?
</summary>

<br/>

> Install Node
>
> Install Code Editor like VS Code
>
> npx create-react-app
>
> nameOfTheApp npm start
> 

</details>

<details>

<summary>
#13 What are the Main Files in a React Project?
</summary>

<br/>

> index.html
>
> components
>
> App.js
>
> index.js
>
> App.test.js (optional)
>
> Index.css (optional)
> 

</details>

<details>

<summary>
#14 How React App Load and display the components in the browser?
</summary>

<br/>

> Request/Response <-> index.html <-> index.js <-> App.js
> 

</details>

<details>

<summary>
#15 React vs Angular
</summary>

<br/>

> Similarity: both are used to create SPA applications using components
>
> Differences:
>
>> React is a JS library while Angular is a complete framework
>>
>> React uses virtual DOM while Angular uses the real DOM
>>
>> React is lightweight compared to Angular
>>
>> React depends on external libraries since it's not a complete framework compared to Angular
>> 

</details>

<details>

<summary>
#16 What are other JS Frameworks other than React?
</summary>

<br/>

> Angular, Vue, Backbone, Ember, Svelte, Flutter
> 

</details>

<details>

<summary>
#17 Whether React is a Framework or a Library - what is the difference?
</summary>

<br/>

> Given that React is a library it has limitations and depends on other libraries to fulfill specific requirements compared to Angular which is a framework which has all the basics
> 

</details>

<details>

<summary>
#18 How React provides Reusability and Composition?
</summary>

<br/>

> Once you create a component, it can be reused in multiple places even projects
>
> Composition is creating new and big components by combining existing small components - allows separation of concerns between components
> 

</details>

<details>

<summary>
#19 What are State, Stateless, Stateful and State Management terms?
</summary>

<br/>

> State refers to the current data of the component
>
> Stateful means when a user performs some actions in the UI, application should be able to update and re-render that state otherwise it is stateless
>
> State management - achieved through hooks, redux and other libraries
> 

</details>

<details>

<summary>
#20 What are Props in JSX?
</summary>

<br/>

> Way to pass data from one component to another.
> 

</details>

<details>

<summary>
#21 What is NPM? What is the role of the node_modules folder?
</summary>

<br/>

> NPM or Node Package Manager is used to manage dependencies for your React project including the React library itself
>
> node_modules folder holds all the dependency libraries
> 

</details>

<details>

<summary>
#22 What is the role of a public folder in React?
</summary>

<br/>

> Holds static files like images, favicon, icons etc. and index.html

</details>

<details>

<summary>
#23 What is the role of the src folder in React?
</summary>

<br/>

> Used to store all source code of the application.

</details>

<details>

<summary>
#24 What is the role of the index.html page in React?
</summary>

<br/>

> Index.html is the main SPA page/html file
>
> The component in the index.js file that holds the application logic will replace the root div in index.html
> 

</details>

<details>

<summary>
#25 What is the role of the index.js file and ReactDOM in React?
</summary>

<br/>

> ReactDOM is a JS library that renders components to the DOM or browser
>
> index.js file is the JS file that replaces the root element of the index.html file with the newly rendered components
> 

</details>
