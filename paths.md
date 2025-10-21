---
layout: default
title: HTB Academy Paths
permalink: /paths/
---

# HTB Academy Paths Index

All learning path notes, organized here.

{% for item in site.paths %}
## [{{ item.title }}]({{ item.url | relative_url }})
**Status:** {{ item.status | default: "Not Started" }}
---
{% endfor %}
