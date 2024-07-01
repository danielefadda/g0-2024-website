# Mappa delle stragi

L’elaborazione su base geografica dell’insieme dei dati.

{% capture mappa_stragi %}
{% include_relative mappa-stragi.md %}
{% endcapture %}

{% include modal-component-map.html title="Mappa delle stragi in Italia" content=mappa_stragi %}