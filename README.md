# Crédit Immo · site public

Site public de **Crédit Immo**, simulateur de crédit immobilier pour iPhone, iPhone Duo et iPad :
présentation, assistance et politique de confidentialité, référencées par la fiche App Store.

| Page | Adresse |
|---|---|
| Accueil | https://francoisgn.github.io/ios-app_credit-immo-pub/ |
| Assistance | https://francoisgn.github.io/ios-app_credit-immo-pub/assistance |
| Confidentialité | https://francoisgn.github.io/ios-app_credit-immo-pub/confidentialite |

Une question, un bug, une idée : [ouvrir une issue](https://github.com/francoisgn/ios-app_credit-immo-pub/issues/new/choose).
Une faille de sécurité : voir [SECURITY.md](SECURITY.md), jamais d'issue publique.

## Fonctionnement

Site Jekyll publié par GitHub Pages depuis la branche `master` (racine), sans thème externe :
`_layouts/default.html`, `assets/style.css` (clair et sombre), une page Markdown par adresse.
Le code de l'app est dans un dépôt privé.

Aperçu local : `bundle exec jekyll serve` avec la gem `github-pages`, ou simplement pousser :
Pages reconstruit le site en une minute environ.

Qualité : `pre-commit install` une fois, puis `pre-commit run --all-files` (rejoué par la CI).

## Support

Crédit Immo est gratuite. Pour soutenir son développement : les packs d'icônes dans l'app
(Réglages › Soutenir l'app), ou un café :

[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-francoisgn-FFDD00?logo=buymeacoffee&logoColor=black)](https://buymeacoffee.com/francoisgn)
