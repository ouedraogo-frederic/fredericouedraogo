# Installation sur ton dépôt GitHub

1. Copie tout le contenu de ce dossier à la racine de ton dépôt `ouedraogo-frederic.github.io`
   (écrase l'éventuel `index.md` ou `_config.yml` déjà présents — ce sont les seuls fichiers
   en conflit avec un dépôt Jekyll par défaut).

2. Commit et push :
   ```
   git add .
   git commit -m "Nouvelle identité visuelle du site"
   git push
   ```

3. GitHub Pages reconstruit le site automatiquement (1–2 min). Aucune configuration
   supplémentaire n'est nécessaire : le thème est entièrement personnalisé, pas de
   dépendance à un thème distant.

## À compléter en priorité

- `parcours.md` — dates et intitulés exacts (marqués `[à compléter]`)
- `contact.md` — e-mail, LinkedIn, ORCID
- `publications.md` — tes articles, et les descriptions des programmes FluorAgro /
  Sol AfricO Tox / PPR OM / Physalis&Co
- Remplacer `assets/img/` par une photo si tu veux un portrait en page d'accueil
  (ajoute `<img>` dans `index.md`)

## Ajouter un nouveau billet de blog

Crée un fichier dans `_posts/` nommé `AAAA-MM-JJ-titre-court.md` avec cet en-tête :

```yaml
---
title: "Titre du billet"
date: 2026-09-20
tags: [terrain, résultats]
---

Contenu du billet en Markdown.
```

## Tester en local (facultatif)

```
gem install bundler jekyll
bundle init
echo 'gem "jekyll"' >> Gemfile
echo 'gem "jekyll-feed"' >> Gemfile
bundle install
bundle exec jekyll serve
```

Le site sera visible sur `http://localhost:4000`.
