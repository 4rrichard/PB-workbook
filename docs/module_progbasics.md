# Programming Basics Questions

## Data Basics

- **What are the differences between objects, arrays, and primitives in JavaScript? How are they used in programming? How would you access the value of a specific key in an object?**

  - **Objects**: Stores key-value pairs, keys are unique.
  - **Arrays**: Stores values, each value has an index.
  - **Primitives**: Represents single values.
  - **Accessing the value of a specific key**: Use dot notation (e.g., `cat.name`) or bracket notation (e.g., `cat["name"]`).

- **Explain the concept of key-value pairs in objects and how they differ from indexed elements in arrays.**

  - You can find a specific value with unique keys in objects, whereas arrays store elements in an ordered manner and are accessed through their indices (e.g., used for lists).

- **Describe a scenario where you would choose to use an object instead of an array, or vice versa, and explain your reasoning.**

  - **Arrays**: Useful for storing similar values like strings or numbers, especially when the order of elements is important.
  - **Objects**: Ideal for representing real-world concepts like storing data about a person or a product.

- **How can you retrieve the first and last items of an array?**

  - **First item**: `array[0]`
  - **Last item**: `array[array.length - 1]`

- **Identify the five most commonly used primitive types in JavaScript, and provide examples demonstrating when and how to use them.**
  - **Five primitives**: string, number, boolean, null, undefined
    - **String**: Used for text-based values (e.g., `"Hello"`).
    - **Number**: Used for calculations (e.g., `42`).
    - **Boolean**: For comparisons (e.g., `true`, `false`).
    - **Null**: Represents an intentionally empty value (e.g., `let x = null`).
    - **Undefined**: Indicates uninitialized variables (e.g., `let x;`).

---

## Algorithm Basics

- **Provide examples of assignment operators in JavaScript.**

  - `=`, `+=`, `-=`, `*=`, `/=`

- **Name some of the arithmetic operators in JavaScript.**

  - `+`, `-`, `*`, `/`, `%`, `**`

- **What are the different comparison operators in JavaScript?**

  - `===`, `==`, `!==`, `!=`, `<`, `>`, `>=`, `<=`

- **Name a few logical operators used in JavaScript.**

  - `&&`, `||`, `!`

- **Explain the differences between a `for` loop, `for...of` loop, and `for...in` loop in JavaScript.**

  - **For loop**: Mainly used when the index of elements is important.
  - **For...of loop**: Used to iterate over array values when the order is not important.
  - **For...in loop**: Iterates over the keys in an object.

- **If you can't use any built-in functions or methods, how would you calculate the average of values in an array?**
  - Create a `let` variable initialized to `0` outside the loop.
  - Use a `for` loop to add each number to it with `+=`.
  - Divide the sum by the array's length.

---

## Function Basics

- **What is a function in JavaScript? Explain its purpose and how it is used in programming.**

  - A function in JavaScript is a reusable block of code designed to perform specific tasks. Functions take inputs (parameters), process them, and return outputs. They make code modular and reusable.

- **Describe the different syntax elements that make up a JavaScript function.**

  - **Function keyword**: Marks the start of a function declaration.
  - **Function name**: Identifies the function (e.g., `myFunction`).
  - **Parameters (optional)**: Input variables (e.g., `(param1, param2)`).
  - **Function body**: The code block defining the function's behavior.
  - **Return (optional)**: Sends a result back to the caller.

- **How do you pass arguments to a function? Explain the concept of parameter passing and provide an example.**

  - Call the function with arguments (e.g., `cats("Kitty")`).
  - Inside the function, use a parameter to reference the argument (e.g., `function(catName)`).

- **What is the difference between function expressions and function declarations? Provide examples of each.**

  - **Function Declaration**: `function cat() {}`
  - **Function Expression**: `const cat = function() {}` (can be named or anonymous).

- **Explain what a callback function is in JavaScript.**

  - A callback is a function passed as an argument to another function. It is used to handle tasks like asynchronous operations (e.g., data fetching).

- **What is the scope of variables in JavaScript functions? Explain the difference between local and global variables.**
  - **Global variables**: Accessible anywhere in the program.
  - **Local variables**: Only accessible within the function or block where they are defined.

---
