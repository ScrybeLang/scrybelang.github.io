---
layout: default
title: Usage
nav_order: 3
permalink: /usage
---

# Usage
<hr>

To compile a project, simply type:

```shell
scrybe <args>
```

into a terminal. Your `PATH` must be set up correctly with the Python environment for this to work properly. If this doesn't work, try:

```shell
python -m scrybe <args>
```

Arguments may be enclosed in double quotes.

## Arguments

### Project

The first argument must be a path to the project directory you wish to compile.

### Output Filename

Include a valid filename ending in `.sb3` to override the file name of the outputted Scratch project. By default, this is the name of the directory or the project name as configured in `setup.sbc`.

### Log Level (`-log`)

Scrybe outputs logs when compiling a project. The valid log levels are:

* 1: `debug`
* 2: `info`
* 3: `warning`
* 4: `error`

Enter any of these to see that log level and any logs with a higher log level. The default log level is `info`.

### Color (`-color`)

By default, log output is colorized. To change this behavior, use with an argument of `on` or `off`.

<hr>

## Examples

```shell
scrybe ./project
```

```shell
scrybe ./project -log debug
```

```shell
scrybe "C:/Users/.../Desktop/My Project" -color off "my file name.sb3"
```
