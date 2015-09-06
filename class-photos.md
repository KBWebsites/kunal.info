---
title: Class Photos
layout: default
classes: [1, 3, 4]
---
{% for i in page.classes %}
## Class {{ i }}
<a rel="gallery" href="/files/class-photos/class-{{ i }}.jpg" class="fancybox">
    <img src="/files/class-photos/class-{{ i }}.jpg" alt="Class {{ i }}">
</a>
{% endfor %}