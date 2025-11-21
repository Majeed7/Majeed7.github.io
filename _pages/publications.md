---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
---

{% comment %}Simplified dynamic yearly grouping with internal links to publication pages{% endcomment %}
{% assign pubs = site.publications | sort: 'date' | reverse %}
{% assign years = pubs | map: 'year' | uniq %}

{% for y in years %}
## {{ y }}
<ul>
{% for p in pubs %}{% if p.year == y %}<li><a href="{{ p.url | relative_url }}">{{ p.title | markdownify | strip_html }}</a>. {{ p.citation }} {% if p.link and p.link != p.url %}[<a href='{{ p.link }}' rel="noopener">external</a>]{% endif %}{% if p.doi %} DOI: <a href='https://doi.org/{{ p.doi }}'>{{ p.doi }}</a>{% endif %}</li>{% endif %}{% endfor %}
</ul>
{% endfor %}
