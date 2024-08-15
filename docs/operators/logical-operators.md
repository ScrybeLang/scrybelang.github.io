---
layout: default
title: Logical operators
parent: Operators
permalink: /operators/logical-operators
nav_order: 3
---

# Logical Operators

<hr>

Scrybe supports the logical operators `and`, `or`, `not`, and `in`. These work how you would expect, and have normal precendece. `in` works with both normal variables and lists.

```scrybe
say(not 5 < 3);      // true
say("e" in "world"); // false
say(1 and 2 and 3);  // true
```
