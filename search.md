```java
{
  {% assign comma = false %}
  {% for page in site.html_pages %}{% if page.search_exclude != true %}{% if comma == true%},{% endif %}"{{ forloop.index0 }}": {
    "title": "{{ page.title | replace: '&amp;', '&' }}",
    "content": "{{ page.content | markdownify | replace: '</h', ' . </h' | replace: '<hr', ' . <hr' | replace: '</p', ' . </p' | replace: '</ul', ' . </ul' | replace: '</tr', ' . </tr' | replace: '</li', ' | </li' | replace: '</td', ' | </td' | strip_html | escape_once | remove: 'Table of contents' | remove: '```'  | remove: '---' | replace: '\', ' ' | replace: ' .  .  . ', ' . ' | replace: ' .  . ', ' . ' | normalize_whitespace }}",
    "url": "{{ page.url | absolute_url }}",
    "relUrl": "{{ page.url }}"
  }{% assign comma = true %}
  {% endif %}{% endfor %}
}
```
