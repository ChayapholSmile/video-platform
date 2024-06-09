---
layout: default
title: "Home"
---

<h2>Videos</h2>
<div class="videos">
    {% for video in site.videos %}
        <div class="video">
            <h3><a href="{{ video.url | relative_url }}">{{ video.title }}</a></h3>
<img src="https://img.youtube.com/vi/{{ video.youtube_video_url }}/mqdefault.jpg" alt="" width="560" height="318">
        </div>
    {% endfor %}
</div>
