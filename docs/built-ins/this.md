---
layout: default
title: This
parent: Built-ins
permalink: /built-ins/this
nav_order: 3
---

# `this`

<hr>

## Fields

Here are the fields provided by this builtin:

| Field name                                    | Field description    |
| --------------------------------------------- | -------------------- |
| ![](/assets/motion_xposition.png) `x`         | X position           |
| ![](/assets/motion_yposition.png) `y`         | Y position           |
| ![](/assets/motion_direction.png) `direction` | Direction in degrees |
| ![](/assets/looks_size.png) `size`            | Size as a percentage |
| `costume.name`                                | Costume name         |
| `costume.number`                              | Costume number       |
| ![](/assets/sound_volume.png) `volume`        | Played sound volume  |

Each of these fields besides `costume.name` and `costume.number` can be assigned to arbitrarily to alter that field. For example:

```scrybe
this.x += 10;            // Move 10 pixels to the right
this.direction -= 90;    // Rotate 90 degrees counterclockwise
this.size *= 2;          // Double size
this.volume = this.size; // Not sure why you would want to do this but it's possible
```

## Methods

Here are the methods provided by this builtin that should be used in an expression rather than as a statement:

| Method name                                                          | Method parameters    | Method description                                                           |
| -------------------------------------------------------------------- | -------------------- | ---------------------------------------------------------------------------- |
| ![](/assets/sensing_touchingobject.png) `touching`                   | `target`             | If the sprite is visually touching `target`                                  |
| ![](/assets/sensing_touchingcolor.png) `touching_color`              | `color`              | If the sprite is visually touching the color `color`                         |
| ![](/assets/sensing_coloristouchingcolor.png) `color_touching_color` | `color_1`, `color_2` | If the color `color_1` on the sprite is touching `color_2` on another sprite |
| ![](/assets/sensing_distanceto.png) `distance_to`                    | `target`             | The distance (in pixels) to `target` (both centers)                          |

Possible values for `target`:
 - `C.MOUSE`
 - `C.EDGE`
 - Any sprite name

Color values must be in 6-digit hexadecimal form with a leading octothorpe.

This builtin provides no methods meant to be used as statements.
