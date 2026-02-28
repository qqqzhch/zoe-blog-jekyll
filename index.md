---
layout: home
---

## 最新文章

{% for post in site.posts limit: 5 %}
### [{{ post.title }}]({{ site.url }}{{ post.url }})
<small>{{ post.date | date: "%Y年%m月%d日" }}</small>

{{ post.excerpt | strip_html | truncate: 200 }}

{% endfor %}
