---
layout: default
---

物忘れ激しいお年頃なので色々と書き残しつつ、興味本位で技術的な試行錯誤や世の中のあれこれについて考える。

{% for category in site.categories %}
  {% capture name %}{{ category[0] }}{% endcapture %}
  <h2>{{ name }} ({{ site.categories[name] | size }})</h2>
  <ul class="posts">
  {% for post in site.categories[name] %}
    <li>
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      - <span class="post-date">{{ post.date | date: "%Y.%m.%d" }}</span>
    </li>
  {% endfor %}
  </ul>
{% endfor %}
