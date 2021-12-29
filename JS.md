# Javascript CheatSheet

## Main brackets

- `{ }`: is mainly used for `________`
- `( )`: is mainly used for `________`
- `[ ]`: is mainly used for `________`

## Javascript Basics

**Comments**
Comments in javascript are in the following format

```js
/* This 
is
a 
multiline
comment */

// this is a single line comment
```

**Variables and constants**
variables -> `let`
`___`: for variables
`___`: for constants

```js
// to create a new variable
________;
// to create a new constant
________;
```

**Main Types:**

```js
// Number:
let a = _____;
// String:
let b = _____;
// Boolean:
let c = _____;
```

**Print**
To print out on the console

```js
// 1. printing string
______.log(_____Hello World_____); // -> Hello World

// 2. printing values inside stored variables or constant
const pi = 3.14;
______.log(pi); // 3.14

// 3. printing more than one element,
const x = 5;
const y = 10;
______.log(____________________); // 5 Hello World 10

// 4. console.log adds one line after it finishes
______.log(); // will just print an empty new line
```

### Basics

#### Strings

Anything in javascript between `" "` or `' '` or back ticks ` `` ` is called a string
Every text should be between quotation marks.

**Special Characters**

```js
console.log("________"); // prints a new line
console.log("________"); // prints a tab   space
console.log("________"); // prints a single back slash \
console.log("________"); // prints a single quotation mark "
```

**String Interpolation**
To add values inside a string we use the back tics `` `TEXT ${VARIABLE or COMPUTATION} TEXT` ``

```js
const x = 1;
const y = 100;
console.log(`__________`); // prints: x:1, y:100
console.log(`__________`); // prints: 101
```

**Mathmatical operations**

```js
// addition
10 _ 5

// subtraction
10 _ 5

// multiplication
10 _ 5

// division
10 _ 5

// remainder: The reminder of the division
10 _ 5

```

#### If statement

**Logical operations**

```js
// Equals
"5" __ 5 // returns true

// Strictly Equals (Better usage: returns true if same value, same type)
"5" ___ 5 // returns true

// doesn't equal
5 __ 5 // returns false

// greater than
10 _ 5 // returns false

// greater than or equal
10 __ 10 // returns true

// less than
10 _ 5 // returns false

// less than or equal
10 _ 5 // returns false


// connects 2 booleans, both of them should be true to make the final result true
10 > 5 __ "Hello" == "Hi" // returns false, because the second one is false

// connects 2 booleans, one of them should be true to make the final result true
10 > 5 __ "Hello" == "Hi" // returns true, because the first one is true
```

**If Statement**

```js
// The condition inside the () should return either true or false
const x = 5;
___(x === 5){
  // statement that will be executed if the condition was true
}

// You can link the if statement with else to execute if the condition was false

const x = 5;
if(x!=5){
  // do job 1
}
____{
  // do job 2
  // This code will only be execute if only the condition inside the if didn't work
  // you don't put a condition after the else statement
}

// The if chain, only one of the following jobs will be executed
if(CONDITION){
  // job 1
}
____ __(CONDITION 2){
  // job 2
}
____ __(CONDITION 2){
  // job 3
}
else{
  // job 4
}
```

There are some rules for the if chain

1. You can only have `else if`s between if and else
2. You cannot add `else` after `else`
3. One job only the if chain will be executed, even if the other `else if`s conditions where true

**Reminder %**
We use the reminder `%` for couple of usages, most importantly, knowing even or odd numbers.
Even numbers will return true on the following statement

```js
const x = ???
// if you want to check if x is even, you do the following condition
if(___________){
  // will only be executed if x was event
}
```

---

# Functions

You deal with functions in 2 main things

1. Function creation
2. Function execution (invoking)

```js
// 1. function creation
________ functionName(){
  // This code will be executed when you call the function
}

// 2. To invoke the function
functionName()
```

**parameters and arguments**

- We call them parameters from the outside when we call the function
- We call them arguments from the inside when we create the function

```js
// 1. Function that takes multiple arguments
function foo_________{
}

// 2. Calling the function and passing multiple parameters
______________________


```

**Return**
A function can return using the command `_______` by the end of the function

```js
// this function for example returns the square of any number you plug it
function square(x){
  ______ x * x;
}
console.log(square(4)) // this will log 16
```

> **COMMON MISTAKE**
> When we return, we use the console.log to log the returned value. Lots of times, we do the mistake of trying to console.log inside the function.

---

# Arrays

You can put groups of elements

```js
// New array
let numbers = ___ADD_ANY_NUMBER_HERE___;
```

**Accessing elements**

```js
const array = [100, 90, 80, 40];

// To access the first element
array____;

// To access the second element
array____;
//
```

**Length**

```js
const array = [100, 90, 80, 40];

array._____; // returns number of elements in the array
console.log(array.____); // prints number of elements in the array
//
```

**Length usages: Getting the last element in the array**

```js
const array = [100, 90, 80, 40];

// to get the last element in the array
array[__________];
```

**push and pop**

```js
array._____; // adds a new element
array._____; // removes the last element
//
```

# Loops

There are 2 main loops

1. `____` loop
2. `____` loop

```js
____(condition){
  // keeps looping while the condition is true
}

___(let i=0; i<10; i++){
  // initializes a counter
  // keeps looping while the condition is true
  // and increments on every loop
}
```

# Iteration Methods And Arrow Functions

### Arrow functions

```js
// the function way
function foo() {}
// the arrow function way
___________;
___________;
___________;
```

### Iteration Methods

- Iteration methods work on ******\_\_\_\_****** only!
- All iteration methods go over evrey single element of the array
- Iteration methods take a function that has a parameter of the current value of the array. Preferred to use arrow function inside it.

```js
array.SOME_ARROW_FUNCTION((element) => {
  // Whatever action you want to perform on every element
  // Most arrow functions will require you to return something
});
```

The following are the main iteration methods

1. `._______`: just goes over all the elements, doesn't return anything, and doesn't require you to pass a function that returns anything
2. `.____`: returns a filtered copy of the array that is based on a condition that you return from the function you pass it.
3. `.____`: returns a transformed copy of the array that is based on a returned shape of every element that you return from the function you pass it
4. `.____`: looks exactly like `.filter`, but it only returns the first element that matches the condition
5. `.____`: looks exactly like `.find`, but it only returns true if it finds 1 element that matches the condition
6. `.____`: returns a single value that is compiled throught the whole array using `previous` and `current` values being passed in passed function. We usually use it to get the sum

```js
const array = [10, 20, 30, 40, 50, 60];
array.___((e) => e / 10); // returns a transformed array equals to [1,2,3,4,5]
array.___((e) => e <= 30); // returns a filtered array equals to [10, 20, 30]
array.___((e) => e === 20); // returns 20
array.___((e) => e === 20); // returns true
array.___((prev, current) => prev + current); // returns the sum of the array (210)
```
