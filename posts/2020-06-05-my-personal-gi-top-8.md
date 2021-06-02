---
title: "[0] Git"
date: "2020-06-05"
categories:
  - "git"
tags:
  - "coding"
  - "git"
  - "github"
  - "newbie"
coverImage: "../static/img/images/0/0/Screenshot-2020-06-05-at-19.06.03.png"
---

At the moment I am especially interested in [Git](https://github.com/villivald) and have recently passed two courses devoted to this technology. [One course](https://plus.tuni.fi/tie-git/v2/) was from the [University of Tampere](https://www.tuni.fi/en), which I’m going to include in my degree. And the other one is a course called [Git In-depth](https://frontendmasters.com/courses/git-in-depth/) from [Frontend Masters](https://frontendmasters.com/).

Actually, both courses were quite impressive, and I have learned a lot about Git. So, there are several points I found out and which I found particularly important as my personal top-8:

1). **A remote repository**

Adding and deleting:

![](https://reverent-carson-67c52e.netlify.app/static/img/images/0/Screenshot-2020-06-04-at-19.02.58.png)

![](https://reverent-carson-67c52e.netlify.app/static/img/images/0/Screenshot-2020-06-04-at-19.03.44.png)

2). **Branches**

With switching to a new branch and without it:

![](https://reverent-carson-67c52e.netlify.app/static/img/images/0/Screenshot-2020-06-04-at-19.05.53.png)

3). **Stashing**

There is a simple example of using stashes below. It is quite handy when you want to save some changes but do not want to commit it yet.

![](https://reverent-carson-67c52e.netlify.app/static/img/images/0/Screenshot-2020-06-04-at-19.18.18.png)

4). **Tags** are not something I use a lot, but anyway I think they could be useful for some occasions.

![](https://reverent-carson-67c52e.netlify.app/static/img/images/0/Screenshot-2020-06-04-at-19.24.16.png)

You should use _git push --tags_ (or _git push tag_name_) to push tags to a remote repository.

5). **Git merge**. Fast-forwarding by default vs no fast-forward.

_git merge exercise3_:

![](https://reverent-carson-67c52e.netlify.app/static/img/images/0/Screenshot-2020-06-04-at-19.32.30.png)

I got the difference between _git merge some_branch_ and _git merge --no-ff some_branch_. It is becoming obvious when you use _git log --graph_.

_git merge --no-ff exercise3:_

![](https://reverent-carson-67c52e.netlify.app/static/img/images/0/Screenshot-2020-06-04-at-19.32.06.png)

6). **Git log - Grep, filter, since**

There are some more "advanced" git features, like grep, filter and since:

![](https://reverent-carson-67c52e.netlify.app/static/img/images/0/Screenshot-2020-06-04-at-19.37.49.png)

7). **Git log - no-pager and oneline**

![](https://reverent-carson-67c52e.netlify.app/static/img/images/0/Screenshot-2020-06-04-at-19.49.06.png)

8). **Git commit --amend**

Amend is a very useful commit "editing" tool. Actually, it's not exactly editing, but as we can see from the sha of commits - c8a341a vs dcbdc49, amend creates a new commit from the last one.

![](https://reverent-carson-67c52e.netlify.app/static/img/images/0/Screenshot-2020-06-05-at-19.06.03.png)

P.S.

Finally, I realized that git pull = git fetch + git merge. Amen.
