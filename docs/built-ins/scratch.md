---
layout: default
title: Scratch
parent: Built-ins
permalink: /built-ins/scratch
nav_order: 1
---

# `scratch`

<hr>

## Fields

Here are the fields provided by this builtin:

| Field name                                      | Field description                                            |
| ----------------------------------------------- | ------------------------------------------------------------ |
| `backdrop.name`                                 | The name of the current backdrop                             |
| `backdrop.number`                               | The costume number of the current backdrop                   |
| ![](/assets/sensing_answer.png) `answer`        | The answer given by the user to a `scratch.ask(...)` query   |
| ![](/assets/sensing_mousedown.png) `mouse_down` | If the left mouse button is clicked or the screen is touched |
| ![](/assets/sensing_mousex.png) `mouse_x`       | The current X position of the mouse or finger on the screen  |
| ![](/assets/sensing_mousey.png) `mouse_y`       | The current Y position of the mouse or finger on the screen  |
| ![](/assets/sensing_loudness.png) `loudness`    | The current input volume of the microphone as a percentage   |
| ![](/assets/sensing_username.png) `username`    | The detected username of the user running the project        |

## Methods

Here are the methods provided by this builtin that should be used in an expression rather than as a statement:

| Method name                                       | Method parameters     | Method description                                |
| ------------------------------------------------- | --------------------- | ------------------------------------------------- |
| ![](/assets/sensing_keypressed.png) `key_pressed` | `key`                 | Returns whether or not `key` is currently pressed |
| ![](/assets/sensing_of.png) `get_attribute`       | `attribute`, `target` | Returns the `attribute` attribute of `target`     |

Possible values for `key`:
 - Any character in the range U+0021 to U+007E
 - `C.SPACE`
 - `C.ENTER`
 - `C.UP_ARROW`
 - `C.DOWN_ARROW`
 - `C.LEFT_ARROW`
 - `C.RIGHT_ARROW`

Possible values for `attribute`:
 - `C.VOLUME`
 - If `target` is the stage:
    - `C.BACKDROP_NAME`
    - `C.BACKDROP_NUMBER`
 - Otherwise:
    - `C.X_POSITION`
    - `C.Y_POSITION`
    - `C.DIRECTION`
    - `C.COSTUME_NUMBER`
    - `C.COSTUME_NAME`
    - `C.SIZE`

Possible values for `target`:
 - `C.STAGE`
 - Any sprite name

Here are the methods provided by this builtin that should be used as a statement rather than in an expression:

| Method name                                                  | Method parameters        | Method description                                                                                             |
| ------------------------------------------------------------ | ------------------------ | -------------------------------------------------------------------------------------------------------------- |
| ![](/assets/control_stop.png) `stop`                         | `mode`                   | Stops a certain aspect of the project according to `mode`                                                      |
| ![](/assets/sensing_askandwait.png) `ask`                    | `query`                  | Asks `query` with a message box and waits for the user's response, stored in `scratch.answer`                  |
| ![](/assets/event_broadcast.png) `broadcast`                 | `broadcast`, [`message`] | Broadcasts `broadcast` to the project with an optional `message`                                               |
| ![](/assets/event_broadcastandwait.png) `broadcast_and_wait` | `broadcast`, [`message`] | Broadcasts `broadcast` to the project with an optional `message` and waits for all listeners to finish running |
| ![](/assets/control_create_clone_of.png) `clone`             | [`target`]               | Creates a clone of the current sprite or another one                                                           |
| ![](/assets/control_delete_this_clone.png) `delete_clone`    | None                     | Deletes the clone this method is ran on                                                                        |

Possible values for `mode`:
 - `C.ALL`
 - `C.OTHER_SCRIPTS`
 - `C.THIS_SCRIPT`

Possible values for `message`:
 - Anything except a list

Possible values for `target`:
 - `C.MYSELF` (default for when called without any arguments)
 - Any sprite name
