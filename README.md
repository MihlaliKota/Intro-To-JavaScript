# Intro To JavaScript

# Week 1

## Day 1

### JavaScript Introduction
----------------------------

JavaScript is a versatile and widely used programming language that is primarily employed in web development. It's a core technology for creating dynamic and interactive content on websites, ranging from simple animations to complex web applications.

At its core, JavaScript is a scripting language that allows developers to add functionality to web pages. Unlike HTML (Hypertext Markup Language) and CSS (Cascading Style Sheets), which are used for structuring and styling web content respectively, JavaScript adds behavior to web pages. This means it can respond to user actions, manipulate the content on a page in real-time, and interact with the browser's Document Object Model (DOM) to dynamically update the content without reloading the entire page.

JavaScript is not limited to just web development; it's also commonly used in other areas such as server-side development (Node.js), game development, mobile app development (using frameworks like React Native or Ionic), and even desktop application development (using frameworks like Electron).

In summary, JavaScript is a powerful programming language that enables developers to create interactive and engaging web experiences, and its versatility extends beyond the web to various other domains of software development.

### Variables, Operators & Assignments
--------------------------------------

**Comments**

In JavaScript, comments are annotations or notes that you can add to your code. They are not executed by the computer and are solely meant for humans to read and understand the code better. Comments are essential for explaining the purpose of your code, documenting how it works, or providing reminders for yourself or other programmers who may work on the code later.

There are two main types of comments in JavaScript:

1. Single-line comments: These comments start with two forward slashes `//` and continue until the end of the line. Anything written after `//` on the same line is considered a comment and is ignored by the JavaScript interpreter.

   Example:
   ```javascript
   // This is a single-line comment
   var x = 5; // This comment explains the purpose of the following code
   ```

2. Multi-line comments (also known as block comments): These comments start with `/*` and end with `*/`. They can span multiple lines and are used when you need to comment out larger sections of code or write longer explanations.

   Example:
   ```javascript
   /* This is a multi-line comment
      It can span multiple lines
      and is useful for documenting larger sections of code */
   var y = 10; /* This is an inline multi-line comment */
   ```

Comments are incredibly useful for making your code more understandable to yourself and others who might read it later. They can help you remember why you wrote a certain piece of code, explain complex logic, or provide warnings about potential issues. It's good practice to include comments in your code regularly, especially for sections that might be confusing or require clarification. However, be mindful not to over-comment, as too many comments can clutter your code and make it harder to read.


**Variables**

In JavaScript, variables are like containers that hold information. They allow you to store and manipulate data in your code. Think of them as labeled boxes where you can put different types of information, such as numbers, text, or even more complex data like lists or objects.

Here are the key points to understand about variables in JavaScript:

1. **Declaring Variables**: Before you can use a variable, you need to declare it. This means you're telling JavaScript that you want to reserve a space in memory to store some data. You declare a variable using the `var`, `let`, or `const` keywords, followed by the name you want to give to the variable.

   Example:
   ```javascript
   var age; // Declaring a variable named 'age'
   let name; // Declaring a variable named 'name'
   const PI = 3.14; // Declaring a constant variable named 'PI'
   ```

2. **Assigning Values**: After declaring a variable, you can assign a value to it using the assignment operator `=`. This value can be a number, text, boolean, or any other valid JavaScript data type.

   Example:
   ```javascript
   age = 25; // Assigning the value 25 to the variable 'age'
   name = "John"; // Assigning the value "John" to the variable 'name'
   ```

3. **Variable Types**: In JavaScript, variables can hold different types of data, such as numbers, strings (text), booleans (true or false), arrays (lists), objects (collections of properties), and more.

   Example:
   ```javascript
   var num = 10; // Number variable
   var text = "Hello"; // String variable
   var isTrue = true; // Boolean variable
   ```

