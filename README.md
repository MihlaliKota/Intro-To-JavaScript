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

**Functions**

- **Calling Functions**: You can call one function from another, allowing you to nest functions and run them together.
- **Creating Objects with User-defined Functions**: Objects are central to JavaScript, and you can create your own objects using functions.
  - **Steps**: Define the object in a user-defined function, then use the `new` keyword to create the object.
- **Defining Properties**: After creating an object, you can define properties for it by assigning values to them.
  - **Methods**: An object's properties can also be methods, which are actions applied directly to objects.

**Operators**

JavaScript has various types of operators:
- Assignment: Assigns a value to its left operand based on the value of its right operand.
- Comparison: Compares operands and returns a logical value based on whether the comparison is true.
- Arithmetic: Performs mathematical operations on numerical values.
- Bitwise: Treats operands as a set of 32 bits and performs bitwise operations.
- Logical: Operates on Boolean values and returns a Boolean value.
- String: Concatenates two string values together.
- Conditional (Ternary): The only operator taking three operands and returns one value based on a condition.
- Comma: Evaluates both operands and returns the value of the last operand.
- Unary: Performs an operation with only one operand.
  - Delete: Deletes an object's property.
  - Typeof: Returns the type of its operand.
  - Void: Specifies an expression to be evaluated without returning a value.
- Relational: Compares operands and returns a Boolean value.
  - in: Returns true if the specified property is in the specified object.
  - instanceof: Returns true if the specified object is of the specified object type.
- Operator Precedence: Determines the order operators are applied when evaluating an expression. Parentheses can override precedence.

JavaScript operators include binary, unary, and a special ternary operator, each with different behaviors and use cases. Understanding how to use and combine these operators is essential for effective JavaScript programming.

**Regular Expressions**

Regular expressions (regex) are sequences of characters used for search patterns in text operations. They describe what you're searching for in text data. They can range from simple characters to complex patterns. Regular expressions enable various text search and replace operations.

Example:
```javascript
var patt = /w3schools/i;
```
Explanation:
In this example, `/w3schools/i` is a regular expression where `w3schools` is the pattern for search, and `i` is a modifier indicating case insensitivity.

In another scenario, if we have a sentence: "The dog chased the cat." and we want to match the pattern "the", we can use the regex `/the/`.

```javascript
let sentence = "The dog chased the cat.";
let regex = /the/;
```
Notice how `/the/` indicates the pattern we're searching for in the sentence. 

To determine if a pattern exists in a string, we use the `test()` method:

```javascript
let myString = "Hello, World!";
let myRegex = /Hello/;
let result = myRegex.test(myString); // Result will be true
```
Let's consider finding "Waldo" in a text:

```javascript
let waldoIsHiding = "Somewhere Waldo is hiding in this text.";
let waldoRegex = /Waldo/;
let result = waldoRegex.test(waldoIsHiding); // Result will be true
```
Note that `waldoRegex` is case-sensitive, so `/Waldo/` returns true, whereas `/waldo/` would return false.

## Day 3

### JavaScript Forms
--------------------

**JavaScript Methods and “this” Keyword**

In JavaScript, objects can include functions, known as methods. A method is essentially a property of an object that holds a function value. Accessing object methods is done using dot notation, where you call the object name followed by the method key along with parentheses. Similarly, you can add methods to objects by defining them within the object's declaration.

JavaScript offers numerous built-in methods for various tasks. For instance, the `parseInt()` method of the Number object converts a numeric string to an integer value. You can also add methods to objects after their creation, as demonstrated by adding the `greet` method to the `student` object in an example.

When accessing properties within an object's method, the `this` keyword is used to refer to the object itself. It allows the method to access and manipulate the object's properties effectively. However, functions inside objects can also access their variables similar to regular functions.

Example:
```javascript
let person = {
  name: "John",
  age: 30,
  greet: function() {
    return "Hello, my name is " + this.name + " and I am " + this.age + " years old.";
  }
};
console.log(person.greet()); // Output: Hello, my name is John and I am 30 years old.
```

**JavaScript Switch Statement**

The switch statement in JavaScript is employed to execute different actions based on varying conditions. It allows for the selection of one of multiple code blocks to execute. The syntax involves evaluating a switch expression once and comparing its value with each case's values. If a match is found, the associated block of code executes; otherwise, the default code block executes. 

For instance, the `getDay()` method returns the weekday as a number between 0 and 6, where Sunday is 0 and Saturday is 6. By using a switch statement with `getDay()`, you can determine the weekday name. 

```javascript
let day;
switch (new Date().getDay()) {
  case 1:
    day = "Monday";
    break;
  // additional cases for other weekdays...
  default:
    day = "Unknown";
}
```

The `break` keyword is used to exit the switch block once a match is found, preventing further execution. If no case matches the switch expression, the `default` keyword specifies the code to run. It's worth noting that the `default` case doesn't have to be the last one.

When multiple cases match a case value, the first one encountered is selected. If no matching cases are found, the program proceeds to the default label. If there's no default label, the program continues to the statements after the switch.

Switch cases employ strict comparison (===), meaning values must be of the same type to match. If the operands aren't of the same type, no match occurs.

