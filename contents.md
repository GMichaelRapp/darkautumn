---

layout: default
title: Table of Contents
nav_order: 1.75
comments: false

---

<div class="constrain">
   <h1>Table of Contents</h1> 
   <section class="card-list">
           {% for post in site.posts offset:1 %}
           <div class="card">
                   <img src="{{ post.thumbnail_image.small }}" />
                   <div class="card-details">
                   <h3>{{ post.date | date:"%d %b" }} - {{ post.title }}</h3>
               <a href="{{ post.url }}" class="btn">Read More</a>
                   </div>
               </div>
           {% endfor %}
          
   </section>
</div>

---

{% include footer.html %}
