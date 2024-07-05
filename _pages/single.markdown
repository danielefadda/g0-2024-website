---
layout: default-full
title:  "Atlante delle stragi nazifasciste"
subtitle: "cronografia della guerra nazista in Italia"
show_sidetoc: true
header_type: hero #base, post, hero,image, splash
header_img: assets/images/Atlante_cover.jpeg
header_title: "Atlante delle stragi nazifasciste"
vega: true
---

[//]: # (variables section)
{% capture introduction_content %}
{% include_relative snippets/introduction.md %}
{% endcapture %}

{% capture section_1_content %}
{% include_relative snippets/section-1.md %}
{% endcapture %}

{% capture timeline_stragi %}
{% include_relative snippets/chart-timeline.md %}
{% endcapture %}

{% capture map_stragi %}
{% include_relative snippets/chart-map.md %}
{% endcapture %}

{% capture introduction_image %}
{% include_relative snippets/gallery-images.md %}
{% endcapture %}

{% capture stragi_all %}
{% include_relative snippets/mappa-stragi-intro.md %}
{% endcapture %}

{% capture mappa_stragi %}
{% include_relative snippets/mappa-stragi-intro.md %}
{% endcapture %}

{% capture video_content %}
{% include snippets/video.html id="UOQEACobAHk" provider="youtube" video_res="hq2" %}
{% endcapture %}

[//]: # (Include section)
{% capture introduction_tech %}
{% include_relative snippets/introduction-tech.md %}
{% endcapture %}

<div class="tech" style="display: none">
  {% include one-column-sm.html content=introduction_tech %}
</div>

{% include one-column-sm.html content=introduction_content %}

{% include one-column-sm.html content=timeline_stragi %}
<hr>

{% capture tech_section1 %}
{% include_relative snippets/section1-tech.md %}
{% endcapture %}

<div class="tech" style="display: none">
  {% include one-column-sm.html content=tech_section1 %}
</div>

{% include two-columns.html col-one=introduction_image col-two=section_1_content %}
<hr>
{% include one-column-cards.html width='40%' datasource=site.data.img-selector url ='url' name='name' description='description' %}
{% include img-selector.html %}

{% include chart-selector.html %}

{% include big-numbers.html %}
<hr>
{% include one-column-sm.html content=mappa_stragi %}
<hr>


{% include one-column-sm.html content=video_content %}

{% include code-explanation.html %}