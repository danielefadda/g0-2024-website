Sei all'interno della pagina `single.markdown` questa pagina è stata creata per visualizzare tutto il contenuto all'interno di una single-page.

**Aggiunta di testo in una colonna**

Il blocco che segue è un testo introduttivo, scritto interamente in _markdown_. Questo testo è stato scritto nel file `introduction.md` ed appare in una colonna stretta (layout: `one-column-sm.html`).


Per caricare il paragrafo all'interno della pagina è necessario fare le seguenti operazioni:
- Creare una variabile in `single.md` che includa il contenuto del file `introduction.md` utilizzando la seguente sintassi:
{% raw %}
```
{% capture introduction_content %}
{% include_relative introduction.md %}
{% endcapture %}
```
{% endraw %}
- Inserire la variabile all'interno del layout `one-column-sm.html`:
{% raw %}
```
{% include one-column-sm.html content=introduction_content %}
```
{% endraw %}
- Inserire lo snippet di codice appena scritto all'interno del file `single.markdown` nel punto della pagina in cui si vuole visualizzare il paragrafo.
- Il layout `one-column-sm.html` è stato creato per visualizzare un solo paragrafo di testo all'interno di una pagina. Questo layout si trova all'interno della cartella `_includes`

---

**Approfondimento sul bottone che apre il modal**

Alla fine del paragrafo introduttivo è presente un bottone che apre un modal. Questo bottone è stato creato utilizzando il componente `modal-component-intro.html` che si trova all'interno della cartella `_includes`.
Per richiamarlo è necessario fare le seguenti operazioni:

- Creare la variabile per includere il contenuto del modal che si trova all'interno di un file```.md```:
{% raw %}
```
{% capture dataset_details %}
{% include_relative dataset-details.md %}
{% endcapture %}
```
{% endraw %}    
- Includere lo snippet di codice seguente all'interno del file `introduction.md`:
{% raw %}
```
{% include modal-component-intro.html title="Dettagli del dataset" content=dataset_details %}
```
{% endraw %}

_N.B. Il modal è stato creato per visualizzare il dettaglio del dataset, ma può essere utilizzato per visualizzare qualsiasi tipo di contenuto. Tuttavia è consigliabile creare un componente modal specifico per ogni tipo di contenuto che si vuole visualizzare. 
In questa maniera sarà più semplice personalizzare il comportamento e la visualizzazione di ogni modal_