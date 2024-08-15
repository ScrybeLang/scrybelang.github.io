---
layout: default
title: While loops
parent: Control flow
permalink: /control-flow/while-loops
nav_order: 3
---

# While Loops

![](/assets/control_repeat_until.png)

<hr>

While loops in Scrybe are also similar to those of other languages. They consist of the keyword `while`, a condition enclosed in parentheses, and a body. The statements in the body are not run if the condition is falsey upon the first iteration.

If the condition is simply `true`, Scrybe internally simplifies the while loop to a "forever" block in the Scratch palette.

Here are some examples of while loops:

```scrybe
while (true) {
    my_counter += 1;
    say(my_counter);
}
```

```scrybe
while (time.timer < 10) {
    say("It will be ten seconds in... " .. math.ceil(10 - time.timer) .. " seconds");
}
```
