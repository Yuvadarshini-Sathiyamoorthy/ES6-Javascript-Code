# ES6-Javascript-Code

## Exercise 1: Let and Const
### Problem Statement:

Create two variables using let and const. The let variable should be named age and set to 30. The const variable should be named name and set to "Alice". Try to reassign the name variable and observe what happens.

### Hint/Explanation:

ES6 introduced let and const for declaring variables. let is used for variables that can change, while const is for variables that should remain constant.

### Solution:

let age = 30;
const name = "Alice";
name = "Bob"; 
### Output:
![1](https://github.com/Yuvadarshini-Sathiyamoorthy/ES6-Javascript-Code/assets/93482485/5f43b46b-7974-4d1e-bdff-f24664ae1a0c)

## Exercise 2: Arrow Functions
### Problem Statement:

Convert the following function into an arrow function.

function add(a, b) {

return a + b;
}

### Hint/Explanation:

Arrow functions provide a concise syntax and lexically bind the this value.

### Solution:
const add = (a, b) => a + b;
### Output:
![2](https://github.com/Yuvadarshini-Sathiyamoorthy/ES6-Javascript-Code/assets/93482485/2c0fe416-3196-4a65-98a2-6782140232d5)


## Exercise 3: Template Literals
### Problem Statement:

Use a template literal to print "Hello, Alice! Your age is 30." using the variables name and age.

### Hint/Explanation:

Template literals allow embedded expressions and multi-line strings.

### Solution:
console.log(`Hello, ${name}! Your age is ${age}.`);
### Output:
![3](https://github.com/Yuvadarshini-Sathiyamoorthy/ES6-Javascript-Code/assets/93482485/e1918de6-2e52-4767-bda8-632bd8cce861)



## Exercise 4: Destructuring Objects
### Problem Statement:

Given an object { firstName: "Alice", lastName: "Johnson" }, use object destructuring to extract firstName and lastName into variables.

### Hint/Explanation:

Destructuring allows you to unpack values from arrays or properties from objects.

### Solution:
const person = { firstName: "Alice", lastName: "Johnson" };
const { firstName, lastName } = person;
### Output:
![4](https://github.com/Yuvadarshini-Sathiyamoorthy/ES6-Javascript-Code/assets/93482485/0070f30a-ad2a-4378-97b2-8cb6a40eadc4)



## Exercise 5: Destructuring Arrays
### Problem Statement:

Given an array [1, 2, 3, 4, 5], use array destructuring to create variables first and second for the first two elements.

### Hint/Explanation:

Array destructuring works similarly to object destructuring but with array elements.

### Solution:
const numbers = [1, 2, 3, 4, 5];
const [first, second] = numbers;
### Output:
![5](https://github.com/Yuvadarshini-Sathiyamoorthy/ES6-Javascript-Code/assets/93482485/6eeccbc8-8ecc-4b8b-95e4-5ef01cb6f8c2)

## Exercise 6: Spread Operator
### Problem Statement:

Combine two arrays [1, 2, 3] and [4, 5, 6] into a new array using the spread operator.

### Hint/Explanation:

The spread operator allows an iterable (like an array) to be expanded in places where zero or more arguments or elements are expected.

### Solution:

const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const combined = [...arr1, ...arr2];
### Output:
![6](https://github.com/Yuvadarshini-Sathiyamoorthy/ES6-Javascript-Code/assets/93482485/d19b6a1c-f601-4579-9002-a50bdef54da5)

## Exercise 7: Rest Parameters
### Problem Statement:

Write a function that takes multiple arguments and returns their sum using rest parameters.

### Hint/Explanation:

Rest parameters allow us to represent an indefinite number of arguments as an array.

### Solution:
const sum = (...numbers) => numbers.reduce((acc, current) => acc + current, 0);
### Output:
![7](https://github.com/Kadinsamson/ES6-Javascript/assets/94525955/c9a192d3-68bc-43c2-8566-a75aa86bcd2e)


## Exercise 8: Default Parameters
### Problem Statement:

Create a function greet(name, greeting = "Hello") that greets a person. If no greeting is provided, it should default to "Hello".

### Hint/Explanation:

Default function parameters allow named parameters to be initialized with default values if no value or undefined is passed.

### Solution:
const greet = (name, greeting = "Hello") => ${greeting}, ${name}!;
### Output:
![8](https://github.com/Yuvadarshini-Sathiyamoorthy/ES6-Javascript-Code/assets/93482485/f35e32ec-d5e6-4572-8754-f1f93589a363)

## Exercise 9: Classes and Inheritance
### Problem Statement:

Create a class Animal with a constructor setting the name property. Then, create a subclass Dog that extends Animal and adds a bark method.

### Hint/Explanation:

ES6 classes are syntactical sugar over JavaScript's existing prototype-based inheritance. The extends keyword is used for class inheritance.

### Solution:

class Animal {
    constructor(name) {
        this.name = name;
    }
}

class Dog extends Animal {
    bark() {
        return Woof! My name is ${this.name};
    }
}
### Output:
![9](https://github.com/Yuvadarshini-Sathiyamoorthy/ES6-Javascript-Code/assets/93482485/1593aef2-01d5-43ec-853b-5c0faef72955)


## Exercise 10: Promises and Async/Await
### Problem Statement:

Create a function waitAndReturn that returns a Promise which resolves with the string "Done" after 2 seconds. Then, use async/await to call this function and log the result.

### Hint/Explanation:

Promises are used for asynchronous computations. Async/await is syntactic sugar for working with Promises in a more synchronous fashion.

### Solution:

const waitAndReturn = () => new Promise(resolve => setTimeout(() => resolve("Done"), 2000));
async function run() {
    const result = await waitAndReturn();
    console.log(result);
}
run();

### Output:
![10](https://github.com/Yuvadarshini-Sathiyamoorthy/ES6-Javascript-Code/assets/93482485/0ac567bc-bbe5-4b67-8ecc-60a45f128b2f)

