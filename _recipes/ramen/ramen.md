---
layout: page
title: Ramen
permalink: /ramen/
has_children: true
categories: [Mains, Japanese, Noodles]
---

![]({{ site.baseurl }}/recipes/images/210304-ramen.jpg)
![]({{ site.baseurl }}/recipes/images/210318-ramen.jpg)

<ul class="post-list">
    {% for post in site.recipes %}
    {% if post.parent == "Ramen" %}
    {% include post-list-item.html %}
    {% endif %}
    {% endfor %}
</ul>