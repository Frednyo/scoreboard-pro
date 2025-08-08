# Scoreboard Pro - Déploiement GitHub Pages

Ce dépôt contient une petite application HTML/CSS/JS (fichier `index.html`) — un scoreboard stylé pour gérer un match multijoueurs.

## Contenu
- `index.html` : l'application complète (frontend uniquement).

## Déployer sur GitHub Pages (méthode simple - interface web)
1. Crée un nouveau dépôt sur GitHub (nom au choix, par exemple `scoreboard-pro`).
2. Ajoute `index.html` à la racine du dépôt (upload via l'interface web).
3. Dans les *Settings* du dépôt → *Pages* → sélectionne la branche `main` (ou `master`) et le dossier `/ (root)`.
4. Enregistre. Après quelques secondes, ton site sera disponible à l'adresse `https://<ton-utilisateur>.github.io/<nom-du-repo>/`.

## Déployer avec git en local (ligne de commande)
```bash
# depuis le dossier contenant index.html
git init
git add index.html
git commit -m "Initial commit - Scoreboard Pro"
# remplace <user> et <repo> par tes infos
git remote add origin https://github.com/<user>/<repo>.git
git branch -M main
git push -u origin main
```
Puis active GitHub Pages dans les Settings (branch `main`, dossier `/ (root)`).

## Déployer automatiquement (gh CLI)
Si tu as l'outil `gh` :
```bash
gh repo create <user>/<repo> --public --source=. --push
# puis active pages si nécessaire via l'interface ou via gh api
```

## Remarques
- Le site est entièrement statique : pas besoin de backend.
- Tu peux personnaliser `index.html` (couleurs, textes).
- Si tu veux, je peux générer automatiquement la repo & la publier — mais j'aurai besoin d'accès à ton compte GitHub (et tu dois me le fournir ou faire la procédure toi-même). Par sécurité, je ne peux pas pousser sur ton compte sans autorisation explicite et un moyen d'accès.

Bonne mise en ligne — dis-moi si tu veux que je prépare un README en français plus joli, un logo, ou une version avec favicon + meta tags pour partage social.
