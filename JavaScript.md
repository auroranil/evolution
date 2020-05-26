# JavaScript

## Mocha (May 1995)

## LiveScript (September 1995)

## JavaScript (December 1995)

## JScript (August 1996)

## ECMAScript 1 (June 1997)

### Math object (May be introduced earlier)

```javascript
// bulitin constants
Math.E; // roughly 2.71828
Math.PI; // roughly 3.14127

// builtin functions
Math.cos(Math.PI); // -1
Math.sin(0); // 0
```

## ECMAScript 2 (June 1998)

No new features.

## ECMAScript 3 (December 1999)

### Exception handling

```javascript
try {
    // do something that may throw an error
} catch (err) {
    // log error with err and inform client
    /// that something went wrong
}
```

### Regular expressions

```javascript
// this is a regular expression literal
var re = /Java(?:Script)?/;

"Hello JavaScript!".match(re); // returns true
"You are similar with Java in some ways, and different in other ways.".match(
    re
); // also returns true
"Say hi to jQuery too!".match(re); // returns false
```

### do-while statement

```javascript
do {
  // something
} while (/* condition */);
```

## ECMAScript 4 (July 2008)

Abandoned.

## ECMAScript 5 (December 2009)

### Strict mode

```javascript
"strict mode"; // changes the way JavaScript behaves
```

### Trim string

```javascript
" hello world   ".trim(); // becomes "hello world"
```

## ECMAScript 5.1 (June 2011)

## ECMAScript 6 (June 2015)

### let and const declarations

```javascript
let life; // we can declare a variable without initialising it
life = 42; // setting the variable to be 42
life = 496; // can change the variable's value

const PI = 3.14159265358979;
// cannot change PI after it was declared and initialised
```

### Block scope

```javascript
let i = 0;
{
    let i = 1;
    // here i is 1
}
// here i is 0
```

### Arrow functions

```javascript
const square = x => x * x;
square(5); // becomes 25

const add = (x, y) => x + y;
add(2, 3); // becomes 5
```

### Promises

```javascript
// promise which resolves
new Promise((resolve, reject) => {
    resolve({
        title: "evolution",
        description: "Shows the evolution of programming languages"
    });
})
    .then(result => {
        // do something with result
        // this function will get executed
    })
    .catch(err => {
        // log error for debugging purposes
        // this will not get executed
    });

// promise which rejects
new Promise((resolve, reject) => {
    reject({
        errorMessage: "API failed",
        errorDescription: "Failed to fetch result from API"
    });
})
    .then(result => {
        // do something with result
        // this will not execute
    })
    .catch(err => {
        // log error for debugging purposes
        // this will get executed
    });
```

## ECMAScript 7 (June 2016)

### Exponential operator

```javascript
2 ** 3; // becomes 8
2.5 ** 5.1; // roughly 107.02717
```

### Array.prototype.includes

```javascript
const squareNumbersUpTo5 = [1, 4, 9, 16, 25];

squareNumbersUpTo5.includes(3); // returns false
squareNumbersUpTo5.includes(9); // returns true
squareNumbersUpTo5.includes(36); // returns false
```

## ECMAScript 8 (June 2017)

### async functions

```javascript
const foo = async () => {
    // ... wait for three seconds ...
    return {
        title: "async functions",
        description:
            "They are Promises in disguise! This object will be wrapped in a Promise due to the async keyword specified after foo followed by the equals sign."
    };
};

const bar = async () => {
    try {
        // we use await keyword to unwrap the promise
        // to get the object
        const result = await foo(); // corresponds to .then in Promises
        // do something with result
    } catch (err) {
        // corresponds to .catch in Promises
        // some error happened
        // log it
        // inform user that something went wrong
    }
};
```

## ECMAScript 9 (June 2018)

## ECMAScript 10 (June 2019)
