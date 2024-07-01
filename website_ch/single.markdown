---
layout: default-full
title:  "Atlante delle stragi nazifasciste"
subtitle: "cronografia della guerra nazista in Italia"
show_sidetoc: true
header_type: hero #base, post, hero,image, splash
header_img: assets/images/Atlante_cover.jpeg
vega: true
---

[//]: # (variables section)
{% capture introduction_content %}
{% include_relative introduction.md %}
{% endcapture %}

{% capture section_1_content %}
{% include_relative section-1.md %}
{% endcapture %}

{% capture timeline_stragi %}
{% include_relative chart-timeline.md %}
{% endcapture %}

{% capture map_stragi %}
{% include_relative chart-map.md %}
{% endcapture %}

{% capture introduction_image %}
{% include_relative introduction-image.md %}
{% endcapture %}

{% capture stragi_all %}
{% include_relative mappa-stragi-intro.md %}
{% endcapture %}

{% capture mappa_stragi %}
{% include_relative mappa-stragi-intro.md %}
{% endcapture %}

{% capture video_content %}
{% include snippets/video.html id="UOQEACobAHk" provider="youtube" video_res="hq2" %}
{% endcapture %}

[//]: # (Include section)
{% include one-column.html content=introduction_content %}

{% include one-column.html content=timeline_stragi %}
<hr>
{% include two-columns.html col-one=introduction_image col-two=section_1_content %}

{% include img-selector.html %}

{% include chart-selector.html %}

{% include one-column.html content=mappa_stragi %}
<hr>


{% include one-column.html content=video_content %}

