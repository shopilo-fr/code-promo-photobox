# Code promo Photobox, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Photobox** depuis [shopilo.fr](https://shopilo.fr/reductions/photobox.fr). Renvoie les **coupons Photobox** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-photobox](https://shopilo-fr.github.io/code-promo-photobox/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-photobox
cd code-promo-photobox
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Photobox",
    "code": "SHOPILO25",
    "discount": "25%",
    "description": "25% de reduction sur les livres photo et tirages",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/photobox.fr"
  }
]
```

## Coupons Photobox disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 25% | 25% de reduction sur les livres photo et tirages | [shopilo.fr](https://shopilo.fr/reductions/photobox.fr) |

Codes actifs : **[shopilo.fr/reductions/photobox.fr](https://shopilo.fr/reductions/photobox.fr)**

## Questions frequentes

### Comment utiliser un code promo Photobox ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/photobox.fr), ajoutez les produits a votre panier sur Photobox et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Photobox ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Photobox les plus recents ?
La page [shopilo.fr/reductions/photobox.fr](https://shopilo.fr/reductions/photobox.fr) est mise a jour quotidiennement avec les codes promo Photobox, bons de reduction Photobox et coupons promotionnels Photobox les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Photobox

Photobox est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/photobox.fr), retrouvez les meilleurs codes promo Photobox, coupons Photobox verifies et bons de reduction Photobox actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-photobox
```

```javascript
const { fetchCoupons } = require('code-promo-photobox');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
