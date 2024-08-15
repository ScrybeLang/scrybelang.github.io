---
layout: default
title: Project structure
permalink: /project-structure
has_children: true
nav_order: 5
---

# Project Structure
<hr>

A Scrybe project is contained in a directory. Each file inside of it is optional. If no files are provided inside of the directory, or none can be found that are valid, the output will be an empty Scratch project.

### File Formats

The setup file has the file extension `.sbc`, while all script files have the extension `.sbs`. `sbc` stands for "ScryBe Config", and `sbs` stands for "ScryBe Script".

<hr>

## Files

### `setup.sbc`

This file contains the project declaration and all global variables. See [the setup documentation](./setup) for more information.

### `stage.sbs`

This file contains the scripts for the stage.

### Sprites

There may be a `sprites` folder present in the project directory. Each `.sbs` file in this folder will be added as a sprite.
