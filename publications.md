---
layout: page
title: Publications
permalink: /publications/
---

**Author identifiers**
- ORCID: [0000-0002-3540-6452](https://orcid.org/0000-0002-3540-6452)
- Google Scholar: [Profile](https://scholar.google.com/citations?user=DVoYYdYAAAAJ&hl=en)

---

{% assign pubs = site.data.publications | sort: "year" | reverse %}

{% for pub in pubs %}
**{{ pub.title }}**
{{ pub.authors }}
*{{ pub.venue }}*{% if pub.volume %}, {{ pub.volume }}{% endif %}{% if pub.pages %}, pp. {{ pub.pages }}{% endif %} ({{ pub.year }}){% if pub.note %} – {{ pub.note }}{% endif %}
{% if pub.type %}[{{ pub.type }}]{% endif %}{% if pub.link %} · [Link]({{ pub.link }}){% endif %}

{% endfor %}
