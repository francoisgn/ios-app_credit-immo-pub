# Crédit Immo · site public

Les pages publiques de **Crédit Immo** (simulateur de crédit immobilier pour iPhone, iPhone Duo et iPad) ont
**déménagé sur francois-g.com** :

| Page | Nouvelle adresse | Ancienne adresse (redirigée) |
|---|---|---|
| Présentation | https://francois-g.com/credit-immo/ | https://francoisgn.github.io/ios-app_credit-immo-pub/ |
| Assistance | https://francois-g.com/credit-immo/assistance/ | https://francoisgn.github.io/ios-app_credit-immo-pub/assistance |
| Confidentialité | https://francois-g.com/credit-immo/confidentialite/ | https://francoisgn.github.io/ios-app_credit-immo-pub/confidentialite |

Les anciennes adresses restent en ligne et redirigent vers les nouvelles : la version 1.0.0 de l'app et la fiche
App Store y renvoient encore. Ce dépôt reste aussi le canal d'assistance (issues).

Une question, un bug, une idée : [ouvrir une issue](https://github.com/francoisgn/ios-app_credit-immo-pub/issues/new/choose).
Une faille de sécurité : voir [SECURITY.md](SECURITY.md), jamais d'issue publique.

## Fonctionnement

Site Jekyll publié par GitHub Pages depuis la branche `master` (racine). Chaque ancienne page (`index.md`,
`assistance.md`, `confidentialite.md`) utilise `_layouts/redirect.html` : redirection immédiate côté navigateur
(`meta refresh`), URL canonique vers la nouvelle page, `noindex`, lien visible. `_layouts/default.html` et
`assets/` ne servent plus qu'à l'historique ; le site lui-même vit dans le dépôt `francoisgn/francois-g.com`.
Le code de l'app est dans un dépôt privé.

Aperçu local : `bundle exec jekyll serve` avec la gem `github-pages`, ou simplement pousser :
Pages reconstruit le site en une minute environ.

Qualité : `pre-commit install` une fois, puis `pre-commit run --all-files` (rejoué par la CI).

## Support

Crédit Immo est gratuite. Pour soutenir son développement : les packs d'icônes dans l'app
(Réglages › Soutenir l'app), ou un café :

[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-francoisgn-FFDD00?logo=buymeacoffee&logoColor=black)](https://buymeacoffee.com/francoisgn)
