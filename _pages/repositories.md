---
layout: page
permalink: /repositories/
title: repositories
description: Overview of programming projects I contribute to.
nav: true
nav_order: 3
---

I use GitHub to share code, document analysis workflows, and support collaborative research projects. A few selected repositories are linked below.

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-stretch">
  {% for repo in site.data.repositories.github_repos %}
    {% assign repo_parts = repo | split: '/' %}
    <div class="repo p-2 text-left">
      <div class="card hoverable h-100">
        <div class="card-body">
          <h5 class="card-title"><a href="https://github.com/{{ repo }}" target="_blank" rel="noopener noreferrer"><i class="fab fa-github"></i> {{ repo }}</a></h5>
          <p class="card-text">View the {{ repo_parts[1] }} repository on GitHub.</p>
        </div>
      </div>
    </div>
  {% endfor %}
</div>

More code and project repositories are available on my [GitHub profile](https://github.com/CPRyan).
