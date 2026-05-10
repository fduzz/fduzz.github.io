---
layout: page
permalink: /research/
title: Research
description: 
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
{% comment %}
Previous research renderer, kept for quick rollback:
<div class="publications">

{% bibliography -f {{ site.scholar.bibliography }} %}

</div>
{% endcomment %}

<div class="publications research-one-line">
  <section class="research-section">
    <h2 class="research-section-title">Published &amp; Forthcoming</h2>
    {% bibliography -f {{ site.scholar.bibliography }} --template bib_research --query @*[category=published]* %}
  </section>

  <section class="research-section">
    <h2 class="research-section-title">Working Papers</h2>
    {% bibliography -f {{ site.scholar.bibliography }} --template bib_research --query @*[category=working]* %}
  </section>
</div>