4. **Variable Naming**: When naming variables, there are certain rules to follow:
   - Variable names can contain letters, numbers, underscores (`_`), or dollar signs (`$`).
   - Variable names cannot start with a number.
   - Variable names are case-sensitive (`age`, `Age`, and `AGE` are treated as different variables).

5. **Scope**: Variables have a scope, which defines where they can be accessed. JavaScript has global scope (accessible throughout the entire script) and local scope (limited to a specific function or block of code).

6. **Let and Const**: In modern JavaScript, `let` and `const` are preferred over `var` for declaring variables. `let` is used for variables whose values may change, while `const` is used for variables whose values remain constant (immutable).

   Example:
   ```javascript
   let score = 100; // Mutable variable
   const PI = 3.14; // Immutable constant variable
   ```

Overall, variables are fundamental building blocks in JavaScript, allowing you to store, manipulate, and access data within your code. They provide flexibility and control, enabling you to create dynamic and interactive applications.

**Operators**

In JavaScript, operators are symbols or keywords used to perform operations on variables and values. They allow you to manipulate data, perform calculations, compare values, and more. Operators in JavaScript can be categorized into several types:

1. **Arithmetic Operators**: These operators perform mathematical operations on numeric values.

   - Addition `+`: Adds two values together.
   - Subtraction `-`: Subtracts one value from another.
   - Multiplication `*`: Multiplies two values.
   - Division `/`: Divides one value by another.
   - Remainder `%`: Returns the remainder of a division operation.

   Example:
   ```javascript
   var result = 5 + 3; // result is 8
   ```

2. **Assignment Operators**: These operators are used to assign values to variables.

   - Assignment `=`: Assigns a value to a variable.
   - Addition assignment `+=`: Adds the value of the right operand to the variable and assigns the result to the variable.
   - Subtraction assignment `-=`: Subtracts the value of the right operand from the variable and assigns the result to the variable.
   - Multiplication assignment `*=`: Multiplies the variable by the value of the right operand and assigns the result to the variable.

   Example:
   ```javascript
   var x = 10; // Assigns the value 10 to variable x
   x += 5; // Adds 5 to x, so x becomes 15
   ```

3. **Comparison Operators**: These operators compare two values and return a Boolean result (true or false).

   - Equal to `==`: Returns true if two values are equal.
   - Not equal to `!=`: Returns true if two values are not equal.
   - Greater than `>`: Returns true if the left operand is greater than the right operand.
   - Less than `<`: Returns true if the left operand is less than the right operand.

   Example:
   ```javascript
   var a = 10;
   var b = 5;
   var result = (a > b); // result is true because 10 is greater than 5
   ```

4. **Logical Operators**: These operators are used to combine conditional statements.

   - Logical AND `&&`: Returns true if both operands are true.
   - Logical OR `||`: Returns true if at least one operand is true.
   - Logical NOT `!`: Returns the opposite of the operand's value (true becomes false, and vice versa).

   Example:
   ```javascript
   var x = 10;
   var y = 5;
   var result = (x > 5 && y < 10); // result is true because both conditions are true
   ```

5. **Unary Operators**: These operators work on a single operand.

   - Increment `++`: Increases the value of a variable by 1.
   - Decrement `--`: Decreases the value of a variable by 1.

   Example:
   ```javascript
   var x = 5;
   x++; // Increases x by 1, so x becomes 6
   ```

These are some of the basic operators in JavaScript. Understanding and using operators effectively is essential for performing various tasks in programming, such as calculations, comparisons, and logical operations.

**Assignments**

In JavaScript, assignments are the way we give values to variables. Variables are like labeled boxes where we can store different kinds of information, like numbers, text, or lists of things. Assigning a value to a variable means putting something into that labeled box.

Here's how assignments work in JavaScript:

1. **Declaring Variables**: Before we can assign a value to a variable, we need to declare it. This means we're telling JavaScript that we want to use a particular label to refer to a piece of data. We do this using the `var`, `let`, or `const` keywords, followed by the name we want to give to the variable.

   Example:
   ```javascript
   var age; // Declaring a variable named 'age'
   let name; // Declaring a variable named 'name'
   const PI = 3.14; // Declaring a constant variable named 'PI'
   ```

