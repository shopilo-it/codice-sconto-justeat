# Codice sconto Just Eat, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Just Eat** da [shopilo.it](https://shopilo.it/negozi/justeat.it). Restituisce **coupon Just Eat** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-justeat](https://shopilo-it.github.io/codice-sconto-justeat/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-justeat
cd codice-sconto-justeat
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Just Eat",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto sulla prima consegna a domicilio",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/justeat.it"
  }
]
```

## Coupon Just Eat disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto sulla prima consegna a domicilio | [shopilo.it](https://shopilo.it/negozi/justeat.it) |

Codici attivi: **[shopilo.it/negozi/justeat.it](https://shopilo.it/negozi/justeat.it)**

## Domande frequenti

### Come utilizzo un codice sconto Just Eat?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/justeat.it), aggiungi i prodotti al carrello su Just Eat e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Just Eat?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Just Eat piu recenti?
La pagina [shopilo.it/negozi/justeat.it](https://shopilo.it/negozi/justeat.it) viene aggiornata quotidianamente con i codici sconto Just Eat, voucher Just Eat e coupon promozionali Just Eat piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Just Eat

Just Eat e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/justeat.it) trovi i migliori codici sconto Just Eat, coupon Just Eat verificati e voucher Just Eat attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-justeat
```

```javascript
const { fetchCoupons } = require('codice-sconto-justeat');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