Example exercise:
```javascript
let fruits = "apple";
switch (fruits) {
  case "banana":
    alert("Hello");
    break;
  case "apple":
    alert("Welcome");
    break;
  default:
    alert("Unknown fruit");
}
```

## Day 4

### JavaScript Eve
------------------

**Built-In JavaScript Functions**

In JavaScript, there are several built-in functions that are commonly used to perform various tasks. Let's explore some of these functions with examples:

1. `document.write()`:
   - The `document.write()` method allows you to output text or HTML content directly to the webpage.
   - It's commonly used for quick testing or to dynamically generate content.
   
Example:
```html
<!DOCTYPE html>
<html>
<head>
    <title>document.write() Example</title>
</head>
<body>
    <script>
        document.write("Hello, World!");
    </script>
</body>
</html>
```
Output:
```
Hello, World!
```

2. `window` Object Methods:

   - **`alert()`:** Displays an alert dialog box with the specified message and an OK button.
   - **`confirm()`:** Displays a dialog box with a specified message, along with OK and Cancel buttons.
   - **`prompt()`:** Displays a dialog box that prompts the user for input.
   - **`open()`:** Opens a new browser window.
   - **`close()`:** Closes the current browser window.
   - **`setTimeout()`:** Executes a function or specified code after a specified delay.

Example (Using `confirm()` and `alert()`):
```javascript
// Using confirm() method
var result = confirm("Do you want to proceed?");
if (result === true) {
    alert("You clicked OK!");
} else {
    alert("You clicked Cancel!");
}
```
In this example, a confirmation dialog is displayed, and based on the user's response, an alert is shown accordingly.

Remember, for `prompt()`, `open()`, `close()`, and `setTimeout()`, you can experiment by implementing them in your own scripts to see how they work.


**Methods of the Document Object**

The Document Object in JavaScript provides several methods to interact with and manipulate the contents of an HTML document. Let's explore some of these methods along with examples:

1. `write("string")`:
   - Writes the given string directly onto the document.
   - It's used to dynamically add content to the page.
   
Example:
```html
<!DOCTYPE html>
<html>
<head>
    <title>write() Method Example</title>
</head>
<body>
    <script>
        document.write("This text is dynamically added to the document.");
    </script>
</body>
</html>
```

2. `writeln("string")`:
   - Writes the given string onto the document with a newline character at the end.
   - Similar to `write()` but adds a newline after the specified string.
   
Example:
```html
<!DOCTYPE html>
<html>
<head>
    <title>writeln() Method Example</title>
</head>
<body>
    <script>
        document.writeln("This text is dynamically added to the document with a newline.");
        document.writeln("Next line.");
    </script>
</body>
</html>
```

3. `getElementById()`:
   - Returns the element with the specified id attribute.
   
Example:
```html
<!DOCTYPE html>
<html>
<head>
    <title>getElementById() Method Example</title>
</head>
<body>
    <div id="myDiv">This is a div element with id="myDiv"</div>
    <script>
        var element = document.getElementById("myDiv");
        console.log(element.textContent); // Output: This is a div element with id="myDiv"
    </script>
</body>
</html>
```

4. `getElementsByTagName()`:
   - Returns a collection of elements with the specified tag name.
   
Example:
```html
<!DOCTYPE html>
<html>
<head>
    <title>getElementsByTagName() Method Example</title>
</head>
<body>
    <ul>
        <li>Item 1</li>
        <li>Item 2</li>
    </ul>
    <script>
        var listItems = document.getElementsByTagName("li");
        console.log(listItems.length); // Output: 2
    </script>
</body>
</html>
```

5. `getElementsByClassName()`:
   - Returns a collection of elements with the specified class name.
   
Example:
```html
<!DOCTYPE html>
<html>
<head>
    <title>getElementsByClassName() Method Example</title>
</head>
<body>
    <div class="box">Box 1</div>
    <div class="box">Box 2</div>
    <script>
        var boxes = document.getElementsByClassName("box");
        console.log(boxes.length); // Output: 2
    </script>
</body>
</html>
```

These examples demonstrate how to use various methods of the Document Object to interact with HTML elements within a webpage.

## Day 5

### Reflections
---------------

**Reflections on Week 2:**

During Week 2, I delved deeper into JavaScript concepts, particularly focusing on type conversions, the Document Object Model (DOM), functions, operators, regular expressions, JavaScript forms, built-in JavaScript functions, and methods of the Document Object. Here's a recap of what I've learned and how I applied these concepts:

1. **Type Conversions:*
   - I learned about automatic and explicit type conversions in JavaScript for strings, numbers, and booleans. 
   - Applying these concepts involved understanding when and how to convert data types explicitly to handle different scenarios effectively.

2. **Document Object Model (DOM):*
   - Understanding the DOM's structure and common methods enabled me to manipulate HTML documents dynamically using JavaScript.
   - I applied the dot syntax to access elements within the DOM hierarchy, utilizing methods like `getElementById()` and `getElementsByTagName()`.

3. **Functions and Operators:*
   - I explored the creation and invocation of functions, including nested functions and methods of creating objects with user-defined functions.
   - Learning about various types of operators, such as arithmetic, comparison, and logical operators, helped me perform different operations efficiently.

