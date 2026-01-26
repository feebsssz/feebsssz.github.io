---
layout: page
title: Publications
permalink: /publications/
---

**Author identifiers**
- ORCID: https://orcid.org/0000-0002-3540-6452
- Google Scholar: https://scholar.google.com/citations?user=DVoYYdYAAAAJ&hl=en

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
