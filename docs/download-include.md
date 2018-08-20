# Add a download button with the "download include"

You might want to add a button to highlight a download. 
Use the "download include":

- add the file to "images" folder
- paste the include code on your markdown page where you want the button to appear
- fill in the title and correct filename values

Include code:

```
{% include download.html title="Link name" filename="example.pdf" %}
```

For example, 

- put the file `Week2AND3WarmupFindDoExercise.pdf` in the "images" folder
- the text I want to display in the button is "Warmup Find Do Exercise"
- then the include looks like:

`{% include download.html title="Warmup Find Do Exercise" filename="Week2AND3WarmupFindDoExercise.pdf" %}` 
