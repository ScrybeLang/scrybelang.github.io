---
layout: default
title: Functions
parent: Variables
permalink: /variables/functions
nav_order: 4
---

# Variable Functions

Similarly to other languages, you can call functions on variables and lists to alter their content or use attributes to get information about it. Normal variables and lists have different methods.

You can use the `.length` attribute on any variable or list. Note that this attribute treats numbers like strings.

## Lists

You may call the following functions on a list:

| Function name | Function parameters | Description                        |
| ------------- | ------------------- | ---------------------------------- |
| `push`        | `item`              | Adds `item` to the end of the list |
| `remove`      | `index`             | Removes the item at `index`        |
| `clear`       | None                | Removes all items from the list    |
| `insert`      | `index`, `item`     | Inserts `item` at `index`          |

Additionally, you can call `index` on a list to get the index of the first occurence of an item.
