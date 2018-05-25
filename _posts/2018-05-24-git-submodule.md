---
title: Use Git submodule to inlcude external library from other repository
date: 2018-05-24 23:00:00 Z
categories:
- tips
- git
layout: post
---

## Test case
Imagine you have a repository name `main_repository`. You want to use a library from other repository name `sub_repository`. You want it inside your repository, so other people can easily clone and build your code.

## Add sub repository to your main repository
```shell
git clone https://github.com/main_repository
cd main_repository
git submodule add https://github.com/sub_repository
```

**What happen:** You will have a folder with sub repository. Your main repository will communicate with the sub repository with a file name `.gitmodules`.

## Work with sub repository
It is an independent repository. Work with it as normal, for example

```shell
cd sub_repository
git status
git commit -m "Update to sub repository"
git push
```

or `pul`, `diff`, etc. Whatever you want to.

## Commit changes in sub repository to main repository
Just make a normal commit

```shell
cd main_repository
git status
git commit -m "Update to main repository, inlcuding file from sub repository"
git push
```

If you use Githiub, in the code tabe you will see something like: `sub_repository @ 008d638d`

## Other people want to clone
Either

```shell
git clone main_repository
git submodule init
git submodule update
```

or

```shell
git clone --recurse-submodules https://github.com/main_repository
```

