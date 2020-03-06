{% assign parentTitle = {{include.parent}} %}
<ul>
{% for page in site.pages %}
{% if page.parent == parentTitle %}
  <li><a href="{{page.url}}">{{ page.title }}</a></li>
{% endif %}
{% endfor %}
</ul>
