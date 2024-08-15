---
layout: default
title: Properties
parent: Declarations
permalink: /declarations/properties
nav_order: 2
---

# Sprite Properties

<hr>

Below are the rest of the valid declarations that set a sprite's initial properties. The stage may not use any of these properties.

| Name             | Type             | Description                                                       | Default value  |
| ---------------- | ---------------- | ----------------------------------------------------------------- | -------------- |
| `visible`        | Boolean          | If the sprite should be shown                                     | `true`         |
| `x`              | Number           | The initial X position                                            | `0`            |
| `y`              | Number           | The initial Y position                                            | `0`            |
| `size`           | Positive number  | The initial size, as a percentage                                 | `100`          |
| `direction`      | Number           | The initial direction, in degrees                                 | `90`           |
| `draggable`      | Boolean          | If the sprite should be able to be dragged with the mouse         | `true`         |
| `rotation_style` | String           | The initial rotation style                                        | `"all around"` |
| `layer`          | Positive integer | The initial layer number of the sprite. The stage is at layer `0` | `1`            |
