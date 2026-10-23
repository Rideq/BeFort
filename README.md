# Rideq

Hub degli strumenti di Luca, Daniele e Matteo: app, simulatori e mappe che trasformano dati complessi in strumenti semplici da usare.

Sito: https://rideq.github.io/BeFort/

## Struttura

Il sito è un'unica pagina statica, `index.html` (HTML, CSS e JavaScript inline), pubblicata con GitHub Pages.

## Aggiungere o modificare uno strumento

Modifica l'array `LINKS` nello `<script>` in fondo a `index.html`:

```js
{id:'mio-tool', title:'Nome', url:'https://rideq.github.io/MioTool/', desc:'Descrizione breve.', category:'Categoria', icon:'🔧'}
```

I filtri per categoria si generano automaticamente. Per mettere uno strumento "In primo piano", modifica il blocco `featured-card` nell'HTML.

## Statistiche visite

Le visite sono contate con [GoatCounter](https://www.goatcounter.com) (senza cookie, nessun banner necessario). La dashboard è privata: https://rideq.goatcounter.com (serve il login).

- Visite alla pagina: conteggiate automaticamente.
- Click sugli strumenti: compaiono come eventi `click/<id>` (l'`id` è quello in `LINKS`).

Il codice dell'account (`rideq`) è nello script in fondo a `index.html`. Per contare anche le visite delle singole app, aggiungi la stessa riga nel loro `index.html`:

```html
<script data-goatcounter="https://rideq.goatcounter.com/count" async src="https://gc.zgo.at/count.js"></script>
```
