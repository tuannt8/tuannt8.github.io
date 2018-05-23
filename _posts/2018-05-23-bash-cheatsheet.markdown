---
layout: post
title:  "Bash cheat sheet"
date:   2018-05-22 13:32:31 +0200
categories: tips bash cheatsheet
---

Bash commonly used commands

```shell
for i in {1..100}; do echo $i; done
```

```shell
for i in *.png; do echo $i; done
```

```shell
filename=${fullname%.*}
```