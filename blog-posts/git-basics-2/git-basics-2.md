---
published: false
title: "Git basics"
cover_image: "https://raw.githubusercontent.com/YOUR-USERNAME/YOUR-REPO/master/blog-posts/NAME-OF-YOUR-BLOG-POST/assets/your-asset.png"
description: ""
tags: git
series:
canonical_url:
---

## What is a git branch?

A branch in git is a line of development. You can have multiple branches in your project, and you can merge them together at some point. Have multiple branches can be useful when you have to work in a team, or also you can use branches to make different tasks (fixing a problem or adding a new feature for example). You can create a new branch using

```
git branch name-of-branch
```

The default branch name in git is master, but you can change the name using

```
git branch m new-name
```

You can use the next command to list all the available branches.

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

Using this you were mergin "my-branch" branch into the current branch.
If the two branches you try to merge both have change the same part of the code, Git won't be able to know which version to keep and he will stop the merge, asking you to resolve the conflict manually. You can also use a tool to do this.

## Git on remote

Git works really fine on local, but it also works on remote. It is really helpfull when we are working on a team, and more persons are working on the same project. There are some platforms like Github or Bitbucked in which you can store a remote repository.

## How can I save my changes in the remote repository?

You need to push them. Using the next command

```
git push origin master
```

Origin refers to the remote origin, and master refers to the branch which where I want to push changes.
You can also use git PULL TO get the changes from the remote repository to your working directory.

# You can get

You can copy an existing repository and cloning into your local machine, creating a folder with the project inside. For this, you can use

```
git clone https://www.github.com/username/repo-name
```

with the url of the repository that you want to clone into your computer.

# But there is more...

There is a lot of things to do... DESPEDIDA

# Found a typo?

If you've found a typo, a sentence that could be improved or anything else that should be updated on this blog post, you can access it through a git repository and make a pull request. Instead of posting a comment, please go directly to [my git repository](https://github.com/ThisIsItz/ThisIsDev) and open a new pull request with your changes.
