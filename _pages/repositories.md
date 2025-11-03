---
layout: page
permalink: /repositories/
title: Repositories
description: 
nav: true
nav_order: 2
---

{% if site.data.repositories.github_repos %}

<p style="text-align: center;">Here are some selected GitHub repositories of mine - drawn both from research and personal projects.</p>

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-center align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
