---
layout: default
title: Return values
parent: Functions
permalink: /functions/return-values
nav_order: 2
---

# Function Return Values

Scrybe allows you to return any type from a function besides lists. To specify a return type, prepend any one of these types to the `function` keyword:
 * `num` - Return a number
 * `str` - Return a string
 * `bool` - Return a boolean
 * `var` - Return a general variable

A function declared without a return type will not work in an expression.

To actually return a value, simply use the `return` keyword as you would in most other programming languages. Here's an example of function return values in action:

```scrybe
warp num function factorial(n) {
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
warp num function factorial(n) {
    if (n <= 0)
        return;

    ...
```

You may also use `return` inside of a hat to do the same thing.

## Examples

Here are some other examples of function return types:

```scrybe
warp num function rshift(x, bits) // Returns a number
    return x / 2 ** bits;
```

```scrybe
warp bool is_on_top() // Returns a boolean
    return this.y >= 0;
```

```scrybe
warp str get_greeting(name) { // Returns a string
    if (time.hour < 12) return "Good morning, " .. name .. "!";
    if (time.hour < 5)  return "Good afternoon, " .. name .. "!";
    return "Good evening, " .. name .. "!";
}
```
