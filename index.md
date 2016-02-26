---
layout: page
title: About
---

<br>

{% include about-image.html %}

<br>

{: .center}
`PhD candidate, cycling lover` <br> `and coffee enthusiasm`

<!-- ## Research
<ul class="paper-list">
  {% for post in site.categories.research %}
    <li>
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      <span class="paper-meta"> {{ post.date | date: "%Y" }}. </span>

      {{ post.excerpt }}

    </li>
  {% endfor %}
</ul> -->

## Highlights
* PhD candidate, Image analysis and Computer Graphics, [DTU][DTU], *Denmark*, now
* Research assistant, School of Computing, [NUS][NUS], *Singapore*, 2014
* MSc in Mechanical Engineering, [KAIST][Kaist], *Korea*, 2014
* Offshore developer, Sony Digital Network Application Inc., *Vietnam*, 2010-2012
* BS in Mechanical Engineering, honor program, [HUST][Hust], *Vietnam*, 2010

{% include button-gray.html title="More from my resume" url="/assets/cv.pdf"%}

## Publications
<ul class="paper-list">
  {% for post in site.categories.paper %}
  <hr>
    <li>
      <a  href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>,
      <span class="paper-meta"> {{ post.conf }}. </span>
      <span class="paper-meta"> {{ post.date | date: "%Y" }}. </span>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

[DTU]: http://www.dtu.dk
[Kaist]: http://www.kaist.edu/html/en/index.html
[Hust]: http://en.hust.edu.vn/home
[NUS]: http://www.nus.edu.sg
[cv]: /assets/cv.pdf
