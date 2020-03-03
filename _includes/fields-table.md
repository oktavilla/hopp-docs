{% assign tableFileParam = {{include.definition}} %}
{% assign tableFile = site.data[tableFileParam] %}

| Content Field                                                                            | Required |
|:-----------------------------------------------------------------------------------------|:---------| {% for entry in tableFile %}
| {% if entry.link %}[{{entry.field}}]({{entry.link}}){% else %}{{entry.field}}{% endif %} | {{entry.required}} | {% endfor %}
