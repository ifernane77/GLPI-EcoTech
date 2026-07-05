# Procédure d’accès à la VM Debian — GLPI EcoTech

## Objectif

Ce document explique comment accéder à la machine virtuelle Debian prévue pour le projet GLPI EcoTech.

## Étapes d’accès prévues

1. Ouvrir le logiciel de virtualisation.
2. Sélectionner la machine virtuelle Debian 11.
3. Démarrer la machine virtuelle.
4. Se connecter avec l’utilisateur prévu.
5. Ouvrir un terminal.
6. Vérifier que la VM fonctionne correctement.
7. Vérifier l’accès au réseau.

## Informations à compléter

| Élément | Valeur |
|---|---|
| Nom de la VM | Debian-GLPI-EcoTech |
| Système | Debian 11 |
| Utilisateur | À compléter |
| Mot de passe | Non stocké dans GitHub |
| Adresse IP | À compléter après vérification |
| Logiciel utilisé | VirtualBox ou VMware |

## Règle importante

Le mot de passe de la VM ne doit pas être écrit dans le dépôt GitHub.

Si une information sensible est nécessaire, elle doit rester hors du dépôt.

## Commandes de vérification

Commandes simples à utiliser dans Debian :

```bash
whoami
hostnamectl
ip a