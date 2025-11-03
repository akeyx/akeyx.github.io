---
layout: default
permalink: /blog/
---

```
cat /dev/urandom
```

## Latest Posts

<ul class="post-list">
{% for post in site.posts %}
    <li>
        <a href="{{ post.url | relative_url }}">
            {{ post.title }}
        </a>
        <span class="post-meta">
            Published on: {{ post.date | date: "%B %d, %Y" }}
        </span>
    </li>
{% endfor %}
</ul>
