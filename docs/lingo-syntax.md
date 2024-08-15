---
layout: default
title: Lingo/syntax
permalink: /lingo-syntax
nav_order: 4
---

# Lingo

Here are some terms used throughout this documentation and their meanings. This list is meant to help you better understand what is said:
 - "Statement" - Something that happens by itself within the code. These are separated by semicolons
 - "Expression" - Something that represents a value rather than a command. These are used within statements to input data to them
 - "Attribute" - Something that is a part of another object. These are accessed through the dot (`.`) operator
 - "Field" - A type of attribute that represents a value or piece of data
 - "Method" - A type of attribute that manipulates something in some way when invoked
 - "Symbol" - The name representing a variable or a list
 - "Normal variable" - Scratch has two types of variables, normal variables and lists; this is the former

<hr>

# Syntax

Scrybe syntax is similar to that of languages like JavaScript.

Statements (but not property declarations) are separated by a semicolon, and thus whitespace does not matter unless it is in a string. So, minified Scrybe code is possible.

All indexes are zero-based, unlike Scratch, which has one-based indexing. This rule applies everywhere except costume/backdrop numbers.

When writing the body of a container, it may either be a set of statements enclosed in braces, or a single statement. This behavior is inspired from braced programming languages, and allows you to do things like:

```scrybe
if (i % 3 == 0 and i % 5 == 0)
    say("Fizzbuzz");           // This statement belongs to the first "if" body
else if (i % 3 == 0)           // This "else" statement also belongs to the first "if" body
    say("Fizz");
else if (i % 5 == 0)           // This "else" statement belongs to the second "if" body
    say("Buzz");
else
    say(i);
```

Internally, Scrybe does not differ between strings and numbers, because usually neither does Scratch. However, if a user attempts to perform numerical operations on a string, they will be met with the number 0.

Expressions may be enclosed in parentheses to alter precedence.

## Error Messages

Scrybe error messages are meant to be easy to debug. They contain the location of the faulty code, a descriptive error message, and the last few lines of code leading up to the line the error is on. All in all, having problems with your code is no pleasant experience, but with Scrybe, at least they look pretty.
