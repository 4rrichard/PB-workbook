# Programming Basics questions

## Data Basics

- What are the differences between objects, arrays, and primitives in JavaScript? How are they used in programming?- How would you access the value of a specific key in an object?

### Objects: stores key value pairs, keys are unique

### Arrays: stores values, each value has an index

### Primitives: different single values

### Accessing the value of a specific key: with the dot notation e.g. cat.name or cat["name"]

- Explain the concept of key-value pairs in objects and how they differ from indexed elements in arrays.

### you can find a specific value with the unique keys in objects, in arrays each element is ordered so they can be found through their indexes(e.g. used for lists)

- Describe a scenario where you would choose to use an object instead of an array, or vice versa, and explain your reasoning.

### Arrays: when I store similar values like strings, numbers where the order of the elements can be important

### Objects: used to represent real world concept: like storing a data of a person or a product

- How can you retrieve the first and last items of an array?

### first: array[0], last: array[array.length - 1]

- Identify the five most commonly used primitive types in JavaScript, and provide examples demonstrating when and how to use them?

### five primitives: string, number, boolean, null, undefined

### string: e.g. providing text based value

### number: calculations

### boolean: e.g. comparing 2 numbers if their value is the same

### null: when a value is intentionally set to have no value

### undefined: e.g. when a function has no return value

## Algorithm Basics

- Provide examples of assignment operators in JavaScript.

### =,+=,-=,,\*=,/=

- Name some of the arithmetic operators in JavaScript.

### +, - , \*, /, %, \*\*

- What are the different comparison operators in JavaScript?

### ===, ==, !==, !=, <,>,>=,<=

- Name a few logical operators used in JavaScript.

### &&,||, !

- Explain the differences between a `for` loop, `for of` loop, and `for in` loop in JavaScript.

### for loop: mainly used when the index of an element is important

### for of loop: where the order is not important just the values of the array

### for in loop:mainly used on objects, to identify the key value pairs(iterating over the keys)

- If you can't use any built-in functions or methods, how would you calculate the average of values in an array?

### create a let variable outside of the for loop with value of 0, then add each number to it from the for loop with the += assignment operator, then divide that final value with the length of the array

## Function Basics

- What is a function in JavaScript? Explain its purpose and how it is used in programming.

### A function in JavaScript is a reusable block of code designed to perform a specific task. Functions take inputs (parameters), process them, and can return an output (result). They help make code modular, reusable, and easier to manage.

- Describe the different syntax elements that make up a JavaScript function.

### function keyword: Marks the beginning of a function declaration.

### Function name: The name of the function (e.g., myFunction).

### Parameters (optional): Variables passed into the function (e.g., (param1, param2)).

### Function body: The block of code that defines the function's behavior.

### Return (optional): Sends a result back from the function to where it was called.

- How do you pass arguments to a function? Explain the concept of parameter passing and provide an example.

### we need to call the function outside of the function: cats(), then add the argument that we want to pass into the function: cats("Kitty"), after that in the function parameter naming the incoming value with something descriptive in this case function(catName), so we can use the incoming value inside the function referring to the parameter name from now on

- What is the difference between function expressions and function declarations? Provide examples of each.

### function declaration is a named function using the function keyword: function cat(){}

### function expression is a function assigned to a variable, here the function can be anonymous or named

- Explain what a callback function is in JavaScript.

### when we call a function inside of an other function passed as an argument, used to handle tasks that take more time(loading data), make functions reusable

- What is the scope of variables in JavaScript functions? Explain the difference between local and global variables.

### global variables can be accessed from local scopes like from inside of a function or a for loop, in the local scope you can only access the values that were declared inside the function or loop inside of them and other functions can reach them unless the value is passed to them as an argument from within the function

## Built-in Features

- What are some commonly used built-in functions or methods in JavaScript for working with strings? Provide examples and explain their usage.

### toString(): converts the data into a string, e.g (4).toString() = "4"

### toLowerCase(): converts the string into lowercase letters e.g (CAT).toLowerCase() = cat

### toUpperCase(): converts the string into uppercase letters e.g (cat).toUpperCase() = CAT

### slice(): can be used to extract a section of a string e.g. "cat".slice(0,1) = "at"

