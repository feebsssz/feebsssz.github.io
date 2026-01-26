---
layout: page
title: Education
permalink: /education/
---

{% for degree in site.data.education %}
### {{ degree.degree }} — {{ degree.institution }}
{{ degree.start }} – {{ degree.end }}

{% if degree.details %}
<ul>
{% for item in degree.details %}
  <li>{{ item }}</li>
{% endfor %}
</ul>
{% endif %}
{% endfor %}
