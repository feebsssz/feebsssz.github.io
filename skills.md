---
layout: page
title: Skills
permalink: /skills/
---

{% for skill in site.data.skills %}
### {{ skill.category }}

{{ skill.description }}

{% endfor %}
