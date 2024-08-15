---
layout: default
title: Types
parent: Variables
permalink: /variables/types
nav_order: 3
---

# Variable Types

Variables defined in Scrybe are either normal variables or lists. Normal variables can either be strings, numbers, or a Boolean. Strings are enclosed in double or single quotes and can be escaped with a backslash (`\`). Internally, all types of normal variables are the same.

<hr>

## Scopes

Similarly to variables defined in `setup.sbc`, the values of variables defined at the top-level of a script must consist solely of literals and cannot use any symbols.

## Examples

You can define a normal variable like so:

```scrybe
my_string = "Hello, World!";
my_number = 15;
my_decimal = 3.14;
my_quote = "Benjamin Franklin once said, \"Ouch.\"";
```

Lists are defined using brackets, like so:

```scrybe
fibonacci = [1, 1, 2, 3, 5, 8, 13, 21];
messages = ["Hello!", "Goodbye!", "See you later!"];
```
