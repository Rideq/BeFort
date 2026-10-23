# Befort

Hub degli strumenti di Luca e Daniele: app, simulatori e mappe che trasformano dati complessi in strumenti semplici da usare.

Sito: https://rideq.github.io/BeFort/

## Struttura

Il sito è un'unica pagina statica, `index.html` (HTML, CSS e JavaScript inline), pubblicata con GitHub Pages.

## Aggiungere o modificare uno strumento

Modifica l'array `LINKS` nello `<script>` in fondo a `index.html`:

```js
{id:'mio-tool', title:'Nome', url:'https://rideq.github.io/MioTool/', desc:'Descrizione breve.', category:'Categoria', icon:'🔧'}
```

I filtri per categoria si generano automaticamente. Per mettere uno strumento "In primo piano", modifica il blocco `featured-card` nell'HTML.
