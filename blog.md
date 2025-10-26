---
layout: page
title: Blog
permalink: /blog/
---

**Coming soon.** I started writing blog posts more than twenty years ago, but it’s been a long while since I’ve kept a public blog. I’m planning to start posting again—short, practical notes on NLP, data mining, teaching, and interdisciplinary collaborations. Stay tuned.

You’ll be able to browse posts by category <a href="{{ site.baseurl }}/categories/">here</a> once I’m rolling.

<hr>

{% if site.posts and site.posts != empty %}
<ul class="listing">
  {% assign current_year = "" %}
  {% for post in site.posts %}
    {% capture y %}{{ post.date | date: "%Y" }}{% endcapture %}
    {% if current_year != y %}
      {% assign current_year = y %}
      <li class="listing-seperator">{{ y }}</li>
    {% endif %}
    <li class="listing-item">
      <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date: "%Y-%m-%d" }}</time>
      <a href="{{ site.baseurl }}{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
{% else %}
<p>No posts yet — check back soon.</p>
{% endif %}
