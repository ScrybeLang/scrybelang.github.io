---
layout: default
title: Setup
parent: Project structure
permalink: /project-structure/setup
nav_order: 1
---

# `setup.sbc`

This file contains the project declaration and all global variables. The setup file has a different format than that of script files, and thus works differently.

<hr>

## Project Declaration

The project declaration contains the formal name of the Scrybe project, and optionally a file name. It is formatted like so:

```scrybe
project <project name> [as <filename>];
```

Examples:

```scrybe
project "My Project" as "myproject.sb3";
```

```scrybe
project "Jetpack Game";
```

In the second example, the filename would be `Jetpack Game.sb3`. Any characters present in the project name are removed when using it as a filename if they are [invalid Windows directory name characters](https://stackoverflow.com/a/32565700).

<hr>

## Global Variables

By convention, global variables have all uppercase names, but this is not enforced by Scrybe. Global variables can be strings, numbers, lists, or even entire expressions. However, expressions must consist of literals. You cannot reference other variables when defining a global variable. Here are some examples of valid global variable declarations:

```scrybe
HUNDRED = 100;
TWO_THIRDS = 2/3;
MESSAGE = "Hello, World!";
FIBONACCI = [1, 1, 2, 3, 5, 8, 13, 21];
```

Hence their name, global variables are available (in scope) to each script inside of a project.
