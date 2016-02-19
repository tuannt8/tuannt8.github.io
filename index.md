---
layout: single
---

<!-- <div class="home">

  <h1 class="page-heading">Posts</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div> -->

<!-- {% capture about %}{% include_relative about_content.md %}{% endcapture %}
{{ about  | markdownify }} -->

<!-- <div  class="home" markdown="1">
  {% include_relative about_content.md %}
</div> -->

{: .center}
![portrait](/img/portrait.png)

{: .center}
# Tuan Nguyen

I am a PhD candidate from [Technical University Denmark][DTU]. My current research is deformable mesh and its applications. My  [CV][cv].

### Highlights

* Research assistant, School of Computing, [NUS][NUS], Singapore, 2014
* MSc in Mechanical Engineering, [KAIST][Kaist], Korea, 2014
* Offshore developer, Sony Digital Network Application Inc., Vietnam, 2010-2012
* BS in Mechanical Engineering, honor program, [HUST][Hust], Vietnam, 2010

### My researches
<ul class="post-list">
  {% for post in site.categories.research %}
    <li>
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      <span class="post-meta">({{ post.date | date: "%Y" }})</span>
      <!-- {{ post.description }} -->
      {{ post.excerpt }}
      {% assign image = post.images[0] %}
      {% include image.html image=image %}
    </li>
  {% endfor %}
</ul>

### Publications
<ul class="post-list">
  {% for post in site.categories.paper %}
    <!-- <li> -->
      <!-- <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a> -->
      <!-- <span class="post-meta">({{ post.date | date: "%Y" }})</span> -->
      <!-- {{ post.description }} -->
      {{ post.excerpt }}
      {% if post.description %}
        <a href="{{ post.url | prepend: site.baseurl }}">Read more...</a>
      {% endif %}
    <!-- </li> -->
  {% endfor %}
</ul>

[DTU]: http://www.dtu.dk
[Kaist]: http://www.kaist.edu/html/en/index.html
[Hust]: http://en.hust.edu.vn/home
[NUS]: http://www.nus.edu.sg
[cv]: /assets/cv.pdf
