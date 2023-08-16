---
layout: page
title: посты
permalink: /about/
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

### Jekyll *умеет* раскрашивать ваш код 

```java
parameters a, b // mod function
if empty( b )
  result := 0
  return
endif
result := a - int( a / b ) * b  
```
~

Книжное братство [flibusta.is](https://flibusta.is)

Какие версии поддерживает gp ? [gp.com/versions](https://pages.github.com/versions)

( gp = github pages )

hugo [hugo](https://hisava.github.io/hugo)

