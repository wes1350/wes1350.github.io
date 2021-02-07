# Posts

Guides, explanations, and comments on concrete topics.

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li>({{post.date | date: "%Y-%m-%d"}}) <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
