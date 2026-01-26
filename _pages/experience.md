---
layout: page
title: Experience
permalink: /experience/
---

{% for role in site.data.experience %}
### {{ role.role }} — {{ role.organization }}
{{ role.start }} – {{ role.end }}

{% if role.highlights %}
<ul>
{% for item in role.highlights %}
  <li>{{ item }}</li>
{% endfor %}
</ul>
{% endif %}
{% endfor %}
