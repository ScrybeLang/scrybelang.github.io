---
layout: default
title: Return values
parent: Functions
permalink: /functions/return-values
nav_order: 2
---

# Function Return Values

Scrybe allows you to return any non-list variable from a function. Simply use the `return` keyword as you would in most other programming languages.

Here's an example of function return values in action:

```scrybe
warp function factorial(n) {
    result = 1;
    for (i = n; i > 0; i -= 1) {
        result *= i;
    }

    return result;
}

scratch.on_flag() {
    while(true) {
        scratch.ask("What would you like to calculate the factorial of?");
        answer = scratch.answer;

        say_for_seconds("The factorial of " .. answer .. " is " .. factorial(answer), 2);
    }
}
```

Alternatively, you can use `return` without any value to simply stop the script where it is:

```scrybe
warp function factorial(n) {
    if (n <= 0)
        return;

    ...
```

You may also use `return` inside of a hat to do the same thing.
