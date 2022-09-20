---
layout: page
title: Hello, World!
id: home
---

<ul>
{% for note in site.notes %}
<li><a href="{{ note.url }}{%- if site.use_html_extension -%}.html{%- endif -%}" class="internal-link">{{note.title}}</a>{% if note.category != null %} in {{note.category}}{% endif %} <span>({{ note.last_modified_at | date: "%d %B %Y" }})</li>
{% endfor %}
</ul>



