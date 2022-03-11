---
title: Integration
permalink: /integration
excerpt: "How to add integrate 3rd party packages with Modula."

author_profile: false
author: Twist Apps

integr_mirror: common/integrations/mirror.md
---

Modula supports easy integration for any type that extends `MonoBehaviour`.

# Supported by Default
These are integrations with 3rd party packages that are supported out-of-the-box: 

{% if page.integr_mirror %}
  {% include_relative {{ page.integr_mirror }} %}
{% endif %}