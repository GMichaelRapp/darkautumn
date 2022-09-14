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
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
  {% endfor %}
</ul>

---

{% include footer.html %}
