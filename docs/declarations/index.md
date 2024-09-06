---
layout: default
title: Declarations
permalink: /declarations
has_children: true
nav_order: 6
---

# Declarations

Using declarations, you can change [initial properties](/declarations/properties) of targets, such as position and rotation. In addition, you can add [assets](/declarations/assets) to the target using filepaths or glob expressions.

<hr>

## Format

Declarations must always be at the top of any script, before any variables/hats/functions. They are formatted like so:

```scrybe
#<declaration type> <declaration value>
```

Declaration values must be literals, you cannot reference any global variables here. Note the lack of a semicolon at the end.
