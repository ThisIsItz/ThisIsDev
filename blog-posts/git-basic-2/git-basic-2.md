---
published: false
title: "Git basics ++"
cover_image: "https://raw.githubusercontent.com/ThisIsItz/ThisIsDev/master/blog-posts/git-basic-2/assets/git.png"
description: ""
tags: git, beginner, tutorial
series:
canonical_url:
---

In my [previous post](https://dev.to/thisisitz/git-basics-5808) I talked about git basics, but there was more to say about. In this post I continue explaining how git works and how to use it.


## What is a git branch?

A branch in git is a line of development. You can have multiple branches in your project, and you can merge them together at some point. Have multiple branches can be useful when you have to work in a team, or also you can use branches to make different tasks (fixing a problem or adding a new feature for example). You can create a new branch using

```
git branch name-of-branch
```

The default branch name in git is master, but you can change the name using

```
git branch -m new-name
```

You can use the next command to list all the available branches, and also to known in which branch you are working on

```
git branch
```

And also you can switch between branches using

```
git checkout another-branch
```

## So... how can I merge branches?

Git merge allows us to merge, or integrate, different branches into a single branch.
The most common situation is when you merge only two branches. You can use

```
git merge my-branch
```

Using this you were merging "my-branch" branch into the current branch.
If the two branches you try to merge both have change the same part of the code, Git won't be able to know which version to keep and he will stop the merge, asking you to resolve the conflict manually. You can also use a tool to do this.


## Git on remote

Git works really fine on local, but it also works on remote. Remote state is another repository, is a version of your project that is hosted on the internet. It is really helpful when we are working on a team, and more persons are working on the same project. There are some repository hosting services like [Github](https://github.com) or [Bitbucked](https://bitbucket.org/) in which you can store a remote repository, so you can manage your remote repository easily.


## Saving your projects in remote

To add your project, you have to create the remote repository in one of the platforms mentioned (github, bitbucked...) to get an URL. Once you have this, you need to go to the terminal, make sure you are in your project and use the following command

```
git remote add origin https://github.com/user/repo.git 
```

This URL is an example URL where 'User' is your username in git, and 'repo' is the name of your remote repository. If you want to know which remote URL should you use check this [link](https://help.github.com/en/github/using-git/which-remote-url-should-i-use).

You can also check in which remote your project is using the next command

```
git remote -v
```

This command will return the name of the remote URL where your project is.



## How can I save my changes in the remote repository?

You need to push them. Using the next command

```
git push origin master
```

Origin refers to the remote origin, and master refers to the branch where I want to push changes.
You can also use git pull to get the changes from the remote repository to your working directory.

```
git pull origin master
```

It's recommended that you use git pull before git push to avoid conflicts.


## Can I use remote repositories from anyone else?

Sure! You can get a project from an existing repository and cloning into your local computer, creating a folder with the project inside so you can work on that project on yourself. For this, you can use

```
git clone https://www.github.com/username/repo-name
```

with the URL of the repository that you want to clone into your computer.

## But there is more...

There's a lot of things to learn about git yet. In this post and the previous one, I've showed you only the basics. If you want to know more you can check the official [documentation](https://git-scm.com/doc). Thanks for reading!

## Found a typo?

If you've found a typo, a sentence that could be improved or anything else that should be updated on this blog post, you can access it through a git repository and make a pull request. Instead of posting a comment, please go directly to [my git repository](https://github.com/ThisIsItz/ThisIsDev) and open a new pull request with your changes.
