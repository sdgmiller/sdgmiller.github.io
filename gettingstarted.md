# Getting started!!

List all posts with the **gettingstarted** catergory 

<!--{% for category in site.categories %}-->
  <h3>{{ site.categories["gettingstarted"][0] }}</h3>
  <ul>
    {% for post in site.categories["gettingstarted"][0] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
