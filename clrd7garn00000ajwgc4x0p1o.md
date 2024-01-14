---
title: "Functions and types in JavaScript."
seoTitle: "Mastering JavaScript Functions: Boost Your Coding Skills with Practice"
seoDescription: "Explore the diverse world of JavaScript functions in this insightful blog. Discover key concepts, practical tips, and enhance your coding skills. Dive into"
datePublished: Sun Jan 14 2024 07:59:07 GMT+0000 (Coordinated Universal Time)
cuid: clrd7garn00000ajwgc4x0p1o
slug: functions-and-types-in-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1705156555336/08347980-b1f4-4dba-be19-96c818cbf763.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1705218442826/40687609-0a9a-4b05-9ffa-853030b792c4.jpeg
tags: functions, javascript, types

---

## Functions:

Functions is a reusable block of code that performs a specific task or set of tasks.

### Uses:

* Write once use many times, follows DRY principle (Do Not Repeat Yourself).Function defined once can be called multiple times.
    
* Also, this saves lot's of time
    
* The code is easily maintained and easily debugged.
    

---

### Some difference between Loops and Functions

Loops to execute set of code. Let's read how different loops are compared to functions.

* Loops iterate through a block of code until a specified condition is satisfied. In contrast, functions execute specific tasks independently of conditions.
    
* In loops, a block of code is repetitively executed any number of times until a specified condition is met. In contrast, a function needs to be explicitly called to repeat its execution, and it may not necessarily be continuous. Each time the function is nvoked, it executes the designated block of code.
    

Functions can accept parameters and perform computations, whereas in loops, the capability to take parameters and compute is not available.

---

## Let's explore various functions:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705160149948/628eef74-16f9-4180-bd60-176abe7d288e.webp align="center")

### **Function Declarations:**

Functions are created using the `function` keyword, and they are typically given a name. This is a common type of function declaration.

It involves using the `function` keyword followed by a name, parentheses for parameters `()`, and curly brackets `{}` inside where the block of code is written.

In JavaScript, an arbitrary value can be returned from a function. <mark> If a function doesn't explicitly have a </mark> `return` <mark> statement, it implicitly sends </mark> `undefined`<mark>.</mark>

```javascript
function functionName(){
// Logic of code
console.log("Read the Blog completley")
}
functionName();
```

> Output: Read the Blog compleltely

---

### Function Expression:

Function expressions are defined using the keyword 'function,' they lack a specified name. Typically, they are assigned to a variable to facilitate invocation.

**Function expressions can be named or anonymous.**

```javascript
const largestNo=function(a,b){
    if(a>b){
             return a;
     }else if(a<b){
           return b;
     }else{
        console.log("Both are equal");
        return a;
        }
    }
console.log(largestNo(5,7));

//Output
7
```

---

### Arrow Functions:

Arrow functions represent the most concise method of writing functions.

They forego the use of the 'function' keyword and lack a designated function name. Instead, their syntax includes parentheses '()' for parameter reception and '=&gt;' hence name Arrow Function and definition written inside '{}' braces.

```javascript
const square=(a)=>{
    return a*a;
}
console.log(square(3));

//Output
9
```

---

### **Anonymous Function:**

Function with no name.It is created on the fly and does not have an identifier.

```javascript
let sum = function (a, b) {
  return a + b;
};
```

---

### Immediately invoked Function:

These are the functions that are defined and invoked immediately.

They are written inside ()(); Inside first () function definition is written and in second () parameter is passed.

```javascript
console.log((function (a){
    return a*a;    
  })(9) );
//Output
81
```

***<mark>Note: After function invoking ';' (terminating) the fucntion is important.</mark>***

---

### Generator Functions:

Functions that can be paused and resumed, producing a sequence of values over time.

They are used with keyword '<mark>function*</mark>' and '<mark>yield'</mark> keyword is used to pause the execution of the generator function and can also be used **to send a value back to the caller.**

```javascript

function*  count(p){
  
   while(true){
      yield p++;
   }
}
let c=count(15);
console.log(c.next().value);
console.log(c.next().value);
console.log(c.next().value);

//Output
16
17
18
```

---

### **Callback Functions:**

A **callback function** is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.

<mark>Mostly used for asynchronous operations like Database call, network call or fetch data etc.</mark>

```javascript
function square(u, callback) {

 console.log(callback(u)) ;
}

square(8, function (u) {
 return u*u;
});

//Output
64
```

---

### Async Function:

An `async` function in JavaScript is a function that operates asynchronously, allowing for the use of the `await` keyword to pause the execution of the function until a Promise is settled.

This makes it easier to work with asynchronous code in a more synchronous-looking manner, improving code readability.

```javascript
function delay(ms) {
  return new Promise(resolve => setTimeout(resolve, ms));
}

async function exampleAsyncFunction() {
  console.log('Start');

  await delay(2000);

  console.log('After 2 seconds');
}

exampleAsyncFunction();

//Output
Start  (after 2 second)
After 2 seconds
```

---

## Thanks for reading! I would love to hear your thoughts on the blog.

### *<mark>Which function do you use more?</mark>*

Connect me on X [here](https://twitter.com/SHRIvatsa_desai).