4. **Regular Expressions:*
   - Regular expressions allowed me to define search patterns in text operations, enhancing my ability to work with textual data effectively.
   - I practiced using regular expressions to search for patterns within strings and understand their application in practical scenarios.

5. **JavaScript Forms:*
   - Learning about JavaScript methods and the `this` keyword provided insights into object-oriented programming in JavaScript.
   - I gained proficiency in utilizing switch statements to execute different code blocks based on varying conditions.

6. **Built-In JavaScript Functions and Document Object Methods:*
   - Exploring built-in functions like `alert()`, `confirm()`, and `document.write()` empowered me to interact with users and dynamically modify webpage content.
   - Understanding Document Object methods like `getElementById()` and `getElementsByTagName()` enabled me to manipulate HTML elements efficiently within a webpage.

Overall, Week 2 deepened my understanding of JavaScript fundamentals and provided practical insights into leveraging JavaScript to enhance webpage interactivity and functionality. By applying these concepts through examples and exercises, I honed my skills in JavaScript programming and gained confidence in building dynamic web applications.

# Week 3

## Day 1

### JavaScript Events
---------------------

**Strings Operations**

Strings in JavaScript can be created as primitives, from string literals, or as objects using the `String()` constructor. String primitives and objects can be used interchangeably in most cases. String literals can be enclosed in single or double quotes, or using backticks for template literals that allow expression interpolation.

Accessing individual characters in a string can be done using the `charAt()` method or by treating the string as an array-like object with numerical indices. When using bracket notation for character access, properties are not writable or configurable.

In JavaScript, string comparison can be done using the less-than and greater-than operators or the `localeCompare()` method for more complex comparisons. JavaScript distinguishes between String objects and primitive string values, automatically converting primitives to objects when needed.

When using `eval()`, primitives are treated as source code while String objects are treated like other objects. Authors should be aware of potential issues when expecting primitive strings but encountering String objects, although conversion is possible using the `valueOf()` method.

**On-event Handlers**

On-event handlers in DOM elements are properties that manage how elements respond to events like clicks, key presses, or focus changes. These handlers are named according to the event they handle, such as onclick or onkeypress.

You can set event handlers using HTML attributes like `onclick="return handleClick(event);"`, or by setting properties in JavaScript like `document.getElementById("mybutton").onclick = function(event) { ... }`. Each object can have only one on-event handler per event, but you can use `addEventListener()` to add multiple independent handlers.

Event handlers are automatically called when events occur, and they can be assigned real handler functions. Parameters like `event` are passed to handlers, and the `this` keyword refers to the element the handler is registered on. The return value from a handler can determine if the event is canceled.

When discussing event handling, an event listener is set up using `addEventListener()`, while an event handler typically refers to functions registered via on-attributes or properties. `addEventListener()` adds a function or object implementing `EventListener` to the list of event listeners for a specific event type on the target element.

In summary, on-event handlers provide a way to manage how elements respond to events, offering flexibility and control over event-driven interactions in web development.

**Event handlers specific rules**

Event handlers in HTML elements, Document, and Window objects have specific rules for support across different elements and objects. These event handlers can be used as both content attributes and IDL attributes.

onabort: Triggered when an event is aborted, like when media data fetching is stopped prematurely.
oncanplay: Fired when media can start playing but is still buffering.
oncanplaythrough: Indicates media can play continuously without further buffering.
onchange: Activated when a user changes an object and moves away from it.
onclick: Responds to a user clicking on an object.
ondblclick: Fired when a user double-clicks on an object.
ondurationchange: Triggered when the media length changes.
onended: Activated when media playback reaches the end.
oninput: Responds to user input.
onkeydown, onkeypress, onkeyup: Fired on key press events.
onloadeddata, onloadedmetadata: Indicate when media data can be rendered or when media dimensions are determined.
onmousedown, onmouseup: Respond to mouse button presses and releases.
onmouseenter, onmouseleave: Fired when the cursor enters or leaves an element.
onmousemove, onmouseout, onmouseover: Respond to mouse movements over elements.
onmousewheel: Triggered when the mouse wheel is rotated.
onpause, onplay, onplaying: Events related to media playback.
onprogress: Indicates media data fetching progress.
onreset: Fired when a form is reset.
onseeked, onseeking: Events related to seeking in media playback.
onselect: Activated when content is selected.
onsubmit: Fired when a form is submitted.
onsuspend: Indicates media data fetching is suspended.
ontimeupdate: Fired when media playback position changes.
ontoggle: Triggered when a details element is opened or closed.
onvolumechange: Responds to changes in volume or mute status.
onwaiting: Indicates the next media frame is not yet available.

These event handlers provide a way to manage various interactions and behaviors in web development, offering a range of options for handling user actions and media playback events.

## Day 2

### Dynamic JavaScript Techniques
---------------------------------

**Dynamic HTML**

CSS and JavaScript can be integrated with HTML to create dynamic web pages known as dynamic HTML. Events can drive changes on a website, ranging from simple text formatting to dynamic content updates and object movements.

*Changing HTML Objects:*
Objects in HTML can be altered in two main ways:
By modifying the class of the object to adjust its style.
Using the object's style property directly to change its appearance.

