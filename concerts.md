---
layout: page
title: Concerts
permalink: /concerts/
---

<h1 class="page-heading">Upcomming</h1>
<div>
  <ul class="post-list">
  {% assign sorted_pages = (site.categories.concerts | sort: 'concert_date') %}
	{% for concerts in sorted_pages %}
      <li>
        <span class="post-meta">{{ concerts.concert_date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ concerts.url | prepend: site.baseurl }}">{{ concerts.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>
  </div>

