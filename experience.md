---
layout: page
title: Experience
permalink: /experience/
---

{% for role in site.data.experience %}
### {{ role.role }}
**{{ role.organization }}**{% if role.department %}, {{ role.department }}{% endif %} | {{ role.start }} – {{ role.end }}

{% if role.projects %}
{% for project in role.projects %}
*{{ project.name }}*
{% for item in project.items %}
- {{ item }}
{% endfor %}

{% endfor %}
{% endif %}

{% if role.items %}
{% for item in role.items %}
- {{ item }}
{% endfor %}
{% endif %}

---

{% endfor %}
