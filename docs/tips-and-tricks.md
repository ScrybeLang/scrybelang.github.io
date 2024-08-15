---
layout: default
title: Tips & tricks
permalink: /tips-and-tricks
nav_order: 13
---

# Tips & Tricks

<hr>

## Graphic Tricks

 - Switching the costume to a number will set the costume by ID rather than by name
 - Switching the costume to the number 0 will set the costume to the last one. This can be used to find out how many costumes are in a sprite
 - You can do a grayscale effect on a sprite by setting its "color" effect to infinity (anything divided by 0):

```scrybe
function grayscale()
    set_effect(C.COLOR, 1 / 0);
```

## Math Tips

 - The result of a comparison can be used as a "switch" to "toggle" numbers in complex calculations
    - An example of this is shown in the expanded exponentiation implementation, where it is checked if the base is negative
