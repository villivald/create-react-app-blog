---
title: "[8] The University's Fall Semester & Mastering Zsh"
date: "2020-09-13"
categories: 
  - "shell"
  - "studies"
tags: 
  - "bash"
  - "lab"
  - "lahti"
  - "lamk"
  - "shell"
  - "studies"
  - "study"
  - "terminal"
  - "university"
  - "universityofappliessciences"
  - "zsh"
coverImage: "Screenshot-2020-09-13-at-11.47.36.png"
---

Recently my second year at the University started, and I am happy to have some well-known routine in my study life. Nevertheless, in the first part of autumn, I will have only two courses: [Orientation to Sustainability Thinking (2 ECTS)](https://opinto-opas.lab.fi/en/realization/A300CE13-3001), which is more about the sustainable picture in general and [Technical Mathematics (3 ECTS)](https://opinto-opas.lab.fi/en/realization/AT00BT69-3001), which is just a regular theoretical course in math. The first one is completely independent, and on my part, is almost done and is waiting for evaluation. The math course is a regular lecture course and will run until the end of the year. Since the end of September, I will also start another [University module](https://create-react-app.com/my-studies-at-the-university/) dedicated to web development. I am looking forward to starting this particular module since web development is what interests me most at the moment.

By the way, I keep watching some [FrontendMasters](https://frontendmasters.com/) courses, and recently I went through the [Complete Intro to Linux and the Command-Line](https://frontendmasters.com/courses/linux-command-line/) named course by [Brian Holt](https://frontendmasters.com/teachers/brian-holt/). This course was a lot of fun, and Brian is definitely one of the best teachers I have ever seen. I learned a lot about Zsh and Bash commands, such as _less_, _Touch file{1..10..2}.txt_, _rm -rf_, _ls -lsah_, _kill -9_, _whoami_, _ps aux_, _wget_, _curl_, and so on. I refreshed my knowledge about using _sudo_ and manipulating user permissions. There was as well a whole part of the course related to the Vim and Nano, and yes, now I even know how to get out of Vim. I have also learned to create and use my own simple shell scripts, like: 

```
read -p "Enter a folder name: " FOLDER

DESTINATION=~/Desktop/$FOLDER

read -p "Enter a file prefix: " FILE_PREFIX

mkdir -p $DESTINATION
cd $DESTINATION
touch ${FILE_PREFIX}{1..10}.txt
echo done
```

I have also made some changes to the basic Zsh settings on my terminal. For example, I installed the oh-my-zsh framework, which is just outstanding. It allows you to simply add plugins to Zsh. There is my list of plugins: _plugins=(git history osx web-search)_. I have also made some changes to the _.zshrc_ file, which allows the terminal to randomly choose one of my favorite Zsh themes on every boot (spaceship, robbyrussell, amuse, avit, norm, pygmalion, sunrise, wezm, ys).

![](images/Screenshot-2020-09-13-at-12.04.55-1024x820.png)

Blog: [https://create-react-app.com/](https://create-react-app.com/)

Site: [https://proj.create-react-app.com/](https://proj.create-react-app.com/)

Site (mirror on github): [https://villivald.github.io/proj/](https://villivald.github.io/proj/)
