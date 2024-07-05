# Mappa delle stragi

L’elaborazione su base geografica dell’insieme dei dati.
La mappa mostra le stragi suddivise per matrice politica e luogo dell'evento.
La dimensione dei cerchi è proporzionale al numero di vittime.

{% capture mappa_stragi %}
{% include_relative snippets/mappa-stragi.md %}
{% endcapture %}

{% include modal-component-mappa.html title="Mappa delle stragi in Italia" content=mappa_stragi %}