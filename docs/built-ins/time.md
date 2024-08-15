---
layout: default
title: Time
parent: Built-ins
permalink: /built-ins/time
nav_order: 4
---

# `time`

<hr>

## Fields

Here are the fields provided by this builtin:

| Field name                                               | Field description            |
| -------------------------------------------------------- | ---------------------------- |
| `year`                                                   | Current year                 |
| `month`                                                  | Current month (1 - 12)       |
| `date`                                                   | Current date (1 - 31)        |
| `day_of_week`                                            | Current day of week (1 - 7)  |
| `hour`                                                   | Current hour (0 - 23)        |
| `minute`                                                 | Current minute               |
| `second`                                                 | Current second               |
| ![](/assets/sensing_timer.png) `timer`                   | Project timer                |
| ![](/assets/sensing_dayssince2000.png) `days_since_2000` | Days since 2000 (fractional) |

## Methods

Here are the methods provided by this builtin that should be used as a statement rather than in an expression:

| Method name                                       | Method parameters | Method description                           |
| ------------------------------------------------- | ----------------- | -------------------------------------------- |
| ![](/assets/control_wait.png) `sleep`             | `seconds`         | Pause the script for `seconds` seconds       |
| ![](/assets/sensing_resettimer.png) `reset_timer` | None              | Reset the project timer to 0                 |
| ![](/assets/control_wait_until.png) `wait_until`  | `condition`       | Pause the script until `condition` is truthy |
