
---

## `environnement-debian.md`

```md
# Environnement Debian — GLPI EcoTech

## Objectif

Ce document décrit l’environnement Debian prévu pour installer GLPI.

## Machine virtuelle prévue

| Élément | Description |
|---|---|
| Système | Debian 11 |
| Type | Machine virtuelle |
| Usage | Serveur GLPI de test |
| Projet | GLPI EcoTech |
| Épreuve | E5 BTS SIO |

## Rôle de la VM

La machine virtuelle Debian servira de serveur de test pour GLPI.

Elle permettra de simuler un environnement professionnel simple pour :

- installer GLPI ;
- gérer un parc informatique ;
- créer des tickets ;
- gérer des demandes ;
- rédiger une base de connaissances ;
- produire des captures pour le portfolio.

## Vérifications à faire

Avant l’installation de GLPI, il faudra vérifier :

- que la VM démarre correctement ;
- que Debian est accessible ;
- que l’utilisateur peut ouvrir une session ;
- que la connexion Internet fonctionne ;
- que les commandes Linux de base fonctionnent ;
- que les mises à jour peuvent être lancées.

## Commandes simples de vérification

Lorsque la VM sera lancée, les commandes suivantes pourront être utilisées :

```bash
hostnamectl
ip a
pwd
whoami