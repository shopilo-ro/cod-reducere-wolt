# Cod reducere Wolt — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Wolt** de pe [shopilo.ro](https://shopilo.ro/magazin/wolt.com). Returneaza **cupoane Wolt** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-wolt](https://shopilo-ro.github.io/cod-reducere-wolt/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-wolt
cd cod-reducere-wolt
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Wolt",
    "code": "SHOPILO20",
    "discount": "20 lei",
    "description": "20 lei reducere la prima comanda Wolt",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/wolt.com"
  }
]
```

## Cupoane Wolt disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 20 lei | 20 lei reducere la prima comanda Wolt | [shopilo.ro](https://shopilo.ro/magazin/wolt.com) |

Codurile active: **[shopilo.ro/magazin/wolt.com](https://shopilo.ro/magazin/wolt.com)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Wolt?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/wolt.com), adauga produsele in cos pe Wolt, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Wolt?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Wolt?
Pagina [shopilo.ro/magazin/wolt.com](https://shopilo.ro/magazin/wolt.com) este actualizata zilnic cu cele mai noi cod reducere Wolt, voucher Wolt si cupon promotional Wolt.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Wolt

Wolt este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/wolt.com) cele mai bune cod reducere Wolt, cupoane Wolt verificate si voucher Wolt active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-wolt
```

```javascript
const { fetchCoupons } = require('cod-reducere-wolt');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
