---
title: Photos
layout: default
image_width: 160
image_height: 120
images:
- /files/photos/(1).jpg
- /files/photos/(2).jpg
- /files/photos/(3).jpg
- /files/photos/(4).jpg
- /files/photos/(5).jpg
- /files/photos/(6).jpg
- /files/photos/(7).jpg
- /files/photos/(8).jpg
- /files/photos/(9).jpg
- /files/photos/(10).jpg
- /files/photos/(11).jpg
- /files/photos/(12).jpg
- /files/photos/(13).jpg
- /files/photos/(14).jpg
- /files/photos/(15).jpg
- /files/photos/(16).jpg
- /files/photos/(17).jpg
- /files/photos/(18).jpg
---
<div id="gallery">
    {% for image in page.images %}
    {% capture img_url %}//i{% cycle '0', '1', '2' %}.wp.com/{{site.domain}}{{image}}{% endcapture %}
    <a class="fancybox" rel="gallery" href="{{img_url}}">
        <img src="{{img_url}}?resize={{page.image_width}},{{page.image_height}}" alt="" style="height:{{page.image_height}}px" />
    </a>
    {% endfor %}
</div>