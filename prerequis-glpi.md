
---

## `prerequis-glpi.md`

```md
# Prérequis GLPI — GLPI EcoTech

## Objectif

Ce document liste les prérequis nécessaires pour installer GLPI sur Debian 11.

## Prérequis système

Pour installer GLPI, il faut prévoir :

- une machine Debian 11 fonctionnelle ;
- un accès Internet ;
- un utilisateur avec les droits administrateur ;
- un serveur web ;
- PHP ;
- une base de données ;
- un navigateur pour accéder à GLPI.

## Composants nécessaires

| Composant | Rôle |
|---|---|
| Debian 11 | Système d’exploitation serveur |
| Apache | Serveur web |
| PHP | Langage utilisé par GLPI |
| MariaDB ou MySQL | Base de données |
| Navigateur web | Accès à l’interface GLPI |
| GitHub | Stockage de la documentation |

## Vérifications avant installation

Avant d’installer GLPI, il faudra vérifier :

- que Debian démarre correctement ;
- que le réseau fonctionne ;
- que le système peut être mis à jour ;
- que les droits administrateur sont disponibles ;
- que l’espace disque est suffisant ;
- que la date et l’heure sont correctes.

## Risques possibles

Les difficultés possibles sont :

- problème de connexion Internet dans la VM ;
- oubli du mot de passe utilisateur ;
- erreur lors de l’installation des paquets ;
- problème de version PHP ;
- problème de droits sur les fichiers ;
- erreur de connexion à la base de données.

## Preuves attendues

Les preuves à garder seront :

- capture de la VM Debian ;
- capture des commandes de vérification ;
- capture des prérequis installés plus tard ;
- capture du dépôt GitHub avec la documentation ;
- commit Git.