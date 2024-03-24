---
label: Getting Started
icon: rocket
layout: default
order: 100
authors:
  - name: Lucas Guichard
    email: lucasguichard@konekan.fr
    link: https://konekan.fr
    avatar: ../static/images/avatar.jpg
image: ../static/images/ecs_featured.png
tags:
  - plugins
  - EntityCountingSystem
date: 2024-03-20
description: Learn how to enable and start using the plugin.
---

![](../static/images/ecs_featured.png)

# Entity Counting System

||| Details
Plugin version: v1.0.4<br>
Last documentation update: 01/21/2024<br>
|||

## Plugin activation

+++ Blueprint
To enable the plugin using Blueprint, follows the 4 steps and the restart your editor.

  ![](../static/images/ecs_plugin_activation.png)

+++ C++
To enable the plugin using C++, add the plugin module name in your public dependencies like following the code.

```cpp #4 PROJECT.Build.cs
public PluginSandboxProject(ReadOnlyTargetRules Target) : base(Target)
	{
		//...
		PublicDependencyModuleNames.AddRange(new string[] { ..., "EntityCountingSystem"});
		// ...
	}
```
+++