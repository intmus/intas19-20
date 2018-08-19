---
title: Test Page
layout: chapter
---

You might want to add a button to highlight a download. 
Use the "download include":

- add file to "images" folder
- paste the include code on your markdown page where you want the button to appear
- fill in the title and correct filename values

Include code:

```{% raw %}
{% include download.html title="Link name" filename="example.pdf" %}
{% endraw %}```

For example, `{% raw %}{% include download.html title="Warmup Find Do Exercise" filename="Week2AND3WarmupFindDoExercise.pdf" %}{% endraw %}` will become:

{% include download.html title="Warmup Find Do Exercise" filename="Week2AND3WarmupFindDoExercise.pdf" %}
