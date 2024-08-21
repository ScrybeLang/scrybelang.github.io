---
layout: default
title: Internal variable naming
parent: Variables
permalink: /variables/internal-naming
nav_order: 2
---

# Internal Variable Naming

Scrybe allows the user to define any variable anywhere, as you would in a normal programming language. In order to accomplish this, Scrybe has a set of rules that determine what the Scratch variable name should be based on the context where it is defined. This document exists as a disambiguation and a guide to anyone who may be interested in the inner workings of Scrybe variable scoping.

Each variable present in the compiled Scratch project has a prefix to distinguish itself, followed by the user-defined variable name.

<hr>

## Global Variables

Variables that are truly global are defined in `setup.sbc`. These variables have the prefix `g_` and are created in the stage so that they are global in the Scratch project ("for all sprites").

Variables that are defined in the top level of any script are global as well, but only to that script. These variables are defined in the target the script is for. If this target-wide variable is defined in a sprite, it will have the prefix `s_`. Otherwise, it will have the prefix `b_` (`b` standing for "backdrop"). This distinction is necessary so that target-wide variables defined in the stage don't overshadow ones defined in a sprite.

## Scoped Variables

Variables that are defined in a script but are not top-level are scoped. When Scrybe enters a new scope (usually defined by an opening brace), an internal "scope ID" will increment and be pushed to the "scope stack". During variable resolution, only global variables and variables in this stack are checked. Scoped variables have the prefix `s<scope ID>_` for sprites and `b<scope ID>_` for the stage.

## Broadcast Messages

Broadcast messages are global to the Scratch project (because broadcasts are global) and have the prefix `br_<broadcast name>`.

## Function Return Output

Each defined function gets a local variable that represents its output. Function return output variables have the prefix `fo_<function name>`. For functions defined in the stage, their return output variable is named `bfo_<function name>`.
