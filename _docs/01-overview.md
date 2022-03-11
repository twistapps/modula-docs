---

title: What is Modula?
permalink: /
excerpt: "Modula package brings the concept of Modular Entities into Unity Engine."

author_profile: true
author: Twist Apps

install_instructions: common/installation/recommended.md

---

Modula is a package for [Unity Engine](https://unity.com) that helps 
splitting your code into smaller independent parts.
[Get Started](#installation){: .btn .btn--primary .btn--primary .btn--info}

---
![logo](https://user-images.githubusercontent.com/26601205/157171576-6774cfdf-e63d-484e-a954-60717e3eb3ad.png)

---

When needed, inherit from `ModularBehaviour` instead of Unity's default `MonoBehaviour` class.
This lets you **split** all the logic inside of your component and **move** it 
into independent modules, 
which could later be connected to/removed from each instance of that component, 
using the inspector GUI:

![modula2](https://user-images.githubusercontent.com/26601205/157162945-b4b174e2-c7ce-4d8c-af3d-d07a0f27f20b.gif)

That way by distributing the code into small self-containing modules you could make the codebase cleaner and easier to understand.

## Brief Overview

The final gameobject designed using Modula should consist of these components:

- **[Main](/module-features#main-)** behaviour script

    
    {% highlight C# %}// Main Behaviour
    public class Car : ModularBehaviour
    {
         // Your code as you do it usually
         ...
    }{% endhighlight %}

- Some connected modules


    {% highlight C# %}// Example Module
    public class Engine : Module 
     {
         void Start() { ... }
         
         ...
     }{% endhighlight %}

- Other unity Components you need for this system

## Installation
{% if page.install_instructions %}
  {% include_relative {{ page.install_instructions }} %}
{% endif %}

There are other installation methods listed at [**"Installation"** page](/install#2-download-from-asset-store).
{: .notice}

### Updating
Check out the [full page](/install#updating) to read the update instructions.

---
# Next Steps
Code your first module by following **[Quick Start](/quick-start) instructions**.