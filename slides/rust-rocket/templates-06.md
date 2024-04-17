#### Tera Templates

<small>

Tera is a template engine inspired by Jinja2 and the Django template language.

https://keats.github.io/tera/

</small>

```html
<title>{% block title %}{% endblock title %}</title>
<ul>
{% for user in users %}
  <li><a href="{{ user.url }}">{{ user.username }}</a></li>
{% endfor %}
</ul>
```


<aside class="notes">
</aside>
