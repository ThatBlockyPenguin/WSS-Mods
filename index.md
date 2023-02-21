# PenguinMods Index

{% assign doclist = site.pages | sort: 'url' %}
<ul>
  {% for doc in doclist %}
  {% if doc.name contains '.md' %}
  <li><a href="{{ site.baseurl }}{{ doc.url }}">{{ doc.name }}</a></li>
  {% endif %}
  {% endfor %}
</ul>