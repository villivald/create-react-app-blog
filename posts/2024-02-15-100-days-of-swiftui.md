---
title: "[31] 100 Days of Swift UI (upd. 21.02.24)"
date: "2024-02-15"
categories:
  - "swift"
tags:
  - "swift"
  - "swiftui"
  - "100daysofcode"
  - "mobile"
  - "ios"
  - "apple"
coverImage: "../static/img/images/CoverImages/31.webp"
---

### 100 Days of SwiftUI

![100 Days of SwiftUI - logo](https://www.create-react-app.com/static/img/images/31/logo.webp)

Today I started the [100 Days of SwiftUI](https://www.hackingwithswift.com/100/swiftui) course by [Paul Hudson](https://mastodon.social/@twostraws). I've been wanting to learn iOS development for a while now, and I think this is a brilliant opportunity to do so. I'm excited to see what I can build with it.

This post will be updated as I progress through the course. I will be adding the new things I learn and the projects I build as I go along. I will try not to skip any days, but we will see how it goes.

So far, all my experience with Swift is limited to this [Frontend Masters tutorial](https://frontendmasters.com/courses/swift-ios/) by [Maximiliano Firtman](https://firt.dev/). So, I have some basic knowledge of the language and the framework, but I'm still a beginner.

In addition to this post, my progress can be followed on:

- [Mastodon](https://notacult.social/@villivald) (updates and thoughts)
- [Github](https://github.com/villivald/100_Days_of_SwiftUI/tree/main) (code)

#### Day 1: Variables, constants, strings, and numbers

![100 Days of SwiftUI - Day 1](https://www.create-react-app.com/static/img/images/31/day1.webp)

Today, I reviewed some basic concepts of Swift. I already knew about variables and constants, but I learned a couple of new things as well. For example, I learned about multi-line strings (`"""`), type safety (1 + 2.0 = error), and a couple of useful methods (`uppercased()`, `hasPrefix()`, `isMultiple(of:)`). Of course, the first day was an easy one, but nevertheless, it was a good refresher.

#### Day 2: Booleans, string interpolation, and checkpoint 1

This day's material covered such topics as booleans and string interpolation. I noticed that the interpolation syntax in Swift is more elegant and a bit more powerful 🤔 than in Javascript, so that's interesting. At the end of the lesson, I finished the first checkpoint assignment - converting temperature from °C to °F (classic).

#### Day 3: Arrays, dictionaries, sets, and enums

Day 3 had a surprisingly large amount of new information. I learned a couple of previously unknown concepts, such as dictionaries, sets, and enums. I believe that each of them might have particular use cases, but I'm not sure yet when to use them in practice. I suppose it will become clear in the nearest feature.

So far, it seems that the first two weeks of the course will be directed towards learning/refreshing the basics of Swift as a language. After that, we will start using SwiftUI and building something more tangible. I hope that, at this point, the process will become more practical.

#### Day 4: Type annotations and checkpoint 2

![100 Days of SwiftUI - Day 4](https://www.create-react-app.com/static/img/images/31/day4.webp)

Today's lesson was brief, yet it covered an important topic - type annotations. From my point of view, in Swift, it works exactly the same way as in Typescript. I am not 100% sure about type inference, so I will check it later.

The second checkpoint assignment was about returning unique values from the array by converting it to a set. It also seems like a task that can be accomplished almost the same way in Javascript or Typescript.

As you can see from today's image, I still use VSCode for Swift development. I am not sure if it's the best option, and I will probably switch to Xcode sooner or later.

#### Day 5: If, switch, and the ternary operator

##### &&

#### Day 6: Loops, summary, and checkpoint 3

I accidentally skipped a day yesterday, so I am catching up today with two sections. The first (Day 5) was about conditionals - `if`, `switch` and the ternary operator (`2 > 1 ? "Yes" : "No"`). Once again, it feels pretty much the same as in Javascript, except for some minor differences - `Int` and `Double` can not be compared directly in Swift, and `switch` statements must be exhaustive, i.e., go through all the cases or have a `default` case.

Day 6 was dedicated to loops - `for` and `while`. I learned about ignoring the value (`_`), excluding the last entry (`..<`), generating a random number (`Int.random(in: 1...10)`), and using `break` and `continue` statements to control the flow of the loop.

The third checkpoint contained a FizzBuzz task, which I solved at first by using the `%` operator. Then, I realized that Swift has a `.isMultiple(of:)` method and refactored the code to use it.

#### Day 7: Functions, parameters, and return values

It is a wrap for the first week of the course. Today's lesson was an introduction to functions in Swift. I learned the basic syntax, as well as some handy tricks, such as omitting the `return` keyword for single-expression functions, using external parameter names, and skipping the parameter label with `_`.

---