2. **Assigning Values**: Once we've declared a variable, we can assign a value to it using the assignment operator `=`. This is like putting something into the labeled box. The value can be a number, text, boolean (true or false), or any other type of data that JavaScript understands.

   Example:
   ```javascript
   age = 25; // Assigning the value 25 to the variable 'age'
   name = "John"; // Assigning the value "John" to the variable 'name'
   ```

3. **Updating Values**: We can change the value stored in a variable by simply assigning a new value to it. This replaces the old value with the new one.

   Example:
   ```javascript
   age = 30; // Updating the value of 'age' to 30
   ```

4. **Constants**: When we declare a variable using `const`, it means the value of that variable cannot be changed once it's assigned. This is useful when we have a value that we know should never change.

   Example:
   ```javascript
   const PI = 3.14; // Declaring a constant variable named 'PI'
   ```

5. **Scope**: Variables can have different scopes, which determine where they can be accessed. Variables declared inside a function have local scope and can only be used within that function. Variables declared outside any function (globally) have global scope and can be accessed from anywhere in the script.

6. **Undefined**: If we declare a variable but don't assign a value to it, its value will be `undefined` by default. This means the box exists, but there's nothing in it yet.

   Example:
   ```javascript
   var height; // Declaring a variable named 'height' without assigning a value (its value is undefined)
   ```

Assignments are fundamental in JavaScript because they allow us to store and manipulate data, making our code dynamic and responsive to different situations. They give us the ability to work with information in our programs, making them more useful and powerful.

## Day 2

### Strings and Arrays
----------------------

**Strings**

A string in JavaScript is a sequence of characters, including letters, numbers, and symbols, enclosed within single quotes (' '), double quotes (" "), or backticks (` `). They are used to display and work with text, which is crucial for communication in programming. Strings are immutable, meaning they cannot be changed once created.

To create and display strings, we can use `console.log()` to print them to the console or `alert()` to show a popup in the browser. Strings can be written using any of the three types of quotes, but they must match on both sides. It's important to stay consistent with the chosen quote style throughout the code.

Template literals, created with backticks, are a newer way to define strings and offer additional features compared to traditional strings. They allow for easier formatting and interpolation of variables directly within the string.

Using `console.log()`:
```javascript
console.log("This is a string in the console.");
```
Using `alert()`:
```javascript
alert("This is a string in an alert.");
```

While `console.log()` is commonly used for displaying output during development, `alert()` is less common due to its intrusive nature and the need to manually close the popup. The appearance of the alert may vary depending on the browser and operating system used.

**Arrays**

Arrays in JavaScript are a type of data structure used to store ordered collections of values. Unlike objects, which use keys to access values, arrays use indexes to determine the position of each element.

When we need to manage elements in a specific order, such as a list of users or HTML elements, arrays are more convenient than objects because they provide methods to control the order of elements.

To create an empty array, we can use either of the following syntaxes:

```javascript
let arr1 = new Array();
let arr2 = [];
```

Most often, the second syntax is preferred. We can also initialize the array with initial elements:

```javascript
let colors = ["red", "green", "blue"];
```

Array elements are numbered starting from zero, and we can access an element by its index using square brackets:

```javascript
let firstColor = colors[0]; // Accessing the first element
```

We can replace an element by assigning a new value to its index:

```javascript
colors[0] = "yellow"; // Replacing the first element
```

To add a new element to the end of the array, we can use the `push()` method:

```javascript
colors.push("orange"); // Adding a new element to the end of the array
```

The length of an array indicates the total count of elements:

```javascript
let length = colors.length; // Getting the length of the array
```

We can use `alert()` to display the entire array:

```javascript
alert(colors); // Displaying the entire array
```

