# Javascript

Console: the console is the panel that displays important messages, like errors, for developers. 
- in javascript the console keyword refers to an object, or collection of data and actions. 

#### Comments
- //: 'single line comment' will comment out a single line
- /**/: 'multi-line comment' will comment out multiple lines

#### Data Types
- Number: any number (including number with decimal)
- String: any grouping of characters sourrounded by single quotes '...', or double quotes "..."
- Boolean: either true or false (yes or no) reprerented `true` or `false`
- Null: intentional absence of a value represented `null`
- Undefined: represents the absence of a value (given value does not exist) denoted by keyword `undefined`
- Object: collections of related data 

#### Arithmetic Operators
- Add: +
- Subtract: -
- Multiply: *
- Divide: /
- Remainder: %

#### Properties
- .length: stores the number of characters in the string

#### Methods
- methods are actions we can perform

[Javascript Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/prototype)

#### Built-In Objects
[Objects built into javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects)

- Math.random: generate random number
- Math.floor: takes decimal number and rounds down to nearest whole number

[Properties and methods on Math Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)

REVIEW
- Data is printed, or logged, to the console, a panel that displays messages, with console.log().
- We can write single-line comments with // and multi-line comments between /* and */.
- There are 7 fundemental data types in javascript: strings, numbers, booleans, null, undefined, symbol, and object.
    - Numbers are any number without quotes
    - Strings are characters wrapped in single or double quotes
- The built in arithmetic operators include +, -, *, /, %
- Objects, including instances of data types, can have properties, stored information (denoted with a . after the name of the object)
    -objects, including instances of data types, can have methods which perform actions. 
    - methods are called by appending the object or instance with a period, the method name, and parentheses
    - we can access properties and methods by using the ., dot operator
- Built in objects, including Math, are collections of methods and properties that javascript provides
-------------------------------------------------------------------
## 1. Variables: implement Javascript Data types, built-in methods, and variables

REVIEW
- variables hold reusable data in a program and associate it with a name
- variables are stored in memory
- the var keyword is used pre-ES6 version of JS
- let is the preferred way to declare a variable when it can be reassigned, and const is preferred way to declare a variable with a constant value
- variables that have not been initialized store the primitive data type undefined
- mathematical assignment operators make it east to calculate a new value and assign it to the same variable
- the + operator is used to concatenate strings including string value held in variables
- template literals use `` and ${} to interpolate values into a string
- the typeof keyword return the data type (as a string) of value
  

-------------------------------------------------------------------
## 2. Conditionals: use conditionals to control the flow of a program in javascript

### 2.1 Conditional Statements

REVIEW
- an if statement checks a condition and will execute a task if that condition evaluates to true
- if...else statements make binary decisions and execute different code blocks based on a provided condition
- we can add more conditions using else if statement
- comparison operators, including <, >, <=, >=, ===, and !== can compare two values
- the logical and operator, &&, or "and", checks if both provided expressions are truthy
- the logical operator ||, or "or", checks if either provided expression is truthy
- the bang operator, !, switches the truthieness and falsiness of a value
- the ternary operator is shorthand to simplify concise if...else statement
- a swith statement can be used to simplify the process of writing multiple else if statements. The break keyword stops the remaining case's from being checked and executed in a switch statement

-------------------------------------------------------------------
## 3. Functions: construct functions and pass data through them 