*Designing JavaScript Functions:*
JavaScript functions can be designed in various ways:
Directly referencing an object in the function using its ID to modify its style exclusively.
Passing an object's ID as an argument to the function for flexible style changes.
Accessing objects based on events to identify the object involved in the event occurrence. 

**Date Object**

The Date object in JavaScript is a built-in object that stores date and time information, providing various methods for managing and formatting dates. When creating a new Date instance without arguments, it corresponds to the current date and time based on the computer's system settings. JavaScript interprets dates based on a timestamp derived from Unix time, which counts the milliseconds since January 1st, 1970. There are different ways to create a new Date in JavaScript:

1. `new Date()`: Represents the current date and time.
2. `new Date(timestamp)`: Creates a date based on milliseconds since Epoch time.
3. `new Date(date string)`: Generates a date based on a specific date string.
4. `new Date(year, month, day, hours, minutes, seconds, milliseconds)`: Constructs a date based on specified date and time components.

JavaScript provides methods like `getTime()` to retrieve timestamps and various `get` methods to access different components of a date like year, month, day, etc. Additionally, there are corresponding `set` methods to modify these components. UTC methods are available for working with Coordinated Universal Time.

Understanding how JavaScript handles dates is crucial for developers as it involves managing timestamps and date strings effectively for different applications and functionalities.

## Day 3

### Keyboard, Form, and Document/Window Events 
----------------------------------------------

**Keyboard Events**

Understanding keyboard events and their associated event handlers is crucial for interactive web development. Three primary keyboard events are highlighted: keydown, keyup, and keypress.

1. *Keydown Event (onkeydown):* This event triggers when a user presses a key. It's handled using the `onkeydown` event handler. An example demonstrates triggering an alert message upon keydown.

2. *Keyup Event (onkeyup):* This event occurs when a user releases a key. It's managed using the `onkeyup` event handler. An example illustrates displaying an alert message upon keyup.

3. *Keypress Event (onkeypress):* The keypress event triggers when a key press results in a character value. Not all keys trigger this event; for example, special keys like Ctrl or Shift won't generate a keypress event but will still trigger keydown and keyup events. It's handled using the `onkeypress` event handler, and an example showcases alert message display upon keypress.

Understanding and utilizing these keyboard events and their associated event handlers empower developers to create more dynamic and responsive web applications.

**Form Events**

Form events play a vital role in web development, as they respond to user interactions with form controls like text inputs, select boxes, and more. These events trigger when a control receives or loses focus, or when a user modifies a control's value.

Four key form events and their event handlers are highlighted:

1. *Focus Event (onfocus):* This event fires when a user gives focus to an element. It's handled using the `onfocus` event handler. An example demonstrates highlighting a text input's background in yellow when it receives focus.

2. *Blur Event (onblur):* Occurring when a user removes focus from a form element or window, the blur event is managed using the `onblur` event handler. An example showcases displaying an alert message when a text input loses focus.

3. *Change Event (onchange):* When a user alters a form element's value, the change event is triggered. It's controlled with the `onchange` event handler. An example illustrates showing an alert message upon changing an option in a select box.

4. *Submit Event (onsubmit):* Exclusive to form submissions, the submit event occurs when a user submits a form. It's handled using the `onsubmit` event handler. An example depicts displaying an alert message when submitting a form to the server.

Understanding and utilizing these form events and their handlers empower developers to create more interactive and user-friendly web forms.

**Document/Window Events**

Apart from user interactions, events in web development also encompass scenarios like page loading and browser window resizing. These document/window events trigger specific actions and can be controlled using event handlers.

Three significant document/window events and their event handlers are highlighted:

1. **Load Event (onload):** This event fires when a web page finishes loading in the browser. It's managed using the `onload` event handler. An example demonstrates displaying an alert message once the page completes loading.

```javascript
window.onload = function() {
    alert('Page loaded successfully!');
};
```

2. **Unload Event (onunload):** Occurring when a user navigates away from the current page, the unload event is handled using the `onunload` event handler. An example showcases triggering an alert message when attempting to leave the page.

```javascript
window.onunload = function() {
    alert('Are you sure you want to leave this page?');
};
```

3. **Resize Event (onresize):** When a user resizes the browser window, the resize event is triggered. It also occurs when the window is minimized or maximized. Managed with the `onresize` event handler, an example displays an alert message upon resizing the browser window to a new width and height.

```javascript
window.onresize = function() {
    alert('Browser window resized!');
};
```

Understanding and utilizing these document/window events and their associated handlers is essential for creating dynamic and responsive web applications.

# Week 4

## Day 1

### Program Flowcharts, Loops and Decision structures 
-----------------------------------------------------

**Program Flowcharts**

After analyzing a problem or opportunity, designing the program to solve it is essential. This design process results in a program flowchart, illustrating the program's logic and data manipulation. Flowcharts are crucial as they allow for easier determination, arrangement, and modification of complex logic compared to correcting errors in implemented programs. They facilitate easy maintenance and efficient modifications of programs.

*Program Flowchart Symbols:*
Program flowcharts utilize standardized symbols, simplifying comprehension and maintenance by individuals other than the original programmer. These symbols represent various program elements and logic. Watching a video to familiarize oneself with these symbols aids in understanding program flow.

Moving forward, the implementation of critical elements within the program flowchart will be explored in the upcoming section.

