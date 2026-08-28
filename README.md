# dl-mathinfo-vault

Ce dépôt centralise mes cours et exercices de mathématiques et d'informatique à l'UniversitéParis Cité.

> [!NOTE]
> Si votre objectif est simplement de consulter les cours et les documents finalisés, il est fortement recommandé de vous rendre directement sur le site [ewenrdo.fr](https://ewenrdo.fr/ressources).

---

## Utilisation des documents et licences

Certains documents présents dans ce dépôt sont soumis à des restrictions d'utilisation. Il convient de vérifier systématiquement les conditions applicables sur [ewenrdo.fr/ressources](https://ewenrdo.fr/ressources) avant toute réutilisation.

---

## Architecture et module requis (components)

L'arborescence du projet s'appuie sur un package de style partagé (`mathtex-maker`) qui gère la mise en forme des documents LaTeX. Vous pouvez consulter le code source de ce package sur [GitHub](https://github.com/ewenrdo/mathtex-maker). Il est nécessaire d'installer ce package pour compiler correctement les documents du projet.

Pour éviter les duplications et centraliser la maintenance, ce package est intégré au projet sous forme de **sous-module Git** situé à la racine dans le dossier `components/`. Cela permet de lier le dépôt principal à une version précise et indépendante du code de mise en page, tout en garantissant que les fichiers `.tex` (peu importe leur profondeur dans les sous-dossiers) pointent de manière cohérente vers ce même répertoire source.

---

# Contribuer

Les contributions pour corriger une coquille, améliorer un exercice ou proposer une modification sont les bienvenues. Voici la marche à suivre pour proposer un changement :

1. **Créer une branche :** Partez d'une nouvelle branche dédiée à votre modification à partir de `main`.
2. **Modifier le fichier :** Apportez vos corrections directement dans le fichier `.tex` concerné.
3. **Tester la compilation :** Assurez-vous que votre document compile correctement en local en vous plaçant dans son dossier de travail et en veillant à ce que les chemins relatifs pointent bien vers le dossier `components/` à la racine.
4. **Proposer une Pull Request :** Soumettez votre contribution en ouvrant une Pull Request sur le dépôt pour relecture.

**Attention :** S'il vous plait, n'envoyez pas les documents modifiés compilés (PDF) mais uniquement les fichiers `.tex` et les éventuels fichiers de ressources (images, etc.) nécessaires à la compilation dans votre Pull Request. Cela permet de garder le dépôt léger et de faciliter la maintenance.

---

# Contributeurs

Ce projet a bénéficié des contributions des personnes suivantes :

* **Ewen Rodrigues de Oliveira** - Créateur et mainteneur principal, à l'origine de l'écriture initiale des cours et de la mise en place de l'architecture du projet.
* **Laurent Cai** - Contribue régulièrement à la relecture des cours et à l'ajout des preuves des propositions et théorèmes.

> [!WARNING]
> De manière ponctuelle, de l'intelligence artificielle _(via Copilot)_ est utilisée pour écrire plus rapidement certaines parties du cours lorsque je suis en amphithéâtre. Ces parties sont **systématiquement relues et corrigées** directement pour garantir la qualité du contenu.

Les contributions sous forme de propositions de modification ou de correction de coquilles via des Pull Requests sont également enregistrées directement dans l'historique des commits du dépôt.