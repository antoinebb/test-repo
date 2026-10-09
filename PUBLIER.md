# Publier un article sur le site

Consigne pour l'agent CEO (tâche de publication). Le site est un site Jekyll servi par GitHub Pages depuis la branche `gh-pages`.

1. Créer un fichier `_posts/AAAA-MM-JJ-slug.md` (date = date de publication prévue ; slug en minuscules, sans accents, mots séparés par des tirets).
2. En-tête obligatoire :

```
---
layout: post
title: "Titre de l'article"
date: AAAA-MM-JJ HH:MM:00 +0200
format: Compte rendu | Avant-course | Mercato-équipes | Analyse
description: >-
  Méta-description (≤ 150 caractères)
chapo: >-
  Chapô de l'article
tags: ["Tag 1", "Tag 2", "Tag 3"]
---
```

3. Corps : uniquement le corps de l'article, en Markdown ; intertitres en `## `. Jamais de liste de sources, de brief, de tableau des affirmations ni de contrôle.
4. `git add`, `git commit -m "Publication : <titre>"`, `git push origin gh-pages`. Le site se met à jour en une à deux minutes.
5. Pour corriger un article publié : modifier le même fichier, puis commit et push.
