---
title: "[9] A Brand New Website and a Lot of React"
date: "2020-09-29"
categories: 
  - "js"
  - "react"
  - "site"
  - "studies"
tags: 
  - "css"
  - "html"
  - "javascript"
  - "react"
  - "site"
  - "studies"
  - "website"
  - "www"
coverImage: "Screenshot-2020-09-26-at-20.00.35.png"
---

So, as it may be understood from the title of this post, I have made a [new website](https://proj.create-react-app.com/) for my projects. This is not exactly a portfolio or a CV, but something like that. There I put everything that I do during [my studies at the university](https://create-react-app.com/my-studies-at-the-university/) and the self-studies.

### v. 1 - Skeleton

The [first version](https://old.create-react-app.com/Projects/Skeleton/index.html) of the website was made almost a year ago as a web programming [course](https://opetustarjontahaku.lab.fi/search.php#result-13407) assignment. That time I used [Skeleton](http://getskeleton.com/), which is a very simple responsive CSS boilerplate, not so powerful as Bootstrap, but much easier to use. This version of the site was not so fancy, and, in a big way, just a "copy/paste" project from different tutorials.

![](images/Screenshot-2020-09-29-at-16.04.39-1024x648.png)

### v. 2 - HTML, CSS, JS

After a few months, I realized that I want to make a more "stylish" [website](https://old.create-react-app.com/), for which I will not be so ashamed and even can show to someone. That time I decided not to use any kind of frameworks, and go with just HTML, CSS, and JS. I used a flexbox for styling components and implemented some more complicated things (e.g., glitching logo) if you compare it to the previous version. Anyway, the result turned out not to be so impressive.

![](images/Screenshot-2020-09-29-at-16.04.51-1024x520.png)

### v. 3 - React

Finally, about two weeks ago, I started to work on the [current version of the website](https://proj.create-react-app.com/). I decided not to rework the previous versions, but to make it all over again from the scratch. This time I took React as a web framework. I like React for the possibility to write JSX, the hooks system, and the variety of third-party libraries.

![](images/Screenshot-2020-09-28-at-22.30.55-1024x538.png)

At the moment, I use the VS Code as an editor, and I am also using several add-ons for my VS Code setup, e.g., Prettier, ESLint, Bracket Pair Colorizer, etc. I tried many color themes as well but barely could use nothing other but standard Dark+.

I divided my project into many parts, which is quite typical for React development. There are all the components that are placed on the main App.js component:

```
├── Board.js
├── ChipCloud.js
├── Drop.js
├── Dropdown.js
├── Footer.js
├── Grid.js
├── GridItem.js
├── Menu.js
├── Screens.js
├── Stats.js
├── Switch.js
├── Timeline.js
└── Toggle.js
```

In this project, I noticed that grid and flexbox could work in symbiosis, so I used both. As third-party libraries, I used [Material - UI](https://material-ui.com/), [Ant Design](https://ant.design/), and [React Bootstrap](https://react-bootstrap.github.io/). Mostly it is very convenient for styling the drop-down menu, buttons, and so on. This time it was also a bit difficult to make all media queries since the site comprises a lot of components. So it took some amount of time to realize that the media queries for Safari could be done like that:

```
@media not all and (min-resolution: 0.001dpcm) {
  @media only screen and (max-width: 1900px) {
  }
}
```

[The website (29.09.20)](https://proj.create-react-app.com/)

[Website source code on GitHub](https://github.com/villivald)