### replace(): replaces a part of a string to an other string e.g. "cat army".replace("cat", "dog") = "dog army"

- Name at least five built-in functions or methods in JavaScript for manipulating arrays. Describe how each function/method works and provide an example for each.

const arr = [2, 3, 4]

### map() : modifies each element with the same condition given(new array created) arr.map(el => el + 1) = [3,4,5]

### filter() : filters all elements that match the given condition(new array )arr.filter(el => el >=3) = [3,4]

### reduce() : reduces the array to a single value by applying a function to each element arr.reduce((total,currVal)=> total + currVal) = 9

### includes() : checks if a specific value can be found inside of an array(true or false) arr.includes(2) = true

### concat() : merges 2 arrays into a new array arr.concat([5,6,7]) = [2,3,4,5,6,7]

### sort(): sorts an array according to the given condition(modifies original array) arr.sort((a,b)=>b-a) = [4,3,2]

- How can you use built-in functions or methods in JavaScript to perform mathematical operations? Give examples of commonly used functions or methods for mathematical calculations.

### Math.min()

### Math.max()

### Math.random()

### Math.floor()

### Math.ceil()

- What are some built-in functions or methods in JavaScript for manipulating numbers? Describe their functionality and give examples of how they can be used.

### Math.abs()

### Math.floor()

### Math.ceil()

### Number.isInteger()

### Number.parseFloat()

### Number.parseInt()

- Discuss the differences between `for` loops and the `forEach` method in JavaScript.

### for loop for more control over iteration

### for each for easier readability and simpler tasks

## File Basics

- What distinguishes JavaScript data structures from JSON data structures?

### JavaScript Data Structures: These are built-in structures like arrays, objects, sets, and maps used to store and manipulate data within JavaScript programs.

### JSON Data Structures: JSON is a text-based data format used for representing and exchanging data, supporting only basic types like strings, numbers, and objects.

- How would you create a JavaScript data structure from the data in a JSON file?

### JSON.parse() to convert the JSON data (which is a string) into a usable JavaScript object or array

## View Basics

- Explain the difference between JavaScript object data structure and DOM data structure.

### JavaScript Object: A collection of key-value pairs used to store and organize data.

### DOM: A tree-like structure representing the HTML document that allows you to interact with and manipulate the elements on the page.

- What are the necessary steps to change the content of an HTML element using JavaScript?

### 1. Select the element using methods like getElementById(), querySelector(), etc.

### 2. Change the content using properties like textContent, innerHTML, or value.

## Event Basics

- Define an event listener in JavaScript.

### Event Listener: You define an event listener using addEventListener() to listen for an event (e.g., click) on an element.

- Outline the steps involved in changing the content of an HTML element when it is clicked.

### Changing Content: Inside the event listener function, you can change the content of the element (e.g., using textContent or value).

- Inside a `click` event listener, how can you access the element that was clicked?

### Accessing Clicked Element: Inside the click event listener, you can access the element that was clicked using event.target.

## Design Basics

- What are the differences between `display: block`, `display: inline`, and `display: inline-block` in CSS? When would you use each display property, and how do they affect the layout and behavior of elements?

### block: For creating sections or elements that need to span the full width.

### inline: For elements that should flow inline with text or other elements without breaking lines.

### inline-block: For elements that need inline behavior but require dimension control (like buttons in a navigation bar).

- Explain the distinctions between `position: relative` and `position: absolute` CSS properties.

### position: relative: Positions the element relative to its normal position in the document flow, allowing movement with top, left, right, and bottom while keeping its space in the layout.

### position: absolute: Positions the element relative to its nearest positioned ancestor (or the viewport if no ancestor is positioned), removing it from the document flow and not affecting the layout of other elements.

- What is the box model? Name the CSS properties associated with it.

### Content is what you see (text, images).

### Padding is the inner space around the content.

### Border surrounds the padding.

### Margin is the outer space, pushing elements apart.

- Identify the CSS properties that affect font and text appearance.

### font-size

### font-weight

### font-style

### font-family

### line-height

### text-transform

### letter-spacing

### text-align

### text-decoration

### color

