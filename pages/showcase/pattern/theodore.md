---
layout: cards
title: Theodore Showcases
permalink: /showcase/pattern/theodore
---
<div class="container">
<div class="row">
<div class="col">
<div class="card-columns blog">
{% for post in site.showcases %}
{% if post.category == 'theodore' %}
<div class="card hover-shadow mb-3">
<a href="{{ post.url }}" title="{{ post.title | escape}}"><img class="card-img-top img-fluid" src="/img{{ post.url }}{{ post.img }}" alt="{{ post.caption }}"></a>
<footer class="rounded-bottom">
<a href="/blog/category/{{ post.categories }}" title="Browse other posts in this category">{{ post.categories }}</a>
by <a href="/showcase/maker/{{ post.author }}" title="Browse other showcases by this maker">{{ post.author }}</a>
</footer>
</div>
{% endif %}
{% endfor %}
</div>
</div>
</div>
</div>
