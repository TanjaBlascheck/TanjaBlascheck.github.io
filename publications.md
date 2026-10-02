---
layout: default
title: Publications
permalink: /publications/
---

# Publications

{% for pub in site.data.publications %}
* **{{ pub.authors }}**. "{{ pub.title }}". *{{ pub.venue }}*, {{ pub.year }}. 
  {% if pub.pdf %}[<a href="{{ pub.pdf | relative_url }}">PDF</a>]{% endif %}
  {% if pub.code %}[<a href="{{ pub.code }}">Code</a>]{% endif %}
{% endfor %}