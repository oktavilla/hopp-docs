{% assign tableFileParam = {{include.definition}} %}
{% assign tableFile = site.data[tableFileParam] %}

| Content Field                                   | Required |
|:------------------------------------------------|:---------| {% for entry in tableFile %}
| {{entry.field}}                                 | {{entry.required}} | {% endfor %}
