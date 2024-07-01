---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title:  "Atlante delle stragi nazifasciste"
subtitle: "cronografia della guerra nazista in Italia"
show_sidetoc: true
header_type: splash
header_img: assets/images/Atlante_cover.jpeg
vega: true
h_min: 1
---


# L'Atlante delle stragi nazifasciste

L’Atlante delle stragi naziste e fasciste si compone di una banca dati e dei materiali di corredo (documentari, iconografici, video) correlati agli episodi censiti, ospitati all’interno del sito web. 

Nella banca dati sono state catalogate e analizzate tutte le stragi e le uccisioni singole di civili e partigiani uccisi al di fuori dello scontro armato, commesse da reparti tedeschi e della Repubblica Sociale Italiana in Italia dopo l’8 settembre 1943, a partire dalle prime uccisioni nel Meridione fino alle stragi della ritirata eseguite in Piemonte, Lombardia, Veneto e Trentino Alto Adige nei giorni successivi alla liberazione.

L’elaborazione su base cronologica e geografica dell’insieme dei dati censiti ha consentito la definizione di una ‘cronografia della guerra nazista in Italia’, che mette in correlazione modalità, autori, tempi e luoghi della violenza contro gli inermi sul territorio nazionale.

[Button name](#this-is-the-main-title){: .btn .btn-primary .btn-sm  }

<vegachart schema-url="{{ site.baseurl }}/assets/charts/stragi.json" style="width: 100%"></vegachart>

# This is the main title
{: toc}
This is the homepage of the website. You can add content and custom Front Matter to this file. To modify the layout, see [Jekyll's documentation](https://jekyllrb.com/docs/themes/#overriding-theme-defaults).

A long long paragraph, wiht some **bold** and *italic* text. And a [link](https://dieghernan.github.io/chulapa/). 
And a list:
- item 1
  - detail 1
- item 2
- item 3
  - detail 3
  - detail 4
- item 4


<h2 id="aa">My heading</h2>
With a description of the second title.

<i class="fas fa-exclamation-circle"></i> For an icon, you just insert the html code

---
## 2.1 A new title h2
wiht a long block of text, fake text, like Lorem Ipsum, dolor sit amet, consectetur adipiscing elit sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
## 2.2 A second title h2
button:
  text: "Click me"
  url: "https://dieghernan.github.io/chulapa/"
  style: "primary"
  size: "lg"
  icon: "fas fa-arrow-right"
  icon_position: "right"
  target: "_blank"
### 2.3 A first subtitle h3
Some text that justify the existence of this subtitle. I want to write a very long paragraph that describes nothing, and that is not useful at all. But I need to fill this space with some text. So, here it is. I hope you enjoy it.
{% include snippets/video.html id="1hXYuWTWVww" provider="youtube" %}





## 3. An image gallery

{% assign externalgallery = "
https://picsum.photos/seed/10/600/1200,
https://picsum.photos/seed/20/800/500,
https://picsum.photos/seed/30/900/1200,
https://picsum.photos/seed/40/900/1300,
https://picsum.photos/seed/50/750/325,
https://picsum.photos/seed/60/600,
https://picsum.photos/seed/70/700/500" %}

{% include_cached snippets/masonry.html external=externalgallery %}
