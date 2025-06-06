# 📚 `Math-Lesson-Latex` – Un package LaTeX pour écrire des cours de maths plus vite

Bienvenue sur le repo de **Math-Lesson-Latex**, un package LaTeX personnel conçu pour faciliter, accélérer et standardiser la rédaction de cours de mathématiques. Il fournit des commandes prêtes à l’emploi pour les définitions, théorèmes, exemples, applications, remarques, illustrations, vocabulaires, et plus encore — dans un style moderne et coloré.

## 🌟 Objectif

Ce package permet :

* d’unifier la présentation des contenus mathématiques ;
* d’accélérer la rédaction de cours (particulièrement utiles pour enseignants, étudiants, ou créateurs de fiches) ;
* d’améliorer la lisibilité et l’impact visuel grâce à l’usage de couleurs, d’icônes, et de boîtes stylisées.

---

## 📁 Arborescence du projet

```
/components/
  └── components.sty       % Le package LaTeX principal

/images/                   % Éventuelles illustrations utilisées dans les leçons

/main.tex                  % Un fichier d'exemple appliquant tous les composants

/lessons/                  % Tes leçons de mathématiques utilisant ce package
```

---

## 🚀 Installation

Clone le repo, et amuse toi, l'environnement est déjà prêt à être utilisé.

```bash
git clone https://github.com/ton-utilisateur/components-maths.git
```

Dans ton fichier `.tex`, ajoute simplement :

```latex
\usepackage{components}
```

⚠️ Ce package nécessite les extensions suivantes :

* `xcolor`
* `tcolorbox`
* `ifthen`
* `amsmath`, `amssymb`, `amsfonts`
* `fontawesome5`
* `tikz`
* `sectsty`
* `uarial`, `helvet`

---

## 🛠️ Fonctionnalités

Voici les commandes personnalisées disponibles :

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

---

## 🧪 Exemple minimal (`main.tex`)

```latex
\documentclass{article}
\usepackage{components}

\begin{document}

\docTitle{Exemple de cours}

\definition{Une fonction est dite continue si...}

\theorem{Théorème}{Théorème fondamental}{false}{
  Soit $f$ continue sur un intervalle $I$...
}

\example{Soit $f(x) = x^2$. On a...}

\training{Résoudre l'équation $f(x) = 4$.}

\remark{La continuité est nécessaire pour appliquer ce théorème.}

\attention{Ne pas confondre continuité et dérivabilité.}

\vocabulary{Une bijection est une fonction à la fois injective et surjective.}

\carreaux{10}

\end{document}
```

---

## ✍️ Auteur

Développé par **Ewen**, étudiant-entrepreneur en Mathématiques et Informatique à l'Université Paris Cité, CEO de [Wybz](https://github.com/funoxpanda), dans le cadre de l’optimisation de la rédaction pédagogique de cours scientifiques.

---

## 📜 Licence

Ce projet est sous licence MIT — libre à toi de le modifier, partager, et utiliser dans tes propres projets.
