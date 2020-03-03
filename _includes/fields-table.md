{% assign tableFileParam = {{include.definition}} %}
{% assign tableFile = site.data[tableFileParam] %}
{% assign parentTableFileParam = {{include.parent_definition}} %}
{% assign parentTableFile = site.data[parentTableFileParam] %}

<table>
  <thead>
    <tr>
      <th style="text-align: left;">Field Name</th>
      <th style="text-align: left;">Required</th>
      <th style="text-align: left;">Comment</th>
    </tr>
  </thead>
  <tbody>
    {% for entry in parentTableFile %}
    <tr class="parent-definition">
      <td>
        {% if entry.data_model %}
          <a href="{{entry.data_model | prepend: site.base_url}}.html">{{entry.field}}</a>
        {% else %}
          {{entry.field}}
        {% endif %}
        *
      </td>
      <td>{{entry.required}}</td>
      <td>{{entry.comment}}</td>
    </tr>
    {% endfor %}
    {% for entry in tableFile %}
    <tr>
      <td>
        {% if entry.data_model %}
          <a href="{{entry.data_model | prepend: site.base_url}}.html">{{entry.field}}</a>
        {% else %}
          {{entry.field}}
        {% endif %}
      </td>
      <td>{{entry.required}}</td>
      <td>{{entry.comment}}</td>
    </tr>
    {% endfor %}  </tbody>
</table>
