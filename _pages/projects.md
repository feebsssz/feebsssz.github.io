---
layout: page
title: Projects
---

{% for project in site.data.projects %}
### {{ project.name }}
{{ project.description }}

{% if project.highlights %}
<ul>
{% for item in project.highlights %}
  <li>{{ item }}</li>
{% endfor %}
</ul>
{% endif %}
{% endfor %}
