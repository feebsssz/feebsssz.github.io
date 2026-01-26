---
layout: page
title: Education
permalink: /education/
---

{% for degree in site.data.education %}
### {{ degree.degree }}
**{{ degree.institution }}** | {{ degree.start }} – {{ degree.end }}

{% if degree.details %}
{% for item in degree.details %}
- {{ item }}
{% endfor %}
{% endif %}

{% endfor %}