Arrays can store elements of any type:

```javascript
let mixedArray = [1, "apple", true];
```

Overall, arrays are a versatile and commonly used data structure in JavaScript for managing ordered collections of values.

## Day 3

### Functions
-------------

In JavaScript, a function is a reusable block of code that can be called from anywhere in your program. This helps to avoid repetition and promotes modularity in your code by breaking it into smaller, manageable pieces.

Just like other programming languages, JavaScript supports functions like `alert()` and `write()`, which are predefined and can be used repeatedly. These functions are written in core JavaScript and can be called whenever needed.

However, JavaScript also allows you to create your own custom functions. These functions are defined using the `function` keyword, followed by a unique name, optional parameters (inputs), and a block of code enclosed in curly braces.

Example:
```javascript
function sayHello() {
    console.log("Hello!");
}
```

In this example, `sayHello` is the name of the function, and it takes no parameters. The code inside the function (console.log("Hello!");) will be executed whenever the function is called.

Defining and using custom functions in JavaScript allows you to write modular, reusable code, making your programs more organized and easier to maintain.

## Day 4

### Booleans & Conditionals
---------------------------

**Booleans**

Booleans in programming represent values that can be either true or false. They're perfect for situations where something can be "on" or "off," "yes" or "no." Storing booleans in variables helps track their values and update them as needed. For instance:

```javascript
let isRaining = true;
console.log(isRaining); // Output: true
```

In this example, the variable `isRaining` holds the boolean value `true`.

**Conditionals**

In JavaScript, booleans are often used in conjunction with conditionals to control the flow of the program based on whether a condition evaluates to true or false. Conditionals allow you to execute different blocks of code depending on whether certain conditions are met.

For example, the `if` statement is a common conditional structure that checks whether a condition is true and executes a block of code if the condition is met. Here's an example:

```javascript
let isRaining = true;

if (isRaining) {
    console.log("Remember to bring an umbrella!");
}
```

In this example, the code inside the `if` statement is executed only if the `isRaining` variable is `true`. If `isRaining` were `false`, the code inside the `if` statement would not be executed.

Conditionals can also be combined using logical operators such as `&&` (logical AND), `||` (logical OR), and `!` (logical NOT) to create more complex conditions.

Understanding how to use conditionals with booleans is essential for controlling the behavior of your JavaScript programs based on different conditions or states.


# Week 2

## Day 1

### Type Conversions
--------------------

In JavaScript, data types can often be automatically converted to the appropriate type when using operators and functions. For example, the `alert()` function automatically converts any value to a string to display it, while mathematical operations convert values to numbers as needed. However, there are cases where we need to explicitly convert a value to a specific type.

**String Conversion**
String conversion occurs when we need the string representation of a value. This is commonly done when displaying values using `alert()` or when explicitly converting a value to a string using the `String()` function.

```javascript
let value = true;
alert(typeof value); // boolean
value = String(value); // value is now a string "true"
alert(typeof value); // string
```

String conversion is straightforward, with values like `false` becoming `"false"` and `null` becoming `"null"`.

**Numeric Conversion**
Numeric conversion occurs automatically in mathematical operations and expressions. We can explicitly convert a value to a number using the `Number()` function.

```javascript
let str = "123";
alert(typeof str); // string
let num = Number(str); // becomes the number 123
alert(typeof num); // number
```

Explicit numeric conversion is useful when reading values from string-based sources but expecting a number. If the string is not a valid number, the result of the conversion is `NaN`.

**Boolean Conversion**
Boolean conversion is the simplest and happens in logical operations. We can also perform boolean conversion explicitly using the `Boolean()` function.

```javascript
alert(Boolean(0)); // false
alert(Boolean("hello")); // true
alert(Boolean("")); // false
alert(Boolean(1)); // true
```

Values like `0`, an empty string, `null`, `undefined`, and `NaN` are considered "empty" and become `false` when converted to boolean. Other values become `true`.

