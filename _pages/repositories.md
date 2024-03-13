---
layout: page
permalink: /repositories/
title: data & code repositories
description: data & code repositories used in my publications.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}