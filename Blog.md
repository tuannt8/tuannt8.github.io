---
layout: page
title: Blog
permalink: /blog/
---

<ul class="post-list">
  {% for post in site.categories.blog %}
    <li>
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      <span class="paper-meta"> {{ post.date | date: "%B %d, %Y" }}. </span>

      <!-- <a href="{{ post.url | prepend: site.baseurl }}" class="small button-fit">Read more</a> -->

      <!-- {% if post.image %}
        {% assign image = post.image %}
        {% include image-caption.html  img=image width="500"%}
      {% endif %}

      {% if post.video %}
        {% assign videos = post.video %}
        {% include youtube-paper-list.html  video=videos %}
      {% endif %} -->

      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
