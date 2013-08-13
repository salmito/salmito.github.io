---
layout: page
title: Welcome!
tagline: <br />Assorted thoughts in my head...
---
{% include JB/setup %}

* Leda, my personal project! [Leda.co](http://leda.co/)
* Curriculum: 
* Twitter: [TiagoBraw](http://twitter.com/TiagoBraw/)
* Github: [Salmito](http://github.com/Salmito/)

Archive:

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



