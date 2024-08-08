# What is JavaScript?

- JS is a synchronous single-threaded programming language.
- JS is a lightweight object-oriented programming language.

<br><br>

# What is Call?

- The stack maintains the order of execution of execution contexts.
![Call Stack](images/callStack.png)

<br><br>

# JavaScript Primitive Data Types

### Overview

In JavaScript, data types are classified into primitive and non-primitive types.  Primitive data types represent single values and are immutable, meaning their values cannot be changed once created.

## Primitive Data Types

### 1. String
**Description**: Represents a sequence of characters used to store and manipulate text. 
- **Examples**: 
  - `"Hello, world!"`
  - `'JavaScript'`
  - `` `Template literal` ``

### 2. Number
**Description**: Represents both integer and floating-point numbers. It includes standard numeric values.
- **Examples**: 
  - `42`
  - `3.14`

### 3. BigInt
**Description**: Represents integers with arbitrary precision. It allows for the representation of very large integers beyond the range of the `Number` type.
- **Examples**: 
  - `9007199254740991n`

### 4. Boolean
**Description**: Represents a logical value that can be either `true` or `false`. Often used in conditional statements and loops.
- **Examples**: 
  - `true`
  - `false`

### 5. Undefined
**Description**: Represents a variable that has been declared but has not yet been assigned a value. It signifies the absence of a value.
- **Examples**: 
  - `let x; // x is undefined`

### 6. Null
**Description**: Represents the intentional absence of any object value. It is used to denote a deliberate non-value or empty value.
- **Examples**: 
  - `let y = null;`

### 7. Symbol
**Description**: Represents a unique and immutable value often used as a key for object properties, ensuring that property keys are unique.
- **Examples**: 
  - `Symbol('description')`
<br><br>
## Characteristics of Primitive Data Types

- **Immutability**: Primitive values cannot be altered once they are created. For example, modifying a string results in the creation of a new string rather than changing the original one.
- **Pass by Value**: When a primitive value is assigned to a variable or passed to a function, a copy of the value is made. Changes to the variable or parameter do not affect the original value.
- **Simple Representation**: Primitive types represent a single value, unlike non-primitive types which can hold collections or more complex structures.

<br>

**Additional Resources**: [JavaScript Data Types - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)



<br><br>


# JavaScript Non-Primitive Data Types

### Overview

In JavaScript, non-primitive data types are more complex types that can hold collections of values or more intricate structures. Unlike primitive data types, non-primitive types are mutable, meaning their values can be modified. They represent more complex entities and include objects, arrays, and other data structures.

## Non-Primitive Data Types

### 1. Object
**Description**: Represents a collection of key-value pairs where each key is a string (or Symbol) and each value can be any data type. Objects are used to store and organize data in a structured way.
- **Examples**: 
  - `{ name: "Alice", age: 25 }`
  - `const person = { firstName: "John", lastName: "Doe", age: 30 };`

### 2. Array
**Description**: A special type of object used for storing ordered collections of values. Arrays are indexed by numbers and can hold multiple values of any type.
- **Examples**: 
  - `[1, 2, 3, 4, 5]`
  - `const colors = ["red", "green", "blue"];`

### 3. Function
**Description**: A type of object that can be invoked to perform an action or compute a value. Functions are first-class objects in JavaScript, meaning they can be passed as arguments and returned from other functions.
- **Examples**: 
  - `function greet() { console.log('Hello!'); }`
  - `const add = (a, b) => a + b;`

### 4. Date
**Description**: Represents dates and times, allowing for the manipulation and formatting of date-related information.
- **Examples**: 
  - `new Date()`
  - `const now = new Date();`

### 5. RegExp
**Description**: Represents regular expressions, which are patterns used for matching and manipulating strings based on specific patterns.
- **Examples**: 
  - `/^\d+$/`
  - `const regex = /hello/i;`

### 6. Map
**Description**: A collection of key-value pairs where both keys and values can be of any type. Maps remember the original insertion order of the keys.
- **Examples**: 
  - `new Map([['key1', 'value1'], ['key2', 'value2']])`
  - `const map = new Map(); map.set('name', 'Alice');`

### 7. Set
**Description**: A collection of unique values. Sets automatically remove duplicate values and maintain the insertion order.
- **Examples**: 
  - `new Set([1, 2, 3, 1])`
  - `const set = new Set(['apple', 'banana', 'apple']);`

### 8. WeakMap
**Description**: Similar to `Map`, but keys must be objects and are held weakly, meaning they can be garbage collected if there are no other references to the objects.
- **Examples**: 
  - `new WeakMap()`
  - `const weakMap = new WeakMap();`

### 9. WeakSet
**Description**: Similar to `Set`, but only stores objects and holds them weakly.
- **Examples**: 
  - `new WeakSet()`
  - `const weakSet = new WeakSet();`

## Characteristics of Non-Primitive Data Types

- **Mutability**: Non-primitive types are mutable. Their values can be changed after creation.
- **Reference**: When a non-primitive value is assigned to a variable or passed to a function, a reference to the value is used. Changes to the reference affect the original value.
- **Complex Structures**: They can represent more complex data structures compared to primitive types.

**Additional Resources**: [JavaScript Data Types - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)


<br><br>


# Dynamic Typing in JavaScript

### Overview

**Dynamic typing** is a feature of programming languages where variables do not have fixed types. In dynamically typed languages, the type of a variable is determined at runtime rather than at compile time. JavaScript is a dynamically typed language, meaning that variables can hold values of any type and can change types during execution.

## Key Concepts

### 1. Type Flexibility
In JavaScript, variables can hold different types of values at different times. You can assign a number to a variable and later assign a string to the same variable without any type errors.

**Example:**

```javascript
let variable = 42;         // Initially a number
console.log(typeof variable); // "number"

variable = "Hello";        // Now a string
console.log(typeof variable); // "string"
````
<br><br>

# JavaScript Objects

### Overview

In JavaScript, an **object** is a fundamental data structure used to store collections of data and more complex entities. Objects consist of key-value pairs, where each key is a string (or Symbol) and each value can be any data type, including other objects.

## Key Characteristics

- **Key-Value Pairs**: Objects are collections of properties where each property is a key-value pair.
- **Mutable**: Objects can be modified after creation. Properties can be added, changed, or removed.
- **Dynamic**: Properties can be added or removed dynamically at runtime.
- **Prototype Chain**: Objects have a prototype from which they inherit properties and methods.

## Creating Objects

### Object Literal Notation

The most common way to create an object using object literal notation.

**Example:**

```javascript
const person = {
  firstName: 'John',
  lastName: 'Doe',
  age: 30,
  greet: function() {
    console.log('Hello!');
  }
};
```


**Additional Resources**: [JavaScript Data Types - MDN Web Docs](https://javascript.info/object)

<br><br>


