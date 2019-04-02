# Tutorials!!

List all **tutorials** posts


## Using categories
  
{% for category in site.categories %}
{% if category[0] == 'tutorials' %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endif %}
{% endfor %}

## Using tags
  
{% for tag in site.tags %}
{% if tag[0] == 'tutorials' %}
<h3>{{ tag[0] }}</h3>
<ul>
{% for post in tag[1] %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
{% endif %}
{% endfor %}
