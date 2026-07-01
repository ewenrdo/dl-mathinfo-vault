# Getting Started

## Installation et prise en main rapide

1. **Installer VSCode et LaTeX (et son environnement)**
  - Suivre la vidéo d'installation et de configuration de VSCode : [https://www.youtube.com/watch?v=4lyHIQl4VM8](https://www.youtube.com/watch?v=4lyHIQl4VM8)

2. **Cloner le dépôt**
  - Ouvrez un terminal puis exécutez :
    ```bash
    git clone https://github.com/FunoxPanda/Math-Lesson-Maker.git
    ```
  - Ou utilisez l'interface graphique de VSCode :
    - `Ctrl+Shift+P` → “Git: Clone” → collez l'URL du dépôt

3. **Ouvrir le dossier dans VSCode**
  - Menu “Fichier” → “Ouvrir un dossier” → sélectionne le dossier cloné

4. **Compiler un exemple**
  - Ouvrez un fichier `.tex` dans `lessons/` ou `exercises/` (par exemple `lessons/sample.tex`)
  - Cliquez sur “Compiler” (icône LaTeX ou commande `Ctrl+Alt+B` si vous utilisez l'extension LaTeX Workshop)

5. **Astuces**
  - Pour ajouter le package à votre document :
    ```latex
    \usepackage{components}
    ```
  - Les dépendances LaTeX nécessaires sont listées dans le fichier `components/components.sty` (voir les `\RequirePackage{...}`)
  - Pour toute question sur LaTeX ou VSCode, consultez la vidéo ou la documentation officielle.

L'environnement est prêt à l'emploi pour la création de fiches d'exercices et de cours en mathématiques. _(sans doute les commandes sont utilisables pour d'autres matières)_

---

## Commandes personnalisées disponibles

Le fichier `components/components.sty` contient toutes les commandes personnalisées. Un aperçu des commandes ajoutées par le package est disponible dans `lessons/sample.tex`.