- List the steps for adding or removing a class name from an HTML element.

### classList.add()

#### Adds one or more class names to an element.

### classList.remove()

#### Removes one or more class names from an element.

### classList.toggle()

#### Adds a class name if it doesn't exist, or removes it if it does (useful for toggling between two states).

## JavaScript - Language Specialties

- Elaborate on the differences between value and reference data types in JavaScript, specifically in relation to objects and primitives.

### In JavaScript, value types (primitives like numbers, strings, and booleans) hold actual data, and when assigned to a new variable, the value is copied. Reference types (objects, arrays, and functions) store references to the data, so when assigned to a new variable, both variables point to the same object in memory. Changes to reference types affect all references, while changes to value types only affect the variable holding the new value.

- Discuss the concept of mutability and immutability in objects, arrays, and primitives, and explain why it is important to understand when working with data structures in JavaScript.

### Mutability refers to the ability to change the contents of a data structure after it's created. Objects and arrays are mutable in JavaScript, meaning their values or properties can be modified. Primitives like number, string, boolean, etc., are immutable, meaning their values cannot be changed directly; instead, operations create new values.

- Is `null` considered an object or a primitive in JavaScript?

### null is considered a primitive value, even though it is technically of type "object" due to a historical bug in JavaScript.

- "What does `undefined` represent in JavaScript?"

### Uninitialized variables: When a variable is declared but not assigned a value, it is automatically assigned the value of undefined.

### Function return values: If a function doesn't explicitly return a value, it returns undefined by default.

### Missing function arguments: If a function is called with fewer arguments than it expects, the missing arguments will have the value undefined.

- When would you use `var`, `let`, and `const` in JavaScript?

### let: Used when you plan to modify the value of the variable; it allows reassignment and is block-scoped.

### const: Used when you don't want to modify the value of the variable; it creates a constant reference and is block-scoped.

### var: Historically used for variable declarations; it has function scope and is hoisted, but is now generally avoided in favor of let and const due to its scope limitations.

- Explain the concept of hoisting in JavaScript.

### Hoisting in JavaScript is the behavior where variable and function declarations are moved to the top of their scope during the compilation phase.

### var declarations are hoisted and initialized with undefined.

### let and const declarations are hoisted but not initialized (they stay in a "temporal dead zone").

### Function declarations are fully hoisted, including their body, allowing them to be used before they are declared.

## Git

- Discuss the advantages of using a version control system.

### A version control system tracks changes, allows collaboration, provides backup and recovery, supports branching, and helps document code changes, making development more efficient and organized.

- Clarify the differences between Git and GitHub.

### Git is a version control system that tracks changes in code locally on your computer, while GitHub is a cloud-based platform that hosts Git repositories, enabling collaboration, sharing, and remote access to code.

- What is the purpose of remote repositories in Git?

### Remote repositories in Git store a central version of the project on a server, allowing multiple developers to collaborate, share, and synchronize their changes across different machines.

- When does a merge conflict occur in Git?

### A merge conflict occurs in Git when changes to the same line of code or the same file are made in different branches, and Git is unable to automatically reconcile those differences during a merge.

## Terminal

- How would you execute a JavaScript file in the terminal?

### Navigate to the folder where the JavaScript file is located in the terminal using the cd (change directory) command.

### Execute the JavaScript file using the node command followed by the file name.

- What is the keyboard shortcut to stop a running process in the terminal?

### Ctrl + C

- How can you retrieve the previous command executed in the terminal?

### pressing the up arrow

- How do you navigate to the parent directory of the current directory in the terminal?

### ### cd ..

## Debugging

- What techniques can you use while debugging a program?

### Debugging techniques include using print statements, setting breakpoints, stepping through code, reading error messages, writing unit tests, doing code reviews, commenting out code, using a linter, and checking dependencies to identify and fix issues.

- What does step over, step into and step out mean while using the debugger?

### Step Over: Executes the current line of code and moves to the next line, skipping over any function calls without diving into them.

### Step Into: Moves into the function being called on the current line to inspect its code.

### Step Out: Executes the rest of the current function and moves back to the calling code.

- How can you start to debug a program from a certain line using the debugger?

### set a breakpoint on that line
