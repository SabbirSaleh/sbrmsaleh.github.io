---
layout: "hybrid"
title: "Talks & News"
permalink: "/activity/"
---

<p class="eyebrow">Presentations and updates</p>
# Talks & News

## News

<div class="feed">{% for item in site.data.hybrid_news %}<article class="feed-item"><span>{{ item.label }}</span><div><strong>{{ item.title }}</strong><p>{{ item.detail }}</p></div></article>{% endfor %}</div>

## Presentations and posters

{% assign sorted_talks = site.talks | sort: 'date' | reverse %}
<div class="feed">{% for talk in sorted_talks %}<article class="paper"><p class="eyebrow">{{ talk.date | date: '%B %Y' }} · {{ talk.status }}</p><h3><a href="{{ talk.url | relative_url }}">{{ talk.title }}</a></h3><p class="fine">{{ talk.event }}</p></article>{% endfor %}</div>
