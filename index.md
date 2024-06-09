---
layout: default
title: "Home"
---

<h2>Videos</h2>
<div class="videos">
    {% for video in site.videos %}
        <div class="video">
            <h3><a href="{{ video.url | relative_url }}">{{ video.title }}</a></h3>
            <iframe width="560" height="315" src="https://img.youtube.com/vi/{{ video.youtube_video_url }}/mqdefault.jpg" frameborder="0" allowfullscreen></iframe>
        </div>
    {% endfor %}
</div>
