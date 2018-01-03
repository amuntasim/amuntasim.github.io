---
layout: page
permalink: /stories/
title: stories
description: Showcase your writing, short stories, or poems. Replace this text with your description.
---
<div class="container"> 
<ul class="post-list">
{% for poem in site.poetry reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
</div>