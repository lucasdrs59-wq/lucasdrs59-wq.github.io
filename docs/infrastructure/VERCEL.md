# Vercel

## Rôle actuel

Vercel fournit un miroir de production et une preview isolée pour chaque pull
request. GitHub Pages reste l'adresse publique canonique du portfolio.

## Configuration de référence

- dépôt : `lucasdrs59-wq/lucasdrs59-wq.github.io` ;
- branche de production : `main` ;
- framework : Next.js ;
- version Node.js : `22.x`, imposée par `package.json` ;
- répertoire racine : racine du dépôt ;
- variables d'environnement : aucune ;
- commande de validation locale : `npm run verify`.

Après l’unification, le projet Vercel doit être reconnecté à ce dépôt avant la
suppression de l’ancien dépôt `portfolio-v2`.

## Politique d'exploitation

- une PR crée une preview, jamais un environnement de données durable ;
- une fusion sur `main` crée le miroir de production ;
- les déploiements issus de branches fermées sont historiques et ne sont pas
  considérés comme des environnements actifs ;
- aucun secret de production n'est exposé aux previews non approuvées ;
- un domaine personnalisé, s'il est ajouté, est documenté avant bascule DNS.

## Contrôle avant mise en production

1. CI GitHub verte.
2. `npm run verify` réussi avec Node 22.
3. Preview contrôlée sur ordinateur et mobile.
4. Aucun secret ou contenu confidentiel dans l'export.
5. Production Vercel sans erreur de build ni erreur d'exécution.
