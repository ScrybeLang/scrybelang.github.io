---
layout: default
title: If/else statements
parent: Control flow
permalink: /control-flow/if-else-statements
nav_order: 1
---

# If/Else Statements

![](/assets/control_if.png)

<hr>

If/else statements are made similarly to other languages. They consist of the keyword `if`, a condition enclosed in parentheses, and a body. There may optionally be an `else` body that is run if the condition is not met.

Here are some examples of if/else statements:

```scrybe
if (i % 3 == 0 and i % 5 == 0)
    say("Fizzbuzz");
else if (i % 3 == 0)
    say("Fizz");
else if (i % 5 == 0)
    say("Buzz");
else
    say(i);
```

```scrybe
if (distance_to_center > world_radius) {
    scale: num = world_radius / distance_to_center;
    this.x *= scale;
    this.y *= scale;
}
```
