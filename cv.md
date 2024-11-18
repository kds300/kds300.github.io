---
layout: cv
title: Curriculum Vitae
permalink: /cv
---
# Education

{% include education.html %}

# Experience

{% include experience.html %}

# Skills

{% include skills.html %}

# Papers

{% for paper in site.data.papers %}
{{ paper.authors }}.
*{{ paper.title }}*.
{% if paper.journal %}{{ paper.journal }}{% endif %} {% if paper.journal %}({{ paper.year }}){% endif %}
{% endfor %}

# Presentations

{% for presentation in site.data.presentations %}
{{ presentation.authors }}.
*{{ presentation.title }}*.
{{ presentation.type }}.
{{ presentation.where }}.
{% endfor %}