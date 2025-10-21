---
layout: default
title: HTB CPTs Path Modules
permalink: /cpts/
---

# CPTs Path Modules

All CPTs notes, automatically listed by module number.

{% comment %} Loop through all files in the cpts_modules collection {% endcomment %}
{% for module in site.cpts_modules %}
## [Module {{ module.module_num }}: {{ module.title }}]({{ module.url | relative_url }})
**Status:** {{ module.status | default: "In Progress" }}
---
{% endfor %}
