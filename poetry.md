---
layout: page
comments: true
permalink: /poetry/
title: poetry
description: Showcase your writing, short stories, or poems. Replace this text with your description.
---

<ul class="post-list">
{% for poem in site.poetry reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y — %H:%M' }}
        <a class="poem-meta" href="{{ poem.url | prepend: site.baseurl | append: '#disqus_thread' }}">0 Comments</a> </p>
      </li>
{% endfor %}
</ul>

 <script id="dsq-count-scr" src="//seven-times-have-i.disqus.com/count.js" async></script>
