---
layout: page
title: About
---

<br>

{% include about-image.html %}

<br>

{: .center}
I am a PhD candidate from [Technical University of Denmark][DTU]. My current research is `deformable mesh` and its applications.

## Highlights
* Research assistant, School of Computing, [NUS][NUS], Singapore, 2014
* MSc in Mechanical Engineering, [KAIST][Kaist], Korea, 2014
* Offshore developer, Sony Digital Network Application Inc., Vietnam, 2010-2012
* BS in Mechanical Engineering, honor program, [HUST][Hust], Vietnam, 2010

{% include button-gray.html title="More from my resume" url="/assets/cv.pdf"%}

## Publications
<ul class="paper-list">
  {% for post in site.categories.paper %}
    <li>
<hr>
      <span class="paper-meta"> {{ post.date | date: "%Y" }}. </span>
      <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>,
      <!-- {{ post.title }}, -->
      <span class="paper-meta"> {{ post.conf }}. </span>

      <!-- <a href="{{ post.url | prepend: site.baseurl }}" class="small button-fit">Read more</a> -->

      {% if post.image %}
        {% assign image = post.image %}
        {% include image-caption.html  img=image width="500"%}
      {% endif %}

      {% if post.video %}
        {% assign videos = post.video %}
        {% include youtube-paper-list.html  video=videos %}
      {% endif %}
      <!-- {{ post.excerpt }} -->
    </li>
  {% endfor %}
</ul>

[DTU]: http://www.dtu.dk
[Kaist]: http://www.kaist.edu/html/en/index.html
[Hust]: http://en.hust.edu.vn/home
[NUS]: http://www.nus.edu.sg
[cv]: /assets/cv.pdf
