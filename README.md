# Loïc MILANDOU

**Ingénieur en systèmes industriels · Élève à 42 Paris · En transition vers l'informatique**
Je développe un moteur de tableur de zéro comme projet de fin d'études personnel

---

## Spreadsheet Engine

### Pourquoi ce projet ?
Ce projet m'interesse particulierement dû fait de son omniprésence dans les environnements professionnels et de la complexité d'ingénierie.
Mon objectif est de réaliser un tableur performant (faible empreinte mémoire, réponse rapide) qui nativement supporte une utilisation concurrente.
Le construire de zéro me permettra de familiariser à la théorie des compilateurs, les algoritmhes de graphe, les systemes distribuées, la cybersécurité dans un seul projet cohérent et concret.

### Livrables principaux

**Langage d'expression et interpreteur**
C'est le principal outil de communication entre l'utilisateur et le logiciel. Il doit notamment être orienté données et avoir des erreurs claires.

**Graphe de dépendances et détection des cycles**
Le moteur doit être capable de _présenter_ le graphe de dépendance à l'utilisateur et détecter les références circulaires.

**Systemes distribués et Cybersécurité**
Le moteur sera distribué comme un serveur et être capable de supporter l'acces concurrent de plusieurs utilisateurs tout en respectant les droits d'accès et de modification.

## Stack technique
Le moteur sera développé en C / C++.
