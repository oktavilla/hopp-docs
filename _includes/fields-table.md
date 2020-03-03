{% assign tableFileParam = {{include.definition}} %}
{% assign tableFile = site.data[tableFileParam] %}

| Content Field                                                                            | Required | Comment  |
|:-----------------------------------------------------------------------------------------|:---------|:---------| {% for entry in tableFile %}
| {% if entry.data_model %}[{{entry.field}}]({{entry.data_model | prepend: site.base_url}}.html){% else %}{{entry.field}}{% endif %} | {{entry.required}} | {{entry.comment}} | {% endfor %} 
