---
layout: default
title: Main functions
nav_order: 11
permalink: /main-functions
---

# Main Functions

Scrybe translates most of the blocks in the Scratch pallete to global functions. These are available anywhere without having to access any attributes.

## Motion

| Function name                                                 | Function parameters | Function description                         |
| ------------------------------------------------------------- | ------------------- | -------------------------------------------- |
| ![](/assets/motion_movesteps.png) `move_steps`                | `steps`             | Move `steps` pixels in the current direction |
| ![](/assets/motion_goto.png) `go_to`                          | `target`            | Go to a target                               |
| ![](/assets/motion_gotoxy.png) `set_pos`                      | `x`, `y`            | Set position to (`x`, `y`)                   |
| ![](/assets/motion_glideto.png) `glide_to`                    | `target`, `seconds` | Glide to `target` for `seconds` seconds      |
| ![](/assets/motion_glidesecstoxy.png) `glide_to_pos`          | `x`, `y`, `seconds` | Glide to (`x`, `y`) for `seconds` seconds    |
| ![](/assets/motion_pointtowards.png) `point_towards`          | `target`            | Set direction towards `target`               |
| ![](/assets/motion_ifonedgebounce.png) `bounce_off_edge`      | None                | Reflect direction according to touched edge  |
| ![](/assets/motion_setrotationstyle.png) `set_rotation_style` | `style`             | Set allowed methods of rotation              |

Possible values for `target`:
 - `C.RANDOM`
 - `C.MOUSE`
 - Any sprite name

Possible values for `style`:
 - `C.LEFT_RIGHT`
 - `C.DONT_ROTATE`
 - `C.ALL_AROUND`

## Looks

| Function name                                                      | Function parameters  | Function description                  |
| ------------------------------------------------------------------ | -------------------- | ------------------------------------- |
| ![](/assets/looks_sayforsecs.png) `say_for_seconds`                | `message`, `seconds` | Say `message` for `seconds` seconds   |
| ![](/assets/looks_say.png) `say`                                   | `message`            | Say `message`                         |
| ![](/assets/looks_thinkforsecs.png) `think_for_seconds`            | `message`, `seconds` | Think `message` for `seconds` seconds |
| ![](/assets/looks_think.png) `think`                               | `message`            | Think `message`                       |
| ![](/assets/looks_switchcostumeto.png) `set_costume`               | `costume`            | Switch costume to `costume`           |
| ![](/assets/looks_nextcostume.png) `next_costume`                  | None                 | Switch to the next costume            |
| ![](/assets/looks_switchbackdropto.png) `switch_backdrop`          | `backdrop`           | Switch backdrop to `backdrop`         |
| ![](/assets/looks_nextbackdrop.png) `next_backdrop`                | None                 | Switch to the next backdrop           |
| ![](/assets/looks_cleargraphiceffects.png) `clear_graphic_effects` | None                 | Clear all graphical effects           |
| ![](/assets/looks_show.png) `show`                                 | None                 | Show the sprite                       |
| ![](/assets/looks_hide.png) `hide`                                 | None                 | Hide the sprite                       |
| ![](/assets/looks_gotofrontback.png) `set_layer`                   | `layer`              | Send sprite to a certain layer        |
| ![](/assets/looks_goforwardbackwardlayers.png) `change_layer`      | `change`             | Change current layer by `change`      |

Possible values for `layer`:
 - `C.FRONT`
 - `C.BACK`

## Sound

| Function name                                             | Function parameters | Function description                    |
| --------------------------------------------------------- | ------------------- | --------------------------------------- |
| ![](/assets/sound_playuntildone.png) `play_until_done`    | `sound`             | Play `sound` and wait until it finishes |
| ![](/assets/sound_play.png) `play_sound`                  | `sound`             | Start playing `sound`                   |
| ![](/assets/sound_stopallsounds.png) `stop_all_sounds`    | None                | Stop all playing sounds in all targets  |
| ![](/assets/sound_cleareffects.png) `clear_sound_effects` | None                | Clear all auditory effects              |

## Sensing

| Function name                                        | Function parameters | Function description                               |
| ---------------------------------------------------- | ------------------- | -------------------------------------------------- |
| ![](/assets/sensing_setdragmode.png) `set_drag_mode` | `mode`              | Change if sprite is able to be dragged by the user |

Possible values for `mode`:
 - `C.DRAGGABLE`
 - `C.NOT_DRAGGABLE`

## Other

| Function name   | Function parameters | Function description                           |
| --------------- | ------------------- | ---------------------------------------------- |
| `change_effect` | `effect`, `change`  | Change graphical/auditory `effect` by `change` |
| `set_effect`    | `effect`, `value`   | Set graphical/auditory `effect` to `value`     |

Possible values for `effect`:
 - Graphic effects:
    - `C.COLOR`
    - `C.FISHEYE`
    - `C.WHIRL`
    - `C.PIXELATE`
    - `C.MOSAIC`
    - `C.BRIGHTNESS`
    - `C.GHOST`
 - Sound effects:
    - `C.PITCH`
    - `C.PAN`
