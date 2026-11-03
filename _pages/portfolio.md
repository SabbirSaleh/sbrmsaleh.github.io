---
layout: "hybrid"
title: "Projects"
permalink: "/projects/"
---

<p class="eyebrow">Technical portfolio</p>
# Projects and software

<p class="intro">Research implementations and technical demonstrations, not commercial security products.</p>

<div class="cards">
{% for project in site.projects %}<article class="card"><p class="eyebrow">{{ project.status }}</p><h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2><p>{{ project.subtitle }}</p></article>{% endfor %}
<article class="card"><h3>AI-assisted log intelligence</h3><p>Topic modelling and anomaly detection research for operational security data.</p></article>
<article class="card"><h3>Evidence integrity</h3><p>Off-chain evidence with cryptographic commitments and digest verification.</p></article>
</div>
