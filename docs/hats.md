---
layout: default
title: Hats
permalink: /hats
nav_order: 9
---

# Hats

Scratch is event-driven, with scripts under a hat block being executed when an event happens. For example, the most well-known hat is the "when flag clicked" block.

In Scrybe, hats are written such that the statements contained in them are generated under the hat in the Scratch project. For example:

```scrybe
scratch.on_flag() {
    <statements>
}
```

or:

```scrybe
scratch.on_flag() <single statement>
```

<hr>

## ![](/assets/event_whenflagclicked.png) - `scratch.on_flag()`

This hat is executed when the green flag is pressed.

## ![](/assets/event_whenkeypressed.png) - `scratch.on_keypress(<key name>)`

This hat is executed when a key is pressed. See [here](/built-ins/scratch#methods) for a list of valid key names.

## `scratch.on_keyrelease(<key name>)`

This hat is executed when a key is released. See [here](/built-ins/scratch#methods) for a list of valid key names.

## ![](/assets/event_whenthisspriteclicked.png) - `scratch.on_clicked()`

This hat is executed when the sprite it's used in is clicked.

## ![](/assets/event_whenbackdropswitchesto.png) - `scratch.on_backdrop(<backdrop name>)`

This hat is executed when the stage switches to a certain backdrop. Note that this block is not included in the standard Scratch block pallete, so it may be removed without warning.

## ![](/assets/event_whengreaterthan.png) - `scratch.on_greater_than(<value>, <threshold>)`

This hat is executed when a certain value (the timer or microphone volume) exceeds a set threshold.

Possible values for `value`:
 - `C.LOUDNESS`
 - `C.TIMER`

## ![](/assets/event_whenbroadcastreceived.png) - `scratch.on_broadcast(<broadcast name>, [message])`

This hat is executed when a broadcast is received by the target it's placed in, with an optional message.

## ![](/assets/control_start_as_clone.png) - `scratch.on_clone()`

This hat is executed as a clone when it is created.
