---
title: Table of Contents
layout: page
---

<ul class="index-buttons">
<li><a href="{{ "/about.html" | absolute_url }}">About</a></li>
<li><a href="{{ "/forum/index.html" | absolute_url }}">Assignments &amp; Forum</a></li>
<li><a href="https://intmus.github.io/inttheory18-19/">IntMus: Theory</a></li>
</ul>

{% for chapter in site.collections %}
{% if chapter.label != 'posts' %}
## {{ chapter.name }}
{% for lesson in chapter.docs %}
- [{{ lesson.title }}]({{ lesson.url | prepend: site.baseurl }}){% endfor %}
{% endif %}
{% endfor %}