*Best Practices for Flowcharts:*
Although you may desire to enhance the visual appeal of your program flowchart, it's recommended to adhere to standardized symbols. However, you can still add visual interest by incorporating different colors for symbols and labels. When creating program flowcharts, consider the following points:

1. Utilize appropriate symbols to represent different elements of the program logic.
2. Ensure consistent flow direction throughout the flowchart to maintain clarity.
3. Use color schemes or color coding to enhance visual understanding, but avoid overuse or excessive complexity.
4. Maintain consistent sizes for symbols to promote uniformity and readability.
5. Maintain consistent spacing between symbols to enhance the overall organization and clarity of the flowchart.

**JavaScript For Loop**

Now that we have a grasp of flowcharts, let's delve into loops. Loops are instrumental in executing a block of code repeatedly, particularly useful when working with arrays. Instead of manually writing repetitive code to iterate through an array, loops streamline the process. JavaScript offers various types of loops:

1. **for**: Executes a block of code a specified number of times.
2. **for/in**: Loops through the properties of an object.
3. **for/of**: Loops through the values of an iterable object.
4. **while**: Executes a block of code while a condition is true.
5. **do/while**: Similar to while loop but ensures that the code block is executed at least once.

The syntax for a for loop is as follows:

```javascript
for (statement1; statement2; statement3) {
  // code block to be executed
}
```

- Statement1: Executed once before the loop starts.
- Statement2: Defines the condition for executing the code block.
- Statement3: Executed after the code block has been executed on each iteration.

You can customize the initialization, condition, and iteration parts of the loop based on your requirements. These parts are optional and can be omitted if not needed. The flexibility of JavaScript allows for various configurations within the loop structure, making it versatile for different programming scenarios.

## Day 2

### Website and Search Engine Optimization and Game Development 
---------------------------------------------------------------

**Image and Video Optimization**

https://www.freecodecamp.org/news/a-beginners-guide-to-website-optimization-2185edca0b72/

In this article by Mario Hoyos, he shares his experience optimizing images on his website, achieving an impressive 99/100 in Google’s optimization ranking. As a beginner web developer, Mario initially overlooked the impact of images on page load times. However, he realized the importance of image optimization, primarily through compression. Mario used Optimizilla, a user-friendly online tool, to compress images, noting significant size reductions of up to 70%. He suggests alternative tools such as ImageOptim for Mac or FileOptimizer for Windows, or using plugins like Gulp and WebPack for compression during build processes. Mario also discusses the choice between JPEG and PNG formats based on transparency needs, highlighting Google’s webp format for future consideration. For video optimization, Mario recommends platforms like Vimeo, YouTube with the youtube-dl tool, or services like Brightcove, Sprout, or Wistia for professional hosting and optimization.

**General Website Optimization**

From the previous article, the author discusses additional ways to optimize websites beyond image compression. 

1. **Gzip Compression:** The author explains gzip compression, a method to reduce file sizes transmitted over the internet. Although some hosting services offer gzip options, others require manual implementation using compression middleware in server-side code.

2. **Minification:** Minification involves removing unnecessary characters from code to reduce file size without affecting functionality. While build tools like Webpack or Gulp can handle minification, simpler alternatives like HTML-Minifier, CSSNano, and UglifyJS are recommended by Google.

3. **Browser Caching:** Storing static files in the browser cache can significantly speed up website loading times, especially for returning visitors. The author demonstrates how to add cache-control headers to HTTP responses using Node/Express servers.

4. **Content Distribution Network (CDN):** CDNs improve website performance by distributing content across multiple proxy servers worldwide, reducing load times for users regardless of location. Popular CDNs include CloudFront and CloudFlare.

5. **Miscellaneous Tips:** The author offers additional optimization tips, such as lazy-loading images to prioritize above-the-fold content and loading script tags at the bottom of HTML files to improve time-to-interactive.

In conclusion, the author emphasizes the importance of measuring website performance and addressing specific bottlenecks rather than applying generic optimizations. Each website may require unique optimization strategies based on its traffic and service requirements.

**Search Engine Optimization**

https://moz.com/beginners-guide-to-seo/why-search-engine-marketing-is-necessary

This article delves into the basics of Search Engine Optimization (SEO) provided by moz.com, focusing on understanding how search engines work, identifying organic search results, and highlighting the importance of SEO.

Search Engine Basics: Search engines function as answer machines, evaluating numerous factors to determine the relevance of content to user queries. They achieve this through crawling, indexing, and ranking web content.

Organic Search Results: Organic search results are earned through effective SEO and are distinguished from paid advertising. Today's search engine results pages (SERPs) include various formats, such as featured snippets, People Also Ask boxes, and local packs, driven by user intent.

Significance of SEO: While paid advertising and social media can drive website traffic, organic search results occupy more digital real estate, appear credible to users, and receive more clicks. SEO offers substantial traffic opportunities compared to pay-per-click (PPC) advertising and can yield long-term benefits with continuous traffic growth.

Role of SEO: SEO helps optimize websites to provide relevant information to search engines for proper indexing and display in search results. By understanding how search engines work and implementing effective SEO strategies, websites can attract more organic traffic and improve their online visibility.

# NodeJs

## Introduction To NodeJs
-------------------------

