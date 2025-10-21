---
layout: default
title: HTB Academy Paths
permalink: /paths/
---

# HTB Academy Index

All learning paths notes, automatically listed below:

{% for item in site.paths %}
## [{{ item.title }}]({{ item.url | relative_url }})
**Level:** {{ item.level | default: "N/A" }} | **Status:** {{ item.status | default: "Not Started" }}
{{ item.excerpt }} 
---
{% endfor %}
