---
layout: default
title: Types
parent: Variables
permalink: /variables/types
nav_order: 3
---

# Variable Types

Variables defined in Scrybe can be one of the following types:
 * Number (`<variable name>: num = ...`)
 * String (`<variable name>: str = ...`)
 * Boolean (`<variable name>: bool = ...`)
 * General variable (`<variable name>: var = ...`)
 * List (`<variable name>[] = ...`)

Strings are enclosed in double or single quotes and can be escaped with a backslash (`\`).

If a variable is defined without a type, it will be a general variable. General variables act as a number, string, and a Boolean simultaneously, and can be used to avoid type restrictions. Each item in a list is automatically a general variable.

<hr>

## Scopes

The values of variables defined at the top-level of a script must consist solely of literals and cannot reference any variable names.

## Examples

Here is how you define variables:

```scrybe
my_string: str  = "Hello, World!";
my_number: num  = 15;
my_decimal:     = 3.14;
my_bool: bool   = 2 < 5;
my_quote        = "Benjamin Franklin once said, \"Ouch.\"";
```

and lists:

```scrybe
fibonacci[] = [1, 1, 2, 3, 5, 8, 13, 21];
messages[] = ["Hello!", "Goodbye!", "See you later!"];
```