**History Of NodeJs**

Node.js, despite its perception as a new technology, has been around for more than ten years and is one of JavaScript's most widely used tools. Originating in 2009 from Ryan Doll's concept, Node.js is a JavaScript runtime built on Chrome's VA engine. A pivotal moment came in 2011 with npm 1.0's release, the node package manager, enabling the sharing of open-source node libraries and revolutionizing code sharing and maintenance. This solidified Node.js's position as a significant player in the ecosystem.

In 2015, amidst community disagreements over implementation and project management, the Node.js Foundation was established. Consisting of major players like IBM, Microsoft, and PayPal, the foundation operates as a Linux Foundation project. This collaborative effort ensures these influential companies steer the library's growth and development for the long term. The Node.js community is thriving, with numerous international conferences and events, and is widely applied across various industries.

If you've worked with JavaScript before, you're likely familiar with its use in front-end development, enhancing websites with interactive features. But JavaScript goes beyond just the front end. With Node.js, we can extend our JavaScript skills to a wider range of tasks, like building command line tools and creating servers.

Node.js, introduced in 2009, is embraced by big companies like PayPal, Netflix, and Microsoft for developing scalable event-driven applications. In this course, we'll explore key aspects of Node core, including standard input and output, the module system, and file handling. Throughout the course, we'll provide practical examples that are easy to understand and useful in real-world situations.

**JavaScript and Node**

In modern web development, front-end components are everywhere, and they're typically written in JavaScript since web browsers exclusively use this language. Using the same language for both front-end and back-end development offers numerous advantages. It eliminates concerns about syntax differences between languages, making the development process smoother.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/f156e090-9f63-40ea-8120-b2fc77c1d20a)

I've personally experienced this while working extensively with C# and occasionally switching to JavaScript. Managing these transitions was mentally taxing due to syntax variations. But the real advantage is the seamless sharing of code and data structures between the front-end and back-end. Let's explore scenarios where code sharing is crucial. Libraries like Underscore, which provide encryption or utility functions, can be used consistently on both sides.

For example, imagine creating a user authentication system using tokens. Using the same token and encryption library ensures authorization consistency. Similarly, in a web game where an attack algorithm runs on the front end and is checked on the back end to prevent cheating, maintaining identical algorithms is vital.

Another case involves data models, like user definitions with many properties. If these models are in different languages, maintaining them becomes challenging. Modifying multiple data models across two languages is less efficient than doing so in one language, highlighting the importance of minimizing redundancy and maximizing efficiency.

By embracing code sharing and using a common language for both front-end and back-end development, we gain significant benefits in terms of maintainability and overall development efficiency.

**Pros of JavaScript**

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/4264e855-d9ce-45a7-a025-996aff491a74)

With Node.js, we can use the same language for both the back end and front end, making it easier to share code across these parts. A notable feature of JavaScript is its dynamic nature, where the type of a variable is determined by its value rather than during declaration, showing loose typing compared to strong typing.

JavaScript integrates smoothly with JSON (JavaScript Object Notation), a format ideal for web applications on both ends. Unlike other languages in different environments, JavaScript simplifies data transfer from the back end to the front end without complex conversions.

While JavaScript offers numerous advantages, some may see them as drawbacks in specific scenarios. Despite not being a universal solution, the ability to use JavaScript across the front end and back end significantly improves the development experience for web apps.

**Callbacks and Asynchronous Tasks**

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/6b5588f2-4540-492e-abcc-3ea4130ee12a)

Performing tasks synchronously means waiting for each task to finish before moving on to the next one, which can cause blocking. On the other hand, executing tasks asynchronously lets us move to the next task without waiting for the previous one to complete. An example of synchronous processing is when submitting a form results in a grayed-out screen until a response is received, indicating a synchronous background process that delays user interface responsiveness until it's done.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/58b613ca-4557-4359-a257-a4c3e75656e7)

When ranking tasks by completion time on a computer, networking and file system access typically involve long waits, especially in web applications. Node's effectiveness for web apps comes from its skillful management of these tasks.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/3ed70511-9cf5-45e4-89fb-3987fdad9022)

Asynchronous code often involves using callbacks, as demonstrated in the following code snippet where we load and read directories from drive C using Node. In the synchronous version, each line waits for the previous task to complete, as observed when running the code. Conversely, in the asynchronous version, despite having the "this comes after" console log on the last line, it executes first because of the callback defined on line three. This callback is like registering a phone number for a callback in tech support—it allows the execution to continue, and the callback is triggered upon task completion, similar to how readdir calls our "phoneNumber" callback described on line seven.

## Node Globals
---------------

**Node Globals**

Let's delve into how modules work in Node.js. Start by creating a new file in Visual Studio Code named "my-module.js." At the same time, create another file called "module-demo.js," where the goal is to access the code within "my-module.js." This demonstrates the power of code reuse, such as using a math library in various files or projects.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/873b1e0d-ad2c-451e-b062-20fc2d959a2f)

In "my-module.js," use the exports object to share data externally. Create a property named "myText" with a placeholder value, such as "hello from module." This allows other parts of the codebase to access and use this data.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/88589495-98a2-41c7-95bb-f3a4567e686e)

