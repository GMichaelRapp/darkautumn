---

layout: home
title: Home
nav_order: 0
comments: false

---

{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}

{% if post.content.size > post.excerpt.size %}

---

{% include footer.html %}
