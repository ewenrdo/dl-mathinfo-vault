# Math-Lesson-Maker – Générateur pédagogique de documents LaTeX pour les mathématiques

Bienvenue sur **Math-Lesson-Maker** ! Ce projet a pour vocation de faciliter et d’accélérer la création de documents pédagogiques en mathématiques, tout en garantissant une présentation claire, moderne et homogène. Il s’adresse aussi bien aux enseignants qu’aux étudiants ou créateurs de supports, en mettant l’accent sur la lisibilité, la structuration et l’efficacité pédagogique.

> **Disclaimer MATHS-INFO 2** :
> Les étudiants de MATHS-INFO 2 trouveront ici l’ensemble des feuilles de cours de l’année, régulièrement mises à jour.

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
  - Ouvre un terminal puis exécute :
    ```bash
    git clone https://github.com/FunoxPanda/Math-Lesson-Maker.git
    ```
  - Ou utilise l’interface graphique de VSCode :
    - `Ctrl+Shift+P` → “Git: Clone” → colle l’URL du dépôt

3. **Ouvrir le dossier dans VSCode**
  - Menu “Fichier” → “Ouvrir un dossier” → sélectionne le dossier cloné

4. **Compiler un exemple**
  - Ouvre un fichier `.tex` dans `lessons/` ou `exercises/` (par exemple `lessons/sample.tex`)
  - Clique sur “Compiler” (icône LaTeX ou commande `Ctrl+Alt+B` si tu utilises l’extension LaTeX Workshop)

5. **Astuces**
  - Pour ajouter le package à ton document :
    ```latex
    \usepackage{components}
    ```
  - Les dépendances LaTeX nécessaires sont listées dans le fichier `components/components.sty` (voir les `\RequirePackage{...}`)
  - Pour toute question sur LaTeX ou VSCode, consulte la vidéo ou la documentation officielle.

L’environnement est prêt à l’emploi : tu peux modifier, compiler et créer tes propres feuilles de cours ou de TD directement !

---

## Commandes personnalisées disponibles

Voici les principales commandes LaTeX fournies par le package (voir la documentation dans `components/components.sty` et les exemples complets dans `lessons/sample.tex` et `exercises/sample.tex`) :

| Commande                                  | Description                                                          |
| ----------------------------------------- | -------------------------------------------------------------------- |
| `\definition{...}`                        | Encadré pour une **définition**                                      |
| `\theorem{Type}{Titre}{admis ?}{Contenu}` | Encadré pour un **théorème**, une **propriété** ou un **corollaire** |
| `\example{...}`                           | Affiche un **exemple**                                               |
| `\training{...}`                          | Encadré pour une **application** ou un exercice dirigé               |
| `\remark{...}`                            | Met une **remarque importante** en évidence                          |
| `\attention{...}`                         | Signale une **erreur fréquente ou un piège**                         |
| `\illustration{...}`                      | Pour ajouter une **illustration** ou une explication visuelle        |
| `\vocabulary{...}`                        | Présente un **terme de vocabulaire**                                 |
| `\carreaux{n}`                            | Génère une **feuille de petits carreaux** (5x5 mm), de `n` lignes    |
| `\exercise{n}{Titre}{Contenu}`            | Exercice n°`n`, avec son **titre** et son **contenu**               |

Pour des exemples d’utilisation, se référer directement aux fichiers :
- `lessons/sample.tex` pour les feuilles de cours
- `exercises/sample.tex` pour les feuilles de TD

---

---


## Crédits

Ce projet est développé par **Ewen Rodrigues de Oliveira**.
Le design initial des commandes provient de ressources pédagogiques variées qui ont fait leurs preuves dans l’enseignement des mathématiques ainsi que de mon expérience au cours de mes années d'études.

En particulier, je tiens à remercier les sources d'inspiration suivantes :
- Mme Yuen, enseignante agrégée de mathématiques au lycée, pour son approche pédagogique claire et efficace (et la plus grande source d'inspiration pour le projet).
- Les discussions pédagogiques avec M. Alliot, enseignant agrégé de mathématiques au lycée.
- Les documents de cours et de TD utilisés durant mes études à l'université.