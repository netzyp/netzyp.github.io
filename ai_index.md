---
layout: default
title: HTB AI Red Teamer Modules
permalink: /ai/
---

# AI Red Teamer Modules Index

{% for module in site.ai_modules %}
## [{{ module.title }}]({{ module.url | relative_url }})
**Module Focus:** {{ module.focus }}
---
{% endfor %}
