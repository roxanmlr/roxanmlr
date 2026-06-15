# Loïc MILANDOU

Élève à **42 Paris**, je développe un moteur de tableur de zéro comme projet de fin d'études personnel.

---

## Spreadsheet Engine

Un tableur est une interface familière qui cache un problème d'ingénierie non trivial : derrière chaque cellule se trouve un **langage d'expression**, un **graphe de dépendances** et un **moteur d'évaluation**. Construire ce système de zéro, c'est croiser la théorie des compilateurs, l'algorithmique des graphes et le traitement de données dans un seul projet cohérent et concret.

### Pourquoi ce projet

La plupart des projets de portfolio s'arrêtent à l'interface ou à un CRUD. Un moteur de tableur impose d'aller plus loin : il faut comprendre ce qui se passe *sous* l'interface, concevoir un pipeline de traitement complet — de la saisie d'une formule jusqu'au résultat affiché — et gérer des cas que l'on ne peut pas esquiver (cycles, erreurs de types, recalcul partiel).

C'est un projet qui se justifie par sa profondeur technique, pas par sa visibilité.

### Aspects techniques couverts

**Parsing de formules**
Tokenisation du texte saisi, construction d'une grammaire, gestion des priorités d'opérateurs, production d'un arbre syntaxique abstrait (AST).

**Graphe de dépendances**
Chaque cellule référençant une autre crée une arête dans un graphe orienté. Toute modification doit propager le recalcul dans le bon ordre — ce qui nécessite un tri topologique.

**Détection de cycles**
Une référence circulaire est une erreur silencieuse dans un tableur naïf. Le moteur doit la détecter, la signaler et rester dans un état cohérent.

**Moteur d'évaluation**
Parcours de l'AST, évaluation récursive des expressions, recalcul incrémental (ne recalculer que ce qui a changé), mise en cache des résultats intermédiaires.

**Système de types**
Les cellules contiennent des nombres, des chaînes, des booléens, des dates ou des erreurs. Les erreurs se propagent dans les formules comme dans Excel (`#REF!`, `#DIV/0!`, `#CYCLE!`...).

**Fonctions natives**
Implémenter `SUM`, `IF`, `AVERAGE`, `VLOOKUP` et d'autres oblige à concevoir un mécanisme d'appel de fonctions intégré à l'évaluateur, avec gestion des plages de cellules comme arguments.

**Persistance et sérialisation**
Sauvegarde et rechargement d'un état complet : cellules, formules, types, métadonnées. Import et export de formats courants.

**IA appliquée** *(en cours de réflexion)*
Explication de formules en langage naturel, détection d'anomalies dans les données, génération assistée de formules.

---

## Stack

Le projet est développé en **Go**, avec une interface en ligne de commande dans un premier temps. Les choix techniques sont motivés par la clarté du code et la facilité de test, pas par la mode.

---

## Contact

**Loïc MILANDOU** · [@roxanmlr](https://github.com/roxanmlr)