REVIEW
- a function is a reusable block of code that groups together a sequence of statements to perform a specific task
- a function decloration
    
    
           function greetWorld( {
              console.log("Hello, World");
           }
           
           
        KEY
          Function body
          

- a parameter is a named variable inside a function's block which will be assigned the value of the argument passed in when the function is invoked

            function calculateArea( width, height) {
               console.log(width * height);
            }
            
- to call a function in your code
            greetWorld();
        
- handle arbitrary parameters through default parameters which allow us to assign a default value to a parameter in case no argument is passed into the function
- to return a value from a function, we use a return statement
- to define a function using function espression

            const calculateArea = function(width, height) {
               const area = width * height;
               return area;
            }
- to define a function using function notation

            const calculateArea = (width, height) => {
               const area = width * height;
               return area;
            }
            
- function definition can be made concise using concise arrow notation

            SINGLE LINE BLOCK
            const addNumbers = number => number + number;
            
            MILTI LINE BLOCK
            const addNumbers = number => {
               const num = number + number;
               return num; RETURN STATEMENT
            }
    

-------------------------------------------------------------------
## 4. Scope: identify global and block-level scopes in javascript

REVIW
- scope: refers to where variables can be accessed throughout the program, and is determined by where and how they are declared
- blocks: are statements that exist within curly braces {}
- global scope: refers to the context within which variables are accessible to every part of the program
- gobal variables: variables that exist within global scope
- block scope: refers to the context within which variables are accessible only within the block they are defined
- local variables: variables that exist within block scope
- global namespace: the space in our code that contains globally scoped information
- scope pollution: when too many variables exist in a namespace or variable names are reused

-------------------------------------------------------------------
## 5. Array: use arrays to store lists of data

REVIEW
- arrays are lists that store data in JavaScript
- arrays are created with brackets []
- each item inside of an array is at a numbered position, or index, starting at 0
- we can access one item in an array using its index, with syntax like: myArray[0]
- we can also change an item in an array using its index, with syntax like myArray[0] = 'new string';
- arrays have a length property, which allows you to see how many items are in an array
- arrays have their own methods, including .push() and .pop(), which add and remove items from an array respectively
- arrays have many methods that perform different tasks, such as .slice() and .shift, [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
- some built-in methods are mutating, meaning the method will change the array, while others are not mutating.
- variables that contain arrays can be declared with let or const. Even when declaed with const, arrays are still mutable. However, a variable declared with const cannot be reassigned
- arrays mutated inside of a function will keep that changeeven outside the function 
- arrays can be nested inside other arrays
- to access elements in nested arrays chain indices using bracket notation

-------------------------------------------------------------------
## 6. Loops: use loops to execute blocks of code multiple times

REVIEW
- loops perform repetitive actions so we dont have to code that process manually every time
- how to write for loops with an iterator variable that increments or decrements
- use for loop to iterate through an array
- a nested for loop is a loop inside another loop
- while loops allow for different types of stoping conditions
- stopping conditions are crucial for avaoiding infinite loops
- do...while loops run code at least once - only checking the stopping condition after the first execution
- the break keyword allows programs to leave a loop during the execution of its block


-------------------------------------------------------------------
## 7. Iterators: use iterator methods to simplify the process of looping over arrays

### 7.1 High Order Functions

REVIEW
- abstruction allows us to write complicated code in a way thats easy to reuse, debug, and understand for human readers. 
- we can work with functions the same way we work with any other type of data, including reassigning them to new variables
- javascript functions are first-class objects, so they have properties and methods like any other object
- functions can be passed into other functions as parameters
- a high-order function is a function that either accepts functions as parameters, return a function, or both

### 7.2 Iteraters

REVIEW
- .forEach() is used to execute the same code on every element in an array but does not change the array and returns undefined
- .map() executes the same code on every element in an array and returns a new array with the updated elements
- .filter() checks every element in an array to see if it meets certain criteria and returns a new array with the elements that return truthy for the criteria
- .findIndex() returns the index of the first element of an array that satisfies a condition in the callback function. It returns -1 if none of the elements in the array satisfies the condition
- .reduce() iterates through an array and takes values of the elements and returns a single value
- all iterator methods take a callback function, which can be a pre-defined function expression, or an arrow function
[Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

-------------------------------------------------------------------
## 8. Objects: use javascript ES6 object syntax to meodel real-world items

### 8.1 Objects

REVIEW
- objects store collections of key-value pairs
- each value pair is a property-when a property is a function it is known as a method
- an object literal is composed of comma-seperated key-value pairs surrounded by curly braces
- you can access, add or edit a property within an object by using dot notation or bracket notation
- we can add methods to our object literals using key-value syntax with anonymous function expressions as values or by using the new ES6 method syntax
- we can navigate complex, nested objects by chaining operators
- objects are mutable- we can change their properties even when they are declared with const
- objects are passed by reference- when we make changes to an object passed into a function, those changes are permanent
- we can iterate through objects using the For...in syntax

### 8.2 Advanced Objects

REVIEW
- the object that a method belongs to is caled the calling object
- the this keyword refers to the calling object and can be used to access properties of the calling object
- methods do not automatically have access to other internal properties of the calling object
- the calue of this depends on where the this is being accessed from
- we cannot use arrow functions as methods if we want to access other internal properties
- javascript objects do not have built-in privacy, rather there are conventions to follow to notify other developers about the intent of the code
- the usage of an underscore before a property name means the origional developer did not intend for the property to be directly changed
- setters and getter methods allow for more detailed ways of accessing and assigning properties
- factory functions allow us to create object instances quickly and repeatedly
- there are different ways to use object destructing: one way is the property value shorthand and another is destructured assignment


