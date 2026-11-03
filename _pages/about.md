---
layout: "hybrid"
title: "Home"
permalink: "/"
---

<p class="eyebrow">Research · Engineering · Security</p>
# Sabbir Muhammad Saleh

<p class="intro">Software Engineering & Cybersecurity Researcher</p>

I hold a PhD in Computer Science from Western University, Canada. My work investigates secure CI/CD pipelines, software supply-chain security, AI-assisted security analysis, and trustworthy security evidence.

My doctoral research developed **DevSecLogs**, a stage-aware framework and research prototype for making heterogeneous CI/CD security observations more explainable, traceable and integrity-checkable.

<div class="actions"><a class="button" href="{{ '/projects/devseclogs/' | relative_url }}">Explore DevSecLogs</a><a class="button secondary" href="{{ '/publications/' | relative_url }}">Publications</a><a class="button secondary" href="{{ '/cv/' | relative_url }}">CV & Contact</a></div>

## Research at a glance

<div class="cards">{% for item in site.data.hybrid_research limit:4 %}<article class="card"><h3>{{ item.name }}</h3><p>{{ item.detail }}</p></article>{% endfor %}</div>

## Recent highlights

<div class="feed">{% for item in site.data.hybrid_news limit:4 %}<article class="feed-item"><span>{{ item.label }}</span><div><strong>{{ item.title }}</strong><p>{{ item.detail }}</p></div></article>{% endfor %}</div>

[All talks and news]({{ '/activity/' | relative_url }})
