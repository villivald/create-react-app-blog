---
title: "[6] JavaScript - Map, Filter & Reduce"
date: "2020-07-28"
categories: 
  - "js"
tags: 
  - "code"
  - "filter"
  - "function"
  - "javascript"
  - "js"
  - "map"
  - "reduce"
  - "study"
coverImage: "Screenshot-2020-07-27-at-13.16.26.png"
---

I am still focusing on learning JavaScript and especially different JavaScript methods while waiting for the next academic year to begin. The first courses are due to start in early September, so it’s not so long to wait anymore. I hope that it will boost my productivity since now I feel extremely unfocused and a bit confused in the abundance of information.

Anyway, there is still certain progress in my skills. Now I will also probably write more often since I have an idea for a cycle of posts about JavaScript. The first post of this cycle was [published last week](https://create-react-app.com/5-javascript-spread-operator/) and was related to the topic of JS spread operator. In this post, I will go over some significant JavaScript methods such as map, filter, and reduce.

### Map

In this simple example of using a map(), I am creating a function **fn** that takes two arguments - name and id. Then I pass some names to the function and convert the string to the desired form by using the map method.

```
function fn(name, id) {
    console.log(id + 1, ": ", name)
}

["John", "Marie"].map(fn) 

/*
1: John
2: Marie
*/
```

Map() is also suitable for some other use cases. In the code below, I am using it to calculate the length of the elements.

```
var names = ["John", "Tom", "Tim"]

var lengths = names.map(function (name) {
    return name.length
})

console.log(lengths)

// [ 4, 3, 3 ]
```

In the last piece of code, I transform an array of numbers using the map and the sqrt methods (square root).

```
var numbers = [9, 25, 49, 100]
var x = numbers.map(Math.sqrt)

console.log(x)

// [ 3, 5, 7, 10 ]
```

### Filter

A filter() is another helpful JavaScript method. It allows us to literally filter arrays (or in this particular case - an array of objects). In the example below, I created a function that returns an array of users that are logged into our imaginary system.

```
function isLoggedIn(user) {
    return user.session != null
}
console.log([
    {userId: 42, session: "123"},
    {userId: 12},
    {userId: 58,session: "3333"}
].filter(isLoggedIn))

// [ { userId: 42, session: '123' }, { userId: 58, session: '3333' } ]
```

In the next example, I am using a filter() for sorting the elements of an array. The function returns an array of positive numbers.

```
var array = [0, 11, -7, -4, 2, 68];

var positive = array.filter(function (number) {
    return number > 0;
});

console.log(positive); // 11, 2, 68
```

### Reduce

The reduce method is a little more complex. In a few words, it allows us to calculate a single value based on the entire array. In the first example, I created a function **addToRecord** that combines the information given in the arrays.

```
function addToRecord(record, [key, value]) {
    return {
        ...record,
        [key.toUpperCase()]: value
    }
}

console.log(
    [
        ["name", "John"],
        ["age", 30],
        ["isLoggedIn", true]
    ].reduce(addToRecord, {}))

// { NAME: 'John', AGE: 30, ISLOGGEDIN: true }
```

And here we get a short implementation of factorial (5! = 1 × 2 × 3 × 4 × 5 = 120) using the reduce method.

```
let arr = [1, 2, 3, 4, 5]

let result = arr.reduce((res, current) => res * current)

console.log(result)

// 120
```

[https://create-react-app.com/](https://create-react-app.com/)

[https://proj.create-react-app.com/](https://proj.create-react-app.com/)

[https://villivald.github.io/proj/](https://villivald.github.io/proj/)
