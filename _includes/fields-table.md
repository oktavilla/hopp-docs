{% assign tableFileParam = {{include.definition}} %}
{% assign tableFile = site.data[tableFileParam] %}
{% assign parentTableFileParam = {{include.parent_definition}} %}
{% assign parentTableFile = site.data[parentTableFileParam] %}

<table>
  <thead>
    <tr>
      <th style="text-align: left;">Name</th>
      <th style="text-align: left;">Type</th>
      <th style="text-align: left;">Required</th>
      <th style="text-align: left;">Comment</th>
    </tr>
  </thead>
  <tbody>
    {% for entry in parentTableFile %}
    <tr class="parent-definition">
      <td>
        {{entry.field}} *
      </td>
      <td>
        {% if entry.field_type %}
          {% assign file_name = entry.field_type | prepend: 'field-type-' | append: '.md' %}
          {% assign field_type_page = site.pages | where: 'name', file_name %}
          {% assign field_type_title = field_type_page[0].title %}
          {{ field_type_title | replace: " Field", "" }}
        {% else %}
          String
        {% endif %}
      </td>
      <td>{{entry.required}}</td>
      <td>{{entry.comment}}</td>
    </tr>
    {% endfor %}
    {% for entry in tableFile %}
    <tr>
      <td>
        {{entry.field}}
      </td>
      <td>
        {% if entry.field_type %}
          {% assign file_name = entry.field_type | prepend: 'field-type-' | append: '.md' %}
          {% assign field_type_page = site.pages | where: 'name', file_name %}
          {% assign field_type_title = field_type_page[0].title %}
          <a href="{{entry.field_type | prepend: "field-type-" + site.base_url}}.html">{{ field_type_title | replace: " Field", "" }}</a>
        {% else %}
          String
        {% endif %}
      </td>
      <td>{{entry.required}}</td>
      <td>{{entry.comment}}</td>
    </tr>
    {% endfor %}  </tbody>
</table>
