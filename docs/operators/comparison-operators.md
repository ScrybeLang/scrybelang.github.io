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

Each of these operators returns a boolean value, which can be casted to a number (`0` for `false` or `1` for `true`) if necessary. This allows you to do something like the following:

```scrybe
my_variable = (2 < 3) * 5; // Will be 5
my_variable = (4 < 3) * 5; // Will be 0
```

For equality only, two strings can be compared like `string_1 == string_2`. String comparisons are case-insensitive due to Scratch limitations.
