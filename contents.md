---

layout: default
title: Table of Contents
nav_order: 1.75
comments: false

---

<div class="constrain">
   <h1>Table of Contents</h1> 
           {% for post in site.posts offset:1 %}
                   <h3>{{ post.title }} - {{ post.date | date:"%d %b" }}</h3>
           {% endfor %}
          
   </section>
</div>

---

{% include footer.html %}
