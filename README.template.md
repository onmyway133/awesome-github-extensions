# Awesome GitHub Extensions

A curated list of awesome browser extensions for GitHub. Inspired by [awesome-python](https://github.com/vinta/awesome-python), which is inspired by [awesome-php](https://github.com/ziadoz/awesome-php).

{% for category in data %}
## {{ category.category }}

{% for extension in category.extensions %}
* [{{ extension.name }}]({{ extension.url }}) <a href="{{ extension.url }}">{% for browser in extension.browsers %}<img alt="Support {{ browser }}" src="icons/{{ browser }}.png" width="16">{% endfor %}</a> - {{ extension.description }}
{% endfor %}

{% endfor %}
