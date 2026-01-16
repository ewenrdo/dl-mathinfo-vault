# Math-Lesson-Maker – Package LaTeX pour polycopiés mathématiques

Bienvenue sur **Math-Lesson-Maker** ! Ce projet a pour vocation de faciliter et d’accélérer la création de documents pédagogiques en mathématiques, tout en garantissant une présentation claire, moderne et homogène. 

> **Disclaimer L2 MATH / MATHS-INFO 2** :
> Les étudiants de L2 MATH / MATHS-INFO 2 trouveront ici l’ensemble des feuilles de cours de l’année de mathématiques, régulièrement mises à jour.
> Je conseille vivement de consulter [ce site web](https://ewenrdo.fr/ressources) pour accéder à ces ressources, qui y sont rangées de manière plus structurée.

L’objectif est de proposer un cadre unifié pour la rédaction de feuilles de TD et de cours, avec des outils LaTeX personnalisés pour illustrer, expliquer, et valoriser les contenus mathématiques. L’accent est mis sur la pédagogie : chaque commande vise à rendre les notions plus accessibles, à structurer les démonstrations, et à encourager la compréhension active.

---

## Deux types de documents générés

Le projet permet de générer deux types de documents distincts :

- **Feuille de TD** (exercices, travaux dirigés, sujets d’entraînement) : voir les exemples dans `exercises/sample.tex`.
- **Feuille de cours** (supports de cours structurés, définitions, théorèmes, illustrations) : voir les exemples dans `lessons/sample.tex`.

Chaque type dispose de ses propres modèles et commandes adaptées, pour répondre aux besoins spécifiques de la pédagogie mathématique.


## 📁 Arborescence du projet

```
/components/
  └── components.sty       % Le package LaTeX principal

/images/                   % Éventuelles illustrations utilisées dans les leçons

/sample.tex                  % Un fichier d'exemple appliquant tous les composants

/lessons/                  % Tes leçons de mathématiques utilisant ce package
  └── sample.tex           % Document-type

/exercises/                % Tes leçons de mathématiques utilisant ce package
  └── sample.tex           % Document-type
```

---

## Installation et prise en main rapide

1. **Installer VSCode et LaTeX (et son environnement)**
  - Suivre la vidéo d’installation et de configuration de VSCode : [https://www.youtube.com/watch?v=4lyHIQl4VM8](https://www.youtube.com/watch?v=4lyHIQl4VM8)

2. **Cloner le dépôt**
  - Ouvrez un terminal puis exécutez :
    ```bash
    git clone https://github.com/FunoxPanda/Math-Lesson-Maker.git
    ```
  - Ou utilisez l’interface graphique de VSCode :
    - `Ctrl+Shift+P` → “Git: Clone” → collez l’URL du dépôt

3. **Ouvrir le dossier dans VSCode**
  - Menu “Fichier” → “Ouvrir un dossier” → sélectionne le dossier cloné

4. **Compiler un exemple**
  - Ouvrez un fichier `.tex` dans `lessons/` ou `exercises/` (par exemple `lessons/sample.tex`)
  - Cliquez sur “Compiler” (icône LaTeX ou commande `Ctrl+Alt+B` si vous utilisez l’extension LaTeX Workshop)

5. **Astuces**
  - Pour ajouter le package à votre document :
    ```latex
    \usepackage{components}
    ```
  - Les dépendances LaTeX nécessaires sont listées dans le fichier `components/components.sty` (voir les `\RequirePackage{...}`)
  - Pour toute question sur LaTeX ou VSCode, consultez la vidéo ou la documentation officielle.

L’environnement est prêt à l’emploi pour la création de fiches d'exercices et de cours en mathématiques. _(sans doute les commandes sont utilisables pour d’autres matières)_

---

## Commandes personnalisées disponibles

Le fichier `components/components.sty` contient toutes les commandes personnalisées. Un aperçu des commandes ajoutées par le package est disponible dans `lessons/sample.tex`.

---

## Crédits

Le design principal de ce projet est directement inspiré des travaux de Mme Yuen et M. Alliot (version initiale), enseignants agrégés de mathématiques au lycée. Les choix de présentation, de structuration et de style des commandes LaTeX reprennent largement leurs pratiques pédagogiques, qui ont fait leurs preuves auprès des étudiants.

Un grand remerciement à Mme Yuen et M. Alliot pour leur générosité, leur exigence et la qualité de leur enseignement, qui ont servi de fondation à ce projet et à mes connaissances en mathématiques.

Le projet a vocation à évoluer pour intégrer les avancées récentes et améliorer continuellement son contenu pédagogique. Tant que le design reste fidèle à l’esprit et à la structure des documents de ces enseignants, l’utilisation de ce projet doit rester strictement personnelle (usage individuel, non public, non commercial).

Si des modifications substantielles éloignent le projet des modèles d’origine, une réévaluation des conditions d’utilisation sera nécessaire.

**Attention :** Le contenu (plan du cours) du dossier `lessons/dl2_lmath_info` est tous droits réservés à l'Université Paris Cité ([u-pariscite.fr](https://u-pariscite.fr)). Toute réutilisation ou diffusion de ce contenu est strictement interdite sans l'accord de l'université. Il arrive que je modifie le cours pour le rendre plus clair, mais le fond reste le même. Merci de respecter cette condition.
**UPDATE 16/01/2026 :** Dorénavant, les crédits seront mentionnés sur [ewenrdo.fr/ressources](https://ewenrdo.fr/ressources) pour une meilleure visibilité et accessibilité. Le lecteur est invité à s'y référer pour toute question relative aux droits d'utilisation.