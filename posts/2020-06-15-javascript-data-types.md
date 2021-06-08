---
title: "[1] JavaScript Data Types"
date: "2020-06-15"
categories:
  - "js"
tags:
  - "coding"
  - "data"
  - "javascript"
  - "newbie"
  - "webdev"
coverImage: "../static/img/images/CoverImages/1.webp"
---

In addition to my main studies, I constantly watch [FrontendMasters](https://frontendmasters.com/) courses. Those courses are mostly about JavaScript, HTML, CSS, web development in general and things like that. So in this post, I'll share some considerations about JavaScript data types.

Well, at first, there are some basic data types, like strings, numbers and booleans (true vs false):

![](https://reverent-carson-67c52e.netlify.app/static/img/codeImages/types.png)

```javascript
console.log(typeof "Test")
→ string
```

```javascript
console.log(typeof 8)
→ number
```

```
console.log(typeof true)
→ boolean
```

Then, in the following example, we can see the difference between undefined and undeclared variables. The difference is obvious enough, but at the same time, JavaScript takes both cases as undefined for some reason.

```
let x
console.log(typeof x)
→ undefined
```

```
console.log(typeof y)
→ undefined (hmm... undefined or maybe undeclared?)
```

Next, there is a group of quite different things such as an object, array and null that are in practice perceived equally.

```
let x = {}
console.log(typeof x)
→ object
```

```
let list = [1, 2, 3]
console.log(typeof list)
→ object (Array is also an object in JS)

I guess that the better way to differentiate regular objects from arrays is to use Array.isArray.
```

```
console.log(typeof null)
→ object (Wait... null is an object? 🧐 It seems to be so.)
```

There were a couple of completely new things to me as well, such as symbol and bigint. They are definitely not the things I used a lot, so I can't say anything special about them.

```
console.log(typeof Symbol("&"))
→ symbol
```

```
console.log(typeof 1n || BigInt(42))
→ bigint
```

Of course, there is also a function, which data type is a function. Yes, it was easy this time.

```
let w = (name) => { console.log(`Hi ${name}`) }
console.log(typeof w)
→ function
```

And finally, there are also several examples not directly related to JavaScript data types, but which seemed interesting to me.

```
console.log(Number("Test"))
→ NaN

let zero = -0
console.log(Object.is(zero, 0))
→ false
console.log(Object.is(zero, -0))
→ true
```

[https://create-react-app.com/](https://create-react-app.com/)

[https://proj.create-react-app.com/](https://proj.create-react-app.com/)
