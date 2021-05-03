---
layout: default
---
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
	  <br>
	  <br>
	  <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
	<br>
  {% endfor %}
</ul>