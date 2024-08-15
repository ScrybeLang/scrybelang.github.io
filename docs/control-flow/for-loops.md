---
layout: default
title: For loops
parent: Control flow
permalink: /control-flow/for-loops
nav_order: 2
---

# For Loops

![](/assets/control_repeat_until.png)

<hr>

Like if/else statements, for loops in Scrybe are formatted similarly to those found in other programming languages. They consist of the keyword `for`, then an initialization statement, a condition, then finally a post-iteration statement.

In most `for` loops, the post-iteration statement will increment the variable initialized in the initialization statement, usually by one. However, Scrybe does not support increment or decrement operators, so the user must do something like `i += 1` or `i -= 1`. Internally, Scrybe translates `for` loops into a "repeat until" block in the Scratch palette so that it can support a more diverse array of post-iteration statements.

Here are some examples of for loops:

```scrybe
for (i = 0; i < 10; i += 1) {
    say("I can count to " .. i + 1 .. "!");
    time.sleep(1);
}
```

```scrybe
for (y = 0; y < 100; y += 10) {
    for (x = 0; x < 100; x += 10) {
        set_pos(x - 50, y - 50);
        say("Position: (x=" .. x .. ", y=" .. y .. ")");
        time.sleep(0.1);
    }
}
```
