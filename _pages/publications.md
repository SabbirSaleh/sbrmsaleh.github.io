---
layout: "hybrid"
title: "Publications"
permalink: "/publications/"
---

<p class="eyebrow">Research record</p>
# Publications

A curated selection of peer-reviewed papers and a presented, publication-pending conference paper. The complete list is available on [Google Scholar](https://scholar.google.com/citations?user=mm7bYG4AAAAJ).

{% assign ordered = site.publications | sort: 'year' | reverse %}
{% assign previous_year = 0 %}
{% for paper in ordered %}
{% if paper.year != previous_year %}
{% unless forloop.first %}</div>{% endunless %}
<h2 class="year">{{ paper.year }}</h2><div class="feed">
{% assign previous_year = paper.year %}{% endif %}
<article class="paper"><p class="eyebrow">{{ paper.kind }} · {{ paper.status }}</p><h3><a href="{{ paper.url | relative_url }}">{{ paper.title }}</a></h3><p>{{ paper.authors }}</p><p class="fine">{{ paper.venue }}</p>{% if paper.doi %}<p><a href="https://doi.org/{{ paper.doi }}" target="_blank" rel="noopener noreferrer">DOI ↗</a></p>{% endif %}</article>
{% endfor %}{% if ordered.size > 0 %}</div>{% endif %}

<small>CASCON 2026 posters are listed as presentations under Talks & News, not as archival conference papers. The ICSEng paper is labelled publication pending; no DOI is claimed.</small>
