---
layout: page
title: Articles
permalink: /articles/
---

{% if site.data.articles.size > 0 %}
---
{% endif %}


{% for article in site.data.articles %}

{:.article-name}
### [{{ article.name }}]({{ article.url }}){:target="_blank"}
##### {{ article.date }}
{{ article.content }}

---
{% endfor %}
