---
layout: default
title: Functions
parent: Variables
permalink: /variables/functions
nav_order: 5
---

# Variable Functions

Similarly to other languages, you can call functions on variables to alter their content or use attributes to get information about it.

<hr>

## Numbers

Numbers have no fields, methods, or functions.

## Strings

Strings have one field, `length`, that contains the amount of characters it holds.

## Booleans

Booleans have no fields, methods or functions.

## General variables

General variables also have one field, `length`, that works the same way strings do.

## Lists

Lists have one field, `length`, that contains the amount of elements it holds. Lists also have one method, `index`, that gets the index of the first occurence of an item.

Lists have the following functions:

| Function name | Function parameters | Description                        |
| ------------- | ------------------- | ---------------------------------- |
| `push`        | `item`              | Adds `item` to the end of the list |
| `insert`      | `index`, `item`     | Inserts `item` at `index`          |
| `remove`      | `index`             | Removes the item at `index`        |
| `clear`       | None                | Removes all items from the list    |

# Conversion

Conversion between variables can be done with the following built-in functions:
 * `tonum(...)` - Convert argument to a number
 * `tostr(...)` - Convert argument to a string
