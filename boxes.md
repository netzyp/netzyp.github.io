---
layout: default
title: HTB Boxes
permalink: /boxes/
---

# Hack The Box - Machine Notes Index

All machine notes, automatically grouped by difficulty.

{% comment %} Get unique difficulties and sort them (e.g., EASY, MEDIUM, HARD) {% endcomment %}
{% assign difficulties = site.boxes | map: "difficulty" | uniq | sort %}

{% for difficulty in difficulties %}
## {{ difficulty | upcase }}
{% for box in site.boxes %}
{% if box.difficulty == difficulty %}
- [{{ box.title }}]({{ box.url | relative_url }}) (Completed: {{ box.date_completed }})
{% endif %}
{% endfor %}
{% endfor %}
