---
layout: single
---


<div class="row">
<div class="large-4 medium-4 columns" markdown="1">
  {: .center}
  ![portrait](/img/portrait.png)
</div><div class="large-8 medium-8 columns" markdown="1">
  I am a PhD candidate from [Technical University Denmark][DTU]. My current research is deformable mesh and its applications.

  {% include button-gray.html title="More from my CV" url="/assets/cv.pdf"%}
</div>
</div>

### Highlights

* Research assistant, School of Computing, [NUS][NUS], Singapore, 2014
* MSc in Mechanical Engineering, [KAIST][Kaist], Korea, 2014
* Offshore developer, Sony Digital Network Application Inc., Vietnam, 2010-2012
* BS in Mechanical Engineering, honor program, [HUST][Hust], Vietnam, 2010


{% comment %}
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
{% endcomment %}


### Publications
<ul class="post-list">
  {% for post in site.categories.paper %}
      <a class="paper-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>

      <span class="post-meta"> {{ post.conf }}, {{ post.date | date: "%Y" }}. </span>

      <p>{{ post.excerpt }}</p>
  {% endfor %}
</ul>

[DTU]: http://www.dtu.dk
[Kaist]: http://www.kaist.edu/html/en/index.html
[Hust]: http://en.hust.edu.vn/home
[NUS]: http://www.nus.edu.sg
[cv]: /assets/cv.pdf
