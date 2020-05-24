# JavaScript

## Mocha (May 1995)

## LiveScript (September 1995) 

## JavaScript (December 1995)

## JScript (August 1996)

## ECMAScript 1 (June 1997)
Math object (May be introduced earlier)
```javascript
Math.E; // roughly 2.71828
Math.PI; // roughly 3.14127

Math.cos(Math.PI); // -1
Math.sin(0); // 0
```

## ECMAScript 2 (June 1998)

## ECMAScript 3 (December 1999)

## ECMAScript 4 (July 2008)

## ECMAScript 5 (December 2009)
Strict mode
```javascript
"strict mode" // changes the way JavaScript behaves
```

String.trim()
```javascript
" hello world   ".trim() // becomes "hello world"
```

## ECMAScript 5.1 (June 2011)

## ECMAScript 6 (June 2015)
let and const

```javascript
let life; // we can declare a variable without initialising it
life = 42; // setting the variable to be 42
life = 496; // can change the variable's value

const PI = 3.14159265358979;
// cannot change PI after it was declared and initialised
```

Block scope
```javascript
let i = 0;
{
  let i = 1;
  // here i is 1
}
// here i is 0
```

Arrow functions
```javascript
const square = x => x*x;
square(5); // becomes 25

const add = (x, y) => x + y;
add(2, 3); // becomes 5
```

Promises

```javascript
new Promise((resolve, reject) => {
    resolve({
      title: "evolution", 
      description: "Shows the evolution of programming languages" 
    });
}).then(result => {
  // do something with result
})
.catch(err => {
  // log error for debugging purposes
})

new Promise((resolve, reject) => {
    reject({
      errorMessage: "API failed", 
      errorDescription: "Failed to fetch result from API" 
    });
}).then(result => {
  // do something with result
})
.catch(err => {
  // log error for debugging purposes
})
```

## ECMAScript 7 (June 2016)
Exponential operator
```javascript
2**3 // becomes 8
2.5**5.1 // roughly 107.02717
```

## ECMAScript 8 (June 2017)

## ECMAScript 9 (June 2018)

## ECMAScript 10 (June 2019)

