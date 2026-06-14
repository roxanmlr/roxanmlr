# Loïc MILANDOU

**Ingénieur en systèmes industriels · Élève à 42 Paris · Programmation système, réseau et backend en C++**

---

## Projet principal : WebServer

Serveur HTTP en **C++98**, développé à 42 Paris.

L'objectif : comprendre en profondeur le fonctionnement d'un serveur web, des sockets bas niveau jusqu'au traitement complet des requêtes HTTP — sans framework, sans abstraction cachée.

---

### Ce que le projet couvre

```txt
socket · bind · listen · accept · recv · send · close
epoll · non-blocking I/O · HTTP/1.1 · multiclients · Docker
```

- Serveur HTTP sans framework, implémenté from scratch
- Gestion de plusieurs clients simultanés
- Sockets non bloquantes
- Multiplexage d'E/S avec `epoll`
- Parsing HTTP/1.1 : méthodes, en-têtes, corps, chunked encoding
- Réponses HTTP valides : statuts, en-têtes, corps
- Fichiers statiques
- Méthodes `GET`, `POST`, `DELETE`
- Upload de fichiers
- Pages d'erreur personnalisées
- Exécution sous Docker
- Tests de robustesse et de performance (`ab`, `wrk`, `siege`)

---

### Compétences mobilisées

| Domaine               | Détail                                                                 |
|-----------------------|------------------------------------------------------------------------|
| **Langage**           | C++98 — classes, RAII, gestion mémoire manuelle, sans STL moderne     |
| **Réseau**            | Sockets TCP, protocole HTTP/1.1, modèle client/serveur                |
| **Système**           | Linux, appels système, E/S non bloquantes, `epoll`, signaux           |
| **Architecture**      | Séparation parsing / routing / réponse, configuration multi-serveurs  |
| **Tests & perfs**     | Tests de charge, robustesse, débogage système, profiling              |
| **Conteneurisation**  | Docker — isolation, déploiement reproductible                         |

---

### Architecture simplifiée

```txt
Client TCP
    ↓
epoll (multiplexage)
    ↓
Réception des données (recv)
    ↓
Parser HTTP
    ↓
Router / Handler
    ↓
Réponse HTTP (send)
    ↓
Client TCP
```

---

### Pourquoi ce projet

WebServer est un projet de programmation système pur. Il n'y a pas de framework pour masquer la complexité : chaque couche — réseau, parsing, gestion des connexions, génération des réponses — est implémentée à la main.

C'est une base directement utile pour la **cybersécurité** (compréhension des comportements serveur, surface d'attaque, protocoles) et pour le **backend bas niveau** (performance, robustesse, architecture).

> Serveur HTTP · C++98 · Linux · sockets · epoll · HTTP/1.1 · Docker · architecture système

---

## Stack

| Catégorie      | Technologies                       |
|----------------|------------------------------------|
| **Langages**   | C · C++ · Go · Python              |
| **Système**    | Linux · Docker · Git · Makefile    |
| **Backend**    | HTTP · Nginx · REST APIs           |
| **Bases**      | PostgreSQL · SQLite                |

---

## Profil

Ingénieur diplômé en **systèmes industriels (2016)**, élève à **42 Paris**, en transition vers le développement logiciel avec une double spécialité **cybersécurité** et **IA** visée à l'horizon **2027**.

Disponible sur le marché informatique à partir de **décembre 2026**.

---

## Contact

**Loïc MILANDOU**

- GitHub : [@roxanmlr](https://github.com/roxanmlr)
- Disponibilité : **décembre 2026**
