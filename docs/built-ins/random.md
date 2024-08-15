---
layout: default
title: Random
parent: Built-ins
permalink: /built-ins/random
nav_order: 6
---

# `random`

<hr>

## Methods

Here are the methods provided by this builtin that should be used in an expression rather than as a statement:

| Method name                              | Method parameters | Method description                                  |
| ---------------------------------------- | ----------------- | --------------------------------------------------- |
| ![](/assets/operator_random.png) `range` | `min`, `max`      | Returns a random number in the range `min` to `max` |
| `choice`                                 | `item`            | Picks a random element from `item`                  |

If either `min` or `max` are a floating-point number, the result of `range(...)` will also be a floating-point number. Otherwise, the result will be an integer.

`item` may be a normal variable or a list.