Node's module loading system is simple, associating one file with one module. To access "my-module.js," assign its reference to a variable in "module-demo.js" using the require function.

For testing, use a console log to confirm that the values retrieved from our module are as expected. Run the "module-demo.js" file in the console or terminal with the command "node module-demo," and you should see the console log displaying the "hello from module" placeholder text. This shows that data access in "module-demo.js" from another module or file is successful, a capability that can be expanded upon in future development stages.

**Third-Party Packages**

After learning how to create modules in Node.js, it's essential to understand how to use third-party modules.

Node introduces the Node Package Manager (NPM), a tool for managing packages, which are collections of one or more modules. One commonly used package is Lodash. Let's see how to install and use it. Open your console or terminal and install Lodash with the command "npm install lodash." Once installed, check your directory, and you'll notice a new folder named "node_modules," containing the "lodash" package with its JavaScript files providing functionality.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/8178e991-9acf-4e1c-bf0d-21393352a005)

Now that Lodash is installed, let's create a file for our code called "demo.js." Use the "require" function, similar to how we included our custom module, to bring in Lodash. Assign it to a variable, typically named "_". Remember, there's no need to specify a location because Node knows the default module location. Use "console.log" to display the available functions. For example, you can use the "random" function to get a random number between one and one hundred. Unlike plain JavaScript, which needs multiple calls to the math library, Lodash simplifies this process. Save the file and test it with "node demo.js." You should see a random value in the console.

Moving forward, there are various types of NPM packages, including those functioning as command line interfaces. Let's take Nodemon as an example. Install it globally using the "-g" flag to make it accessible across projects. Notice that Nodemon doesn't appear in the local "node_modules" folder but is globally available. Instead of using "node," use "nodemon" to automatically execute scripts upon changes, improving development efficiency.

But what if we install multiple third-party packages and need to track dependencies? That's where the "package.json" file comes in. This file enables us to maintain a list of installed packages and their dependencies. Let's explore its importance in the next step.

**Package.json Files**

As we develop our project, it involves custom files and third-party packages. Yet, when it comes to sharing our app or storing it in a git repository, including all dependencies becomes impractical. This is because they take up considerable space and make the transfer process time-consuming.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/cedd1920-f3c3-47ab-924f-b7688e5d0cfe)

To simplify the process for another developer who wants to use our project, we can create a package.json file. This file keeps track of all the project's dependencies. By using the npm install command, developers can automatically install everything listed in this file. To create the package.json file, open the terminal and type npm init, then follow the prompts or use the defaults. Once created, the file includes the chosen settings and scans the node_modules folder to add dependencies to the list. For a quick creation with default settings, use npm init --yes. Now that we've covered managing modules and packages in Node, let's explore one of the widely used built-in modules for file read and write operations.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/d3442327-cac1-443f-9a24-26819679523f)

## Node Modules
---------------

**Node Modules**

When dealing with heavy input/output operations, two main areas are network and disk access. Let's focus on disk access by working with files. To start, create a new file named demo.js. Next, we'll access the file system within Node by requiring the 'fs' module, which is also conveniently named 'fs.'

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/396e1ada-60e8-407f-957a-6d26b5a4b471)

Firstly, let's create a file to read from. We'll generate a temporary JSON file named data.json. Inside this file, we'll create an object with a property named 'name,' enclosed in double quotes, and use 'Tim' as a placeholder value. 

To access the file system, we'll use the 'readFile' function, passing in the location of our data JSON file as the first parameter. Since this function operates asynchronously, the second parameter is a callback function. We have the option to use either a separate function or an anonymous function directly as the callback, or we can choose a more concise arrow function.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/43135ab6-7109-4906-8ba6-b545d52b009e)

When we run the code, we notice unexpected output with a buffer at the start. This occurs because we haven't specified a file format. To fix this, we move the callback to the third parameter and add 'UTF-8' as a string in the second parameter. This adjustment enables us to successfully read the JSON data without encountering the buffer issue.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/d455f523-5ad8-4e57-8717-3404a98eff59)

Another approach is to directly access the JSON file using 'require'. By creating a variable named 'data' and assigning it the result of 'require' with the path to data.json, we can log the data. Now, we notice two distinct objects in our console - one from 'require' and another from 'readFile.'

These objects have differences. Testing the 'name' property reveals that the object from 'require' is a true object, while the one from 'readFile' is just a string. To address this, within the 'readFile' callback, we create a new variable named 'data' and set it to 'JSON.parse(data)' to convert the string to JSON. As a result, we can access 'data.name', displaying two names in the console.

**Directory Access**

Now that we're familiar with reading files in the file system, let's move on to exploring directory reading. We'll create a new demonstration file that requires access to the file system. To do this, we'll require the 'fs' module and use the 'readdir' function from the file system. The initial parameter for 'readdir' should indicate the directory location we want to read - for example, let's use Drive C as an example.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/044c1c87-92ee-4424-b52c-3cda96d532a0)

Next, let's set up a callback function that accepts error and data as parameters, then proceed to log the data using the console. After saving the changes, use nodemon to run the demo, and observe the output, which will display all directories within Drive C. This demonstrates the straightforward process of reading directories.

**Writing to Files**

