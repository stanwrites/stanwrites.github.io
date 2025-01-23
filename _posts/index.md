---
layout: home
---

# Stan writes

{% for post in site.posts limit:10 %}
<div class="post">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <small class="date">{{ post.date | date: "%b %-d, %Y" }}</small>
  {{ post.excerpt }}
</div>
{% endfor %}

{% if paginator.total_pages > 1 %}
<a href="/archive">View Archive →</a>
{% endif %}
