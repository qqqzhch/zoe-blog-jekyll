---
layout: home
---

## 最新文章

{% assign posts = site.posts | sort: "date" | reverse %}
{% for post in posts limit: 10 %}
### [{{ post.title }}]({{ site.url }}{{ post.url }})
<small>{{ post.date | date: "%Y年%m月%d日" }}</small>

{{ post.excerpt | strip_html | truncate: 200 }}

{% endfor %}
