---
layout: default
title: Assets
parent: Declarations
permalink: /declarations/assets
nav_order: 1
---

# Assets

In Scratch, assets include costumes/backdrops and sounds. These specific kinds of declarations require one or more filepaths/glob expressions.

## Names

The valid asset declaration names are `costume` and `sound`. Do not add an -s at the end if you are providing a list to it.

## Format

The filepath(s) provided in an asset declaration are always relative to the project directory. For example, if you added a costume that pointed to `"assets/ball.png"`, Scrybe would try to find that file like so:

```
project directory/
|-- assets/
|   |-- ball.png
|
|   ...
```

If you are providing a list of filepaths and/or glob expressions, they must also be enclosed in brackets. Otherwise, leave it as a string.

Both sprites and the stage can use these declarations. Adding a "costume" to the stage is the same as adding a backdrop, however you must still use the `costume` declaration name.

## Examples

Here are some examples of valid asset declarations:

```scrybe
#costume "assets/ball.png"
```

```scrybe
#costume "images/*.jpg"
```

```scrybe
#costume ["assets/*.png", "assets/*.jpg", "assets/*.bmp"]
```

```scrybe
#sound "audio/background loop.mp3"
```

```scrybe
#sound ["assets/jump.wav", "assets/death.wav"]
```
