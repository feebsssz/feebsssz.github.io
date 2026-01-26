---
layout: page
title: Skills
---

{% for skill in site.data.skills %}
### {{ skill.category }}
{% if skill.items %}
<ul>
{% for item in skill.items %}
  <li>{{ item }}</li>
{% endfor %}
</ul>
{% endif %}
{% endfor %}
