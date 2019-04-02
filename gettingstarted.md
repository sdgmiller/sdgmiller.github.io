# Getting started!!

List all posts with the **gettingstarted** catergory 

## first attempt
<!--{% for category in site.categories %}-->
  <h3>{{ site.categories["gettingstarted"][0] }}</h3>
  <ul>
    {% for post in site.categories["gettingstarted"][0] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
  
  ## second attempt
  
  {% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

## third attempt, this time using tags

  ## second attempt
  
  {% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
