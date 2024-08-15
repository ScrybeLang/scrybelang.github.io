---
layout: default
title: Declaration
parent: Functions
permalink: /functions/declaration
nav_order: 1
---

# Function Declaration

To declare a normal function, simply type:

```scrybe
function function_name(function_arguments, ...) {
    <function body>
}
```

Functions support an arbitrary amount of arguments, which will be in-scope for the function body. Internally, each parameter is of the type "number or text", which simplifies things and allows booleans to be expressed as binary bits (`0` or `1`).

To make a function run without refreshing the screen, simply add the `warp` keyword to the beginning:

```scrybe
warp function function_name(...
```