Now that we're proficient in file and directory operations, our next focus is on file writing. To start, we create a new file named demo.js and include the file system module. For writing a file, we use the writeFile function, with the file name as the first parameter (in this case, data.json) and the data to be written as the second parameter. Instead of directly specifying the data, you can define a variable, 'data,' as a JSON object. This object includes a 'name' property with the value 'Bob.' Then, we pass this data object as the second parameter to the writeFile function.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/54019508-b849-410e-ad97-eb50676e48ac)

When we run the script using the command node demo.js, it creates a data.json file. However, upon examination, we notice that the file content doesn't match our expectations. This happens because the writeFile function expects a string as the second parameter, not a JSON object. To fix this, we need to convert our object to a string. While one way to do this manually is by enclosing everything in double quotes, a more efficient approach is to use JSON.stringify. We make this adjustment on line seven, resulting in the desired JSON format.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/22add7bc-3716-404a-a389-b9207c1d978f)

While the script works as intended, we encounter a deprecation warning cautioning against calling an asynchronous function without a callback. Upon investigation, we discover that the writeFile function expects a callback as its third parameter. To address this, we create a callback function that logs any errors and a 'write finished' message to the console. With this update, the script eliminates the deprecation warning and provides feedback upon completion.

With a solid understanding of file system operations, our next focus is to explore popular web frameworks for Node.js.

## Node File Management and Streams
-----------------------------------

**Node Frameworks**

We'll delve into different Node.js frameworks for web development. First, let's grasp the concept of a framework. In basic terms, it acts as a foundational structure, similar to the support system of a building or vehicle. In software development, a framework offers the fundamental structure that enables developers to construct their applications on top of it.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/92f91715-fc7f-4f37-938e-6a3aa04436fb)

In web development, especially for building large APIs or HTTP servers, using web frameworks becomes essential. These frameworks provide a structured base and essential components for tasks like serving static files for traditional websites or creating web APIs for interaction in web applications.

A web API acts as a service that enables data retrieval and storage to and from the server or backend. For example, you might use a web API to handle user creation, retrieval, and related functionalities.

Now, let's explore some popular web frameworks for Node.js. Express is a standout choice, well-known for its simplicity and extensive testing. It offers a straightforward and reliable option for developers.

Another notable framework is Sails, which extends beyond a single framework and includes sub-frameworks like an Object Relational Mapper (ORM). This feature-rich framework simplifies database access and provides additional functionalities, making it a comprehensive choice.

Lastly, there's Koa, the most modern framework among those discussed. It offers a contemporary approach to web development and is worth exploring for its innovative features.

In the following sections, we'll examine each of these frameworks - Express, Sails, and Koa - to understand their features and capabilities in greater detail.

**Express**

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/8ba0d40e-d82b-46c8-970b-dbb2fcb02363)

Let's start exploring the first web framework built for Node by visiting expressjs.com. As we scroll down the website, we notice that Express.js offers support for both web applications and web APIs. The term "web application" can sometimes be confusing, as it may not be clear whether it refers to the front end or back end. When we think of applications, we often associate them with functionalities running in browsers or on mobile devices. However, these applications often need to communicate with a server for tasks like user authentication or fetching data to display.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/16835378-d603-432b-befa-97a4624496f2)

A web application integrates functionalities across both the front end and back end throughout the entire application. Consider platforms like Twitter, where the inability to fetch tweets from the back end would severely impact functionality. Express.js, functioning within Node, focuses on the back end. Despite its back-end focus, Express.js plays a crucial role in the overall application, facilitating communication with the back end.

It's important to highlight that Express.js benefits from extensive community support and thorough online documentation due to its longstanding presence in the development community.

**Socket.io**

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/55d917ef-4471-46d7-b9d6-a485cf9d308c)

Socket.io enables real-time, two-way, event-driven communication, overcoming a limitation in Express, which only allows the client to initiate requests to the server. With Socket.io, bidirectional communication is possible, allowing the server to push notifications and data to the client when specific events occur.

This mechanism consists of two parts: a client-side library for browsers and a server-side library for Node.js. Both libraries have nearly identical APIs and operate in an event-driven manner, similar to Node.js. In our upcoming demonstration application, we'll delve into how this functionality works. Let's move forward and create the demo application using these frameworks.

# ReactJS

## Introduction To React
------------------------

**What is React?**

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/2d25a333-9c49-4c41-b704-2a6f87392b5b)

React, a JavaScript library for building user interfaces, was created by Facebook and became open source in March 2013. Since its inception, React has expanded beyond web development, leading to the creation of React Native. This tool allows developers to build native mobile applications using React. 

When delving into React, the React Docs are invaluable resources. They are regularly updated and exceptionally well-written. Additionally, staying informed through the React blog provides insights into the latest releases and plans from the React team.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/d88d4a6f-09a8-478e-96db-b528901fdfaa)

Aside from its widespread adoption, React's appeal stems from the enjoyable user experience it provides and the efficiency it offers through its component-based architecture. Leading companies such as Twitter, Netflix, and Microsoft choose React not only for its popularity but also for its ability to streamline the development of impressive products for both web and native platforms.

![image](https://github.com/MihlaliKota/Intro-To-JavaScript/assets/133135575/8ea6b515-f247-46ce-8bba-5a98d9744d04)

