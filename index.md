---
layout: default
---
Pages:
<ul>
  {% for page in site.pages %}
    <li>
      <h2><a href="{{ page.url }}">{{ page.title }}</a></h2>
      <p>{{ page.excerpt }}</p>
      <p>{{ page.date }}</p>
      <p>{{ page.id }}</p>
    </li>
  {% endfor %}
</ul>
Posts:
<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
---
Last updated {{site.time}}