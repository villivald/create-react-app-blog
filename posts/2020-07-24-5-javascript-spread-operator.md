---
title: "[5] JavaScript - Spread operator"
date: "2020-07-24"
categories:
  - "js"
tags:
  - "array"
  - "javascript"
  - "js"
  - "object"
  - "spread"
  - "syntax"
coverImage: "../static/img/images/5/Screenshot-2020-07-24-at-16.41.18.png"
---

In the last couple of days, I was trying to intensively learn JavaScript. So, in the few next posts will be some thoughts about useful functions, methods, and syntax features. Today I will start with the javascript spread operator.

#### Spread syntax

The javascript spread operator could be a pretty useful tool that saves space and improves the syntax. In the first example below, I am using it for passing **args** array to the **newArgs** on line 5. Next, on lines 7 and 8, I am passing those arrays to **fn** function.

```
fn = (x, y, z, a = 4, b = 5, c = 6) => {
  console.log(x, y, z, a, b, c)
 }
var args = [1, 2, 3]
var newArgs = [...args, "four", "five", "six"] // [1, 2, 3, four, five, six]

fn(...args) // 1 2 3 4 5 6
fn(...newArgs) // 1 2 3 four five six
```

The next example is slightly different. Here I am creating a function, which uses **…args** as a parameter. Inside the function, we have a for-loop that iterates through the list of arguments. In principle, there can be as many arguments as you need. Finally, when the function is being called, it takes all arguments that have been given, 1, 2, or 100, etc.

```
sumAll = (...args) => {
    let sum = 0
    for (let arg of args) {
        sum += arg
    }
    console.log(sum)
}

sumAll(1) // 1
sumAll(1, 2) // 3
sumAll(1, 2, 3) // 6
```

We could also use the spread operator for something like this:

Iteration through the string.

```
const str = "Hello"
var letters = [...str]
console.log(letters) // [ 'H', 'e', 'l', 'l', 'o' ]
```

Dividing an array into a number (**z**) and an object (**w**), which is, in fact, another array. (More about JS Data Types [here](https://create-react-app.com/javascript-data-types/)).

```
var [w, ...z] = [1, 2, 3]

console.log(w, z) // 1 [2, 3]

console.log(typeof(w)) // number
console.log(Array.isArray(w)) // false

console.log(z[1]) // 3
console.log(typeof(z)) // object
console.log(Array.isArray(w)) // true
```

Or even iterating through the object:

```
var object = {
    a: 1,
    b: 2,
    c: 3,
    *[Symbol.iterator]() {
        for (let key of Object.keys(this)) {
            yield this[key]
        }
    }
}

console.log(...object) // 1 2 3
console.log(typeof(object.a)) // number
```

The latest example can be also done in a following way. But in this case, it returns an array:

```
var object = {
    a: 1,
    b: 2,
    c: 3
}

var x = Object.values(object)
console.log(x); // [1, 2, 3]
console.log(typeof(x)) // object
```

[https://create-react-app.com/](https://create-react-app.com/)

[https://proj.create-react-app.com/](https://proj.create-react-app.com/)

[https://villivald.github.io/proj/](https://villivald.github.io/proj/)
