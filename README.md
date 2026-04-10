# Codice sconto vidaXL, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto vidaXL** da [shopilo.it](https://shopilo.it/negozi/vidaxl.it). Restituisce **coupon vidaXL** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-vidaxl](https://shopilo-it.github.io/codice-sconto-vidaxl/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-vidaxl
cd codice-sconto-vidaxl
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "vidaXL",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su mobili e arredamento",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/vidaxl.it"
  }
]
```

## Coupon vidaXL disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su mobili e arredamento | [shopilo.it](https://shopilo.it/negozi/vidaxl.it) |

Codici attivi: **[shopilo.it/negozi/vidaxl.it](https://shopilo.it/negozi/vidaxl.it)**

## Domande frequenti

### Come utilizzo un codice sconto vidaXL?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/vidaxl.it), aggiungi i prodotti al carrello su vidaXL e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon vidaXL?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher vidaXL piu recenti?
La pagina [shopilo.it/negozi/vidaxl.it](https://shopilo.it/negozi/vidaxl.it) viene aggiornata quotidianamente con i codici sconto vidaXL, voucher vidaXL e coupon promozionali vidaXL piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su vidaXL

vidaXL e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/vidaxl.it) trovi i migliori codici sconto vidaXL, coupon vidaXL verificati e voucher vidaXL attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-vidaxl
```

```javascript
const { fetchCoupons } = require('codice-sconto-vidaxl');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
