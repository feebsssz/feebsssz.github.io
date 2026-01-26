---
layout: page
title: Publications
---

{% assign pubs = site.data.publications | sort: "year" | reverse %}

{% for pub in pubs %}
### {{ pub.title }}

**{{ pub.authors }}**  
*{{ pub.venue }}*, {{ pub.year }}  
{% if pub.type %}{{ pub.type }}{% endif %}
{% if pub.link %} · [Link]({{ pub.link }}){% endif %}

---
{% endfor %}
