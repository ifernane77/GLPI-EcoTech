# Installation GLPI — GLPI EcoTech

## Objectif

Ce document prépare l’installation de GLPI dans le cadre du projet GLPI EcoTech.

À cette étape, l’objectif n’est pas encore de finaliser toute l’installation, mais de préparer l’environnement, les prérequis et la procédure à suivre.

## Contexte

GLPI EcoTech est une simulation professionnelle réalisée pour le BTS SIO.

Le projet a pour objectif de représenter la gestion du support informatique d’une petite entreprise : EcoTech.

GLPI permettra plus tard de gérer :

- le parc informatique ;
- les utilisateurs ;
- les tickets d’incidents ;
- les demandes internes ;
- une base de connaissances.

## Environnement prévu

L’installation de GLPI sera réalisée sur une machine virtuelle Debian 11.

L’environnement prévu est le suivant :

| Élément | Choix prévu |
|---|---|
| Système | Debian 11 |
| Application | GLPI |
| Serveur web | Apache |
| Base de données | MariaDB ou MySQL |
| Langage | PHP |
| Accès | Navigateur web |
| Documentation | Markdown + captures d’écran |

## Étapes prévues

Les étapes prévues pour l’installation sont :

1. vérifier que la VM Debian 11 fonctionne ;
2. vérifier l’accès à Internet ;
3. mettre à jour le système ;
4. installer les prérequis nécessaires ;
5. installer Apache ;
6. installer PHP ;
7. installer MariaDB ou MySQL ;
8. télécharger GLPI ;
9. configurer la base de données ;
10. lancer l’assistant d’installation GLPI ;
11. faire les captures d’écran ;
12. documenter les problèmes rencontrés.

## Commandes prévues plus tard

Les commandes exactes seront testées et documentées lors de l’installation réelle.

Exemples de commandes qui pourront être utilisées :

```bash
sudo apt update
sudo apt upgrade
sudo apt install apache2
sudo apt install mariadb-server
sudo apt install php