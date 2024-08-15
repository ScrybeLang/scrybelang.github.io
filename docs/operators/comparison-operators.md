---
layout: default
title: Comparison operators
parent: Operators
permalink: /operators/comparison-operators
nav_order: 2
---

# Comparison Operators

Scrybe supports comparing two numbers with the following operators:

| Operation                                 | Symbol |
| ----------------------------------------- | ------ |
| ![](/assets/operator_lt.png) Less than    | `<`    |
| ![](/assets/operator_gt.png) Greater than | `>`    |
| Less than or equal to                     | `<=`   |
| Greater than or equal to                  | `>=`   |
| ![](/assets/operator_equals.png) Equal to | `==`   |

Using the results of these comparisons with numerical operators will use either the number `0` or `1`, depending on its truthiness. For example:

```scrybe
my_variable = (2 < 3) * 5; // Will be 5
my_variable = (4 < 3) * 5; // Will be 0
```
