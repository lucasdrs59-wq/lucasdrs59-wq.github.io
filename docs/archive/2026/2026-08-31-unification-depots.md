# Unification des dépôts du portfolio

## Décision

Le code source Next.js, la documentation et la publication GitHub Pages sont
regroupés dans `lucasdrs59-wq/lucasdrs59-wq.github.io`.

## Origine

- ancien dépôt source : `lucasdrs59-wq/portfolio-v2` ;
- dernière révision reprise : `03b4fd3fe593ffbdcc52b5e7430055790d7ee4a1` ;
- ancien dépôt de publication : `lucasdrs59-wq/lucasdrs59-wq.github.io` ;
- état avant migration : `archive/pre-unification-2026-08-31`.

## Nouveau fonctionnement

1. Les changements sont proposés par pull request dans le dépôt unique.
2. La CI valide lint, TypeScript et build Next.js.
3. Après fusion dans `main`, l’export `out/` est envoyé à GitHub Pages.
4. Les fichiers compilés ne sont plus versionnés manuellement.

Le dépôt `portfolio-v2` ne doit plus recevoir de changement après la migration.
