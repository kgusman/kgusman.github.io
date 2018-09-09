---
layout: post
title: "Yandex Interview"
description: "First interview for Python back-end developer"
date: 2018-09-10
tags: programming python interview yandex
---

# Yandex interview
It was my first interview for Python back-end developer in Yandex. Below you can see the theoretical questions and tasks that were provided to me.

## Questions
- Generators in Python.
- Context managers in Python.
- What does “yield” do in Python?
- Describe the process of the user request in networks (OSI model).

## Task 1
You have a single linked list:

```
head
 |
 A -> B -> C
```
The task is to reverse this list in O(1):
```
          head
           |
 A <- B <- C
```

## Task 2
Assume that there exists a program that returns a set of  **tags** that are represented in integer values:
```
[15, 4, 6, 8, 10, 23, 5, 9, 7]
```

Your task is to convert this set into human-readable format:
```
4 - 10, 15, 23
```

Additionally, provide tests that you can use for checking that your program works well and fail where it has to fail.