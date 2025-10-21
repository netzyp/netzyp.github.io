---
layout: default
title: HTB Boxes
permalink: /boxes/
---

# Hack The Box - Machine Notes Index

Machines automatically grouped by difficulty.

{% assign difficulties = site.boxes | map: "difficulty" | uniq | sort %}

{% for difficulty in difficulties %}
## {{ difficulty | upcase }}
{% for box in site.boxes %}
{% if box.difficulty == difficulty %}
- [{{ box.title }}]({{ box.url | relative_url }}) 
{% endif %}
{% endfor %}
{% endfor %}
