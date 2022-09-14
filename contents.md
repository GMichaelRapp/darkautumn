---

layout: default
title: Table of Contents
nav_order: 1.75
comments: false

---

## Table of Contents

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}">{{post.date}}</a>
    </li>
  {% endfor %}
</ul>

---

{% include footer.html %}
