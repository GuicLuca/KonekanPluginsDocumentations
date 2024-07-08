---
label: Changelog
icon: book
layout: default
order: 0
authors:
  - name: Lucas Guichard
    email: lucasguichard@konekan.fr
    link: https://konekan.fr
    avatar: ../static/images/avatar.jpg
tags:
  - plugins
  - BlueprintUtilities
date: 2024-05-13
description: All last updates for each version of the plugin
---

## V2.0

===- V2.0.0

[!badge variant="secondary" text="Blueprint node: 51"] &nbsp;&nbsp;&nbsp;&nbsp; [!badge variant="warning" text="Supported platforms: Lunux, Windows, Android"]

General
:   - Two new modules (! runtime and 1 UncookedOnly) to support the Maths library.

Math library
:   - 11 new nodes to improve the math experience with Blueprint.
    `Min`, `Max`, `Invert`, `Oposit`, `Spaceship operator (<=>)`, `+=`, `-=`, `*=`, `/=`, `Greater or Nearly Equal` and `Less or Nearly Equal`

===- V2.0.0

[!badge variant="secondary" text="Blueprint node: 40"] &nbsp;&nbsp;&nbsp;&nbsp; [!badge variant="warning" text="Supported platforms: Lunux, Windows, Android"]

General
:   - The plugin code has been spited in submodule to allow editor and runtime features to be compiled independently.  
    - Huge code refractoring reducing the duplicated code.
    - Performance updates and general code cleanup.

Get As System
:   - All 37 Getters refarctored to use Kismet.
    - Dynamic cast refarctored to use Kismet.
    - All nodes of the module can be converted to pure/impure mode with a click in the context menu.
    - Nodes with a target object can be converted to hard/soft pointer input type with a click in the context menu.

Log System
:   - New project settings (`Display profile's name in node title`, `Should error if no profile selected`, `Log node color`, `Disabled node color`).
    - The Log node refarctored to use kismet.
    - The Log node now implement a format system like the FormatText node.
    - The Log node now change of style and title according to the selected log profile.

=== 

## V1.0

===- V1.0.5

[!badge variant="secondary" text="Blueprint node: 115"] &nbsp;&nbsp;&nbsp;&nbsp; [!badge variant="warning" text="Supported platforms: Lunux, Windows, Android"]

General
:   - The plugin code has been setup in modules to improve code maintanability.  
    - New platforms supported : Linux and Android.

Get As System
:   - 37 Getters implemented with 3 forms: Pure, Impure, SoftRef based
    - Dynamic cast node with 2 forms: Pure, Impure

Log System
:   The log system is user created log profiles based and support all build environement type (Editor, Development (and debug), Shipping)

Workflow library
:   The first node of the library added is TimedDoOnce.

===
