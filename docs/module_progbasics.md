# Programming Basics Questions

## Data Basics

- **What are the differences between objects, arrays, and primitives in JavaScript? How are they used in programming?**

  - **Objects**: stores key-value pairs, keys are unique.
  - **Arrays**: stores values, each value has an index.
  - **Primitives**: different single values.
  - **Accessing the value of a specific key**: with the dot notation e.g., `cat.name` or `cat["name"]`.

- **Explain the concept of key-value pairs in objects and how they differ from indexed elements in arrays.**

  - You can find a specific value with the unique keys in objects.
  - In arrays, each element is ordered so they can be found through their indexes (e.g., used for lists).

- **Describe a scenario where you would choose to use an object instead of an array, or vice versa, and explain your reasoning.**

  - **Arrays**: when storing similar values like strings or numbers where the order of the elements can be important.
  - **Objects**: used to represent real-world concepts like storing the data of a person or a product.

- **How can you retrieve the first and last items of an array?**

  - First: `array[0]`, Last: `array[array.length - 1]`.

- **Identify the five most commonly used primitive types in JavaScript, and provide examples demonstrating when and how to use them.**
  - Five primitives: string, number, boolean, null, undefined.
  - **String**: e.g., providing text-based value.
  - **Number**: calculations.
  - **Boolean**: e.g., comparing two numbers if their value is the same.
  - **Null**: when a value is intentionally set to have no value.
  - **Undefined**: e.g., when a function has no return value.

---

## Algorithm Basics

- **Provide examples of assignment operators in JavaScript.**

  - `=`, `+=`, `-=`, `*=`, `/=`.

- **Name some of the arithmetic operators in JavaScript.**

  - `+`, `-`, `*`, `/`, `%`, `**`.

- **What are the different comparison operators in JavaScript?**

  - `===`, `==`, `!==`, `!=`, `<`, `>`, `>=`, `<=`.

- **Name a few logical operators used in JavaScript.**

  - `&&`, `||`, `!`.

- **Explain the differences between a `for` loop, `for...of` loop, and `for...in` loop in JavaScript.**

  - **For loop**: Mainly used when the index of an element is important.
  - **For...of loop**: Where the order is not important, just the values of the array.
  - **For...in loop**: Mainly used on objects to identify the key-value pairs (iterating over the keys).

- **If you can't use any built-in functions or methods, how would you calculate the average of values in an array?**
  - Create a `let` variable outside of the `for` loop with the value of `0`, then add each number to it from the `for` loop with the `+=` assignment operator, then divide that final value by the length of the array.

---

## Function Basics

- **What is a function in JavaScript? Explain its purpose and how it is used in programming.**

  - A function in JavaScript is a reusable block of code designed to perform a specific task. Functions take inputs (parameters), process them, and can return an output (result). They help make code modular, reusable, and easier to manage.

- **Describe the different syntax elements that make up a JavaScript function.**

  - **Function keyword**: Marks the beginning of a function declaration.
  - **Function name**: The name of the function (e.g., `myFunction`).
  - **Parameters (optional)**: Variables passed into the function (e.g., `(param1, param2)`).
  - **Function body**: The block of code that defines the function's behavior.
  - **Return (optional)**: Sends a result back from the function to where it was called.

- **How do you pass arguments to a function? Explain the concept of parameter passing and provide an example.**

  - We need to call the function outside of the function: `cats()`, then add the argument that we want to pass into the function: `cats("Kitty")`. After that, in the function parameter, name the incoming value with something descriptive (e.g., `function(catName)`), so we can use the incoming value inside the function by referring to the parameter name.

- **What is the difference between function expressions and function declarations? Provide examples of each.**

  - **Function declaration**: A named function using the function keyword, e.g., `function cat() {}`.
  - **Function expression**: A function assigned to a variable. The function can be anonymous or named.

- **Explain what a callback function is in JavaScript.**

  - When we call a function inside another function passed as an argument. Used to handle tasks that take more time (e.g., loading data) and make functions reusable.

- **What is the scope of variables in JavaScript functions? Explain the difference between local and global variables.**
  - **Global variables**: Can be accessed from local scopes like inside a function or a `for` loop.
  - **Local variables**: Only accessible within the function or loop they are declared in, unless the value is passed as an argument.

---

## Built-in Features

- **What are some commonly used built-in functions or methods in JavaScript for working with strings? Provide examples and explain their usage.**

  - `toString()`: Converts data into a string, e.g., `(4).toString()` = `"4"`.
  - `toLowerCase()`: Converts the string into lowercase letters, e.g., `(CAT).toLowerCase()` = `cat`.
  - `toUpperCase()`: Converts the string into uppercase letters, e.g., `(cat).toUpperCase()` = `CAT`.
  - `slice()`: Can be used to extract a section of a string, e.g., `"cat".slice(0, 1)` = `"at"`.
  - `replace()`: Replaces part of a string with another string, e.g., `"cat army".replace("cat", "dog")` = `"dog army"`.

- **Name at least five built-in functions or methods in JavaScript for manipulating arrays. Describe how each function/method works and provide an example for each.**
  - `map()`: Modifies each element with the same condition given (creates a new array), e.g., `arr.map(el => el + 1)` = `[3, 4, 5]`.
  - `filter()`: Filters all elements that match the given condition (creates a new array), e.g., `arr.filter(el => el >= 3)` = `[3, 4]`.
  - `reduce()`: Reduces the array to a single value by applying a function to each element, e.g., `arr.reduce((total, currVal) => total + currVal)` = `9`.
  - `includes()`: Checks if a specific value can be found inside an array (returns true or false), e.g., `arr.includes(2)` = `true`.
  - `concat()`: Merges two arrays into a new array, e.g., `arr.concat([5, 6, 7])` = `[2, 3, 4, 5, 6, 7]`.

---
