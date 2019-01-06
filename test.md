---
title: Test Page
layout: chapter
---

# Download Button

To add a button to highlight a download, use the "download include":

- add file to "images" folder
- paste the include code on your markdown page where you want the button to appear
- fill in the title and correct filename values

Download include code:

```{% raw %}
{% include download.html title="Link name" filename="example.pdf" %}
{% endraw %}```

For example, `{% raw %}{% include download.html title="Warmup Find Do Exercise" filename="Week2AND3WarmupFindDoExercise.pdf" %}{% endraw %}` will become:

{% include download.html title="Warmup Find Do Exercise" filename="Week2AND3WarmupFindDoExercise.pdf" %}

# Spotify Embed 

To embed a Spotify item, use the "spotify include":

- View the Spotify song, album, or playlist you want to share
- Right-click on the item and select "Copy Playlist link", which should look something like `https://open.spotify.com/playlist/5Qqq55hpWCPoAXs70Z1TMo`
- Paste the spotify include code on your markdown page where you want the embed to appear
- fill in the `id` as the last part of the Spotify link (should be "type/idnumber"), and add `size="large"` if you want a full sized embed

For example, 

```{% raw %}
{% include spotify.html id="playlist/5Qqq55hpWCPoAXs70Z1TMo" size="large" %}
{% endraw %}```

becomes: 

{% include spotify.html id="playlist/5Qqq55hpWCPoAXs70Z1TMo" size="large" %}

Small example:

```{% raw %}
{% include spotify.html id="playlist/1B2P0PRIzorihMPPyqGGXN" %}
{% endraw %}```

{% include spotify.html id="playlist/1B2P0PRIzorihMPPyqGGXN" %}

# YouTube embed 

To embed a YouTube video, use the "youtube include":

- View the video on YouTube, click the "Share" button
- Copy the link, for example `https://youtu.be/6JQm5aSjX6g`
- Paste youtube include code on your markdown page where you want the embed to appear
- Fill in the `id` with the number found at the end of the share link

For example,

```{% raw %}
{% include youtube.html id="6JQm5aSjX6g" %}
{% endraw %}```

becomes:

{% include youtube.html id="6JQm5aSjX6g" %}
