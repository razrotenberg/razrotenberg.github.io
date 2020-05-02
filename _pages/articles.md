---
layout: page
title: Articles
permalink: /articles/
---

{% for article in site.data.articles %}

<hr>

{:.article-name}
### [{{ article.name }}]({{ article.url }}){:target="_blank"}

##### {{ article.date }}

{{ article.content }}

[Read more...]({{article.url}}){:.button target="_blank"}

{% endfor %}
