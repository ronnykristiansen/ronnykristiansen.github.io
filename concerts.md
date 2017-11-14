---
layout: page
title: Retrospektiv
permalink: /retrspectiveKIT/
---

<h1 class="page-heading">Upcomming</h1>
<div>
  <ul class="post-list">
  {% assign sorted_pages = (site.categories.retrospectiveKIT | sort: 'concert_date') %}
	{% for page in sorted_pages %}
      <li>
        <span class="post-meta">{{ page.concert_date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>
  </div>

