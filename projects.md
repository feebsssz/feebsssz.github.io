---
layout: page
title: DS/ML Projects
permalink: /projects/
---

{% for project in site.data.projects %}
### {{ project.name }}

{{ project.description }}

**Skills:** {{ project.skills }}{% if project.ref %}
**Ref:** {{ project.ref }}{% endif %}

---

{% endfor %}
