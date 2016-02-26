---
layout: default
title: Blog
permalink: /blog/
---
<div class="home">

  <h1>Posts</h1>

  <ul class="posts">
    {% for post in site.categories.blog %}
      <li>
      <span class="post-date"> {{ post.date | date: "%B %d, %Y" }}. </span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>

        <p>
        <!-- {{ post.excerpt }} -->
        </p>
      </li>
    {% endfor %}
  </ul>

</div>
