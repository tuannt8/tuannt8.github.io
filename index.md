---
layout: about
title: About
---

<!-- <br> -->

{% include about-image.html %}

<br>

{: .center}
~~~
PhD candidate, cycling lover and coffee enthusiasm
~~~


## Highlights
* PhD candidate, Image analysis and Computer Graphics, [DTU][DTU], *Denmark*, now
* Research assistant, School of Computing, [NUS][NUS], *Singapore*, 2014
* MSc in Mechanical Engineering, [KAIST][Kaist], *Korea*, 2014
* Offshore developer, Sony Digital Network Application Inc., *Vietnam*, 2010-2012
* BS in Mechanical Engineering, honor program, [HUST][Hust], *Vietnam*, 2010


{: .center}
<a target="blank" href="{{ "/assets/cv.pdf" | prepend: site.baseurl }}"> **More from my resume** </a>
<br>
<br>


## Publications
<ul class="paper-list">
  {% for post in site.categories.paper %}
  <hr>
    <li>
      <a class="link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>,
      <span class="meta"> {{ post.conf }}. </span>
      <span class="meta"> {{ post.date | date: "%Y" }}. </span>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

[DTU]: http://www.dtu.dk
[Kaist]: http://www.kaist.edu/html/en/index.html
[Hust]: http://en.hust.edu.vn/home
[NUS]: http://www.nus.edu.sg
[cv]: /assets/cv.pdf
