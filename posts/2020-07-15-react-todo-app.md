---
title: "[4] React - Todo app"
date: "2020-07-15"
categories:
  - "react"
tags:
  - "app"
  - "application"
  - "code"
  - "coding"
  - "github"
  - "javascript"
  - "npm"
  - "ohjelmointi"
  - "programming"
  - "react"
  - "todo"
  - "website"
coverImage: "../static/img/images/Screenshot-2020-07-14-at-16.18.49.png"
---

Finally, I have some time to write about my experience with React. When I am thinking about all the things I have learned over the last year, React seems to be the most tricky part of web development so far. I watched a bunch of videos and read a lot of everything. And even so, I don’t feel particularly confident in dealing with it.

I guess that the reason is not the complexity of React as a concept, but rather my insufficient understanding of the basics of JavaScript and things related to it. Learning to code turned out to be, at the same time, surprisingly inspiring but also difficult and multilayered. It also differs a lot from my entire previous student experience.

Anyway, in the last few days, I have been working on a React [Todo application](https://proj.create-react-app.com/todo/). As you can see, the functionality of the app is quite limited at the moment. Right now it is only possible to create new tasks, mark tasks as done, or delete them. Nevertheless, I already have on my mind a few options for future development. First of all, I would like to add a possibility to edit tasks and restore them from the trash. Then, there could be some sort of calendar integration, or, at least, the ability to schedule tasks by days. Express could also be added in the future since now there is only local storage for storing information.

The code of an application is available at my [GitHub](https://github.com/villivald/proj/tree/master/todo/code).

The basic configuration of my project was as follows:

```
npx create-react-app APP_NAME

npm i -D prettier
--> .prettierrc --> {}

npm install -D eslint eslint-config-prettier
--> .eslintrc.json -->
{
  "extends": [
    "eslint:recommended",
    "plugin:import/errors",
    "plugin:react/recommended",
    "plugin:jsx-a11y/recommended",
    "prettier",
    "prettier/react"
  ],
  "rules": {
    "react/prop-types": 0,
    "no-console": 1,
    "react-hooks/rules-of-hooks": 2,
    "react-hooks/exhaustive-deps": 1
  },
  "parser": "babel-eslint",
  "plugins": ["react", "import", "jsx-a11y", "react-hooks"],
  "parserOptions": {
    "ecmaVersion": 2018,
    "sourceType": "module",
    "ecmaFeatures": {
      "jsx": true
    }
  },
  "env": {
    "es6": true,
    "browser": true,
    "node": true
  },
  "settings": {
    "react": {
      "version": "detect"
    }
  }
}

--> .gitignore -->
node_modules/
.DS_Store
.cache/
dist/
coverage/
.env

npm install -D babel-eslint eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react

npm i -D eslint-plugin-react-hooks

npm install -D babel-eslint @babel/core @babel/preset-env @babel/plugin-proposal-class-properties @babel/preset-react
```

I also made some minor changes to my website. There are screenshot and links below:

![](images/Screenshot-2020-07-14-at-16.19.26-1024x541.png)

[https://create-react-app.com/www/](https://create-react-app.com/www/)

[https://proj.create-react-app.com/](https://proj.create-react-app.com/)

[https://villivald.github.io/proj/](https://villivald.github.io/proj/)
