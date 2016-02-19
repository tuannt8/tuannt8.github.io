
{: .center}
![portrait](/img/portrait.png)

{: .center}
#Tuan Nguyen

I am a PhD candidate from [Technical University Denmark][DTU]. My current research is deformable mesh and its applications. My  [CV][cv].

###Highlights

* Research assistant, School of Computing, [NUS][NUS], Singapore, 2014
* MSc in Mechanical Engineering, [KAIST][Kaist], Korea, 2014
* Offshore developer, Sony Digital Network Application Inc., Vietnam, 2010-2012
* BS in Mechanical Engineering, honor program, [HUST][Hust], Vietnam, 2010

###My researches
<ul class="post-list">
  {% for post in site.categories.research %}
    <li>
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      <span class="post-meta">{{ post.date | date: "%Y" }}</span>
      {{ post.excerpt }}
    </li>



  {% endfor %}
</ul>


[DTU]: http://www.dtu.dk
[Kaist]: http://www.kaist.edu/html/en/index.html
[Hust]: http://en.hust.edu.vn/home
[NUS]: http://www.nus.edu.sg
[cv]: /assets/cv.pdf
