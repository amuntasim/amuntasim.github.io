---
layout: page
permalink: /blog/
title: blog
description: Showcase your writing, short stories, or poems. Replace this text with your description
---
 <div class="container"> 
<ul class="post-list">
    {% for post in paginator.posts %}
      <li>
        <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
        <p>{{ post.description }}</p>
        <br/>
        <hr/>
      </li>
    {% endfor %}
</ul>
</div>