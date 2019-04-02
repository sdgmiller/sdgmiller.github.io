# Getting started!!

List all posts with the **gettingstarted** catergory 


  ## second attempt
  
{% for category in site.categories %}
{% if category[0] == 'gettingstarted' %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endif %}
{% endfor %}

## third attempt, this time using tags

  
{% for tag in site.tags %}
  {% if tag[0] == 'gettingstarted' %}
    <h3>{{ tag[0] }}</h3>
    <ul>
      {% for post in tag[1] %}
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  {% endif %}
{% endfor %}
