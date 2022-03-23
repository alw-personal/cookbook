---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Recipe index

{% for cat in site.category-list %}
## {{ cat }}
<ul>
  {% for page in site.pages %}
      {% if page.categories contains cat %}
          <li><a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a></li>
      {% endif %}  <!-- page-category -->
  {% endfor %}  <!-- page -->
</ul>
{% endfor %}  <!-- cat -->