**Summary**
- JavaScript provides automatic and explicit conversion methods for strings, numbers, and booleans.
- String conversion occurs when needing the string representation of a value.
- Numeric conversion happens automatically in mathematical operations and expressions or can be done explicitly with `Number()`.
- Boolean conversion is straightforward and occurs in logical operations or with `Boolean()`.
- Understanding conversion methods is essential for handling different data types effectively in JavaScript.

### Document Object Model
-------------------------

The Document Object Model (DOM) is a programming interface for HTML and XML documents that provides a structured representation of the document and defines how to access its structure from scripts. It allows developers to access web pages as a structured group of nodes and connects web pages to scripts or programming languages.

JavaScript syntax involves accessing objects, properties, and methods using the "dot syntax," where each object containing the property or method is included in the reference separated by dots.

**Terms Defined**
- **Object**: Any scriptable HTML element or core object associated with the JavaScript Object Model (e.g., `window`, `document`, `form`, `image`).
- **Property**: Characteristics of an object, accessed similarly to HTML tag attributes.
- **Method**: Actions applied directly to objects, causing reactions in HTML documents.
- **Method Parameters**: Values passed to methods, providing information needed for their tasks.

**Common JavaScript Methods**
- `alert()`: Displays an alert dialog box.
- `write()`: Writes content to a page.
- `focus()`: Inserts the mouse cursor into a form element.

**Core APIs in the DOM**
- `document.getElementById(id)`: Retrieves an element by its ID.
- `document.getElementsByTagName(name)`: Retrieves elements by their tag name.
- `document.createElement(name)`: Creates a new element.
- `parentNode.appendChild(node)`: Appends a child node to a parent node.

**DOM Structure**
- The `window` object represents the browser, and the `document` object is the root of the document.
- Path references usually include the `document` object, as most objects belong to it.
- The `window` object is omitted in JavaScript code, assuming the method is invoked on the `window` object.

In JavaScript, referencing elements in the DOM is done using the dot syntax, where objects containing the desired element are specified consecutively separated by dots.

## Day 2

### Additional JavaScript Tasks
-------------------------------

### JavaScript Functions and Operators Overview:

#### Functions:
- **Calling Functions**: You can call one function from another, allowing you to nest functions and run them together.
- **Creating Objects with User-defined Functions**: Objects are central to JavaScript, and you can create your own objects using functions.
  - **Steps**: Define the object in a user-defined function, then use the `new` keyword to create the object.
- **Defining Properties**: After creating an object, you can define properties for it by assigning values to them.
  - **Methods**: An object's properties can also be methods, which are actions applied directly to objects.

#### Operators:
JavaScript has various types of operators:
- **Assignment**: Assigns a value to its left operand based on the value of its right operand.
- **Comparison**: Compares operands and returns a logical value based on whether the comparison is true.
- **Arithmetic**: Performs mathematical operations on numerical values.
- **Bitwise**: Treats operands as a set of 32 bits and performs bitwise operations.
- **Logical**: Operates on Boolean values and returns a Boolean value.
- **String**: Concatenates two string values together.
- **Conditional (Ternary)**: The only operator taking three operands and returns one value based on a condition.
- **Comma**: Evaluates both operands and returns the value of the last operand.
- **Unary**: Performs an operation with only one operand.
  - **Delete**: Deletes an object's property.
  - **Typeof**: Returns the type of its operand.
  - **Void**: Specifies an expression to be evaluated without returning a value.
- **Relational**: Compares operands and returns a Boolean value.
  - **in**: Returns true if the specified property is in the specified object.
  - **instanceof**: Returns true if the specified object is of the specified object type.
- **Operator Precedence**: Determines the order operators are applied when evaluating an expression. Parentheses can override precedence.

JavaScript operators include binary, unary, and a special ternary operator, each with different behaviors and use cases. Understanding how to use and combine these operators is essential for effective JavaScript programming.
