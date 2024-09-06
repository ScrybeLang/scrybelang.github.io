---
layout: default
title: Formats
parent: Variables
permalink: /variables/formats
nav_order: 4
---

# Variable Formats

<hr>

## Numbers

Numbers may be either integers or decimals. Decimals may optionally have a digit before the period. With integers, you have several formats available:
 * Binary (base 2): `0b101`, `0b110001011`, `0b101010101`
 * Octal (base 8): `0o174`, `0o2251`, `0o736`
 * Base 10: `15`, `640`, `1078`
 * Hexadecimal (base 16): `0xDEADBEEF`, `0x1f2f3f`

Note that all integers are case-insensitive (when using alternate number systems).

## Strings

Strings are enclosed in double or single quotes and can be escaped with a backslash (`\`). They cannot be split across multiple lines, however most escape codes (`\n`, `\t`) work as expected.

## Booleans

Booleans take the form of the keyword `true` or `false`. When using an integer in place of a boolean (for example, in a loop condition), zero is the only falsy value.

## Lists

Lists are enclosed by brackets (`[`, `]`) and cannot be nested or added with the `+` operator. They may be split across multiple lines.
