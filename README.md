# Math Lesson Maker

Ce dépôt centralise les cours et exercices de mathématiques.

> [!NOTE]
> Si votre objectif est simplement de consulter les cours et les documents finalisés, il est fortement recommandé de vous rendre directement sur le site [ewenrdo.fr](https://ewenrdo.fr/ressources).

---

## Utilisation des documents et licences

Certains documents présents dans ce dépôt sont soumis à des restrictions d'utilisation. Il convient de vérifier systématiquement les conditions applicables sur [ewenrdo.fr/ressources](https://ewenrdo.fr/ressources) avant toute réutilisation.

---

## Architecture et module requis (components)

L'arborescence du projet s'appuie sur un package de style partagé (`mathtex-maker`) qui gère la mise en forme des documents LaTeX. Vous pouvez consulter le code source de ce package sur [GitHub](https://github.com/ewenrdo/mathtex-maker). Il est nécessaire d'installer ce package pour compiler correctement les documents du projet.

Pour éviter les duplications et centraliser la maintenance, ce package est intégré au projet sous forme de **sous-module Git** situé à la racine dans le dossier `components/`. Cela permet de lier le dépôt principal à une version précise et indépendante du code de mise en page, tout en garantissant que les fichiers `.tex` (peu importe leur profondeur dans les sous-dossiers) pointent de manière cohérente vers ce même répertoire source.