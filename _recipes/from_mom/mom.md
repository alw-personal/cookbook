---
layout: page
title: Recipes from Mom
permalink: /mom/
has_children: true
---

<ul class="post-list">
    {% for post in site.recipes %}
    {% if post.parent == "From Mom" %}
    {% include post-list-item.html %}
    {% endif %}
    {% endfor %}
</ul>