# Présentation — GLPI EcoTech

## Contexte et périmètre

Le projet simule le support informatique d’EcoTech, petite entreprise du BTP à Saint-Pierre, La Réunion. Il illustre la gestion du patrimoine, des incidents et demandes et la documentation d’un service informatique pour E5.

L’environnement technique comporte une VM serveur Debian 11 avec Apache, PHP, MariaDB et GLPI et une VM cliente Debian avec GLPI Agent. L’organisation EcoTech, ses utilisateurs, équipements et tickets sont représentés dans GLPI avec des données de simulation.

## Travail attesté

- Installation serveur documentée et captures d’accès à GLPI.
- Configuration réseau des VM et remontée du client Debian par GLPI Agent.
- Création d’une entité EcoTech, de cinq comptes EcoTech et de quatre groupes.
- Habilitation Technician du compte support dans EcoTech.
- Neuf équipements simulés enregistrés et un PC administratif détaillé.
- Huit tickets visibles ; interventions et solutions détaillées pour les incidents imprimante et Internet, premières vérifications pour le Wi-Fi du téléphone.
- Procédure de déclaration d’un ticket et trace d’un article Google Drive.

## Limites de présentation

Les captures prouvent les données saisies et les états affichés. Les interventions déclarées dans les tickets restent celles d’une simulation ; elles ne certifient pas une intervention sur les équipements physiques de l’entreprise. Le client Debian inventorié est visible séparément dans l’entité racine, sans rattachement EcoTech démontré.

Aucun Active Directory, VLAN, serveur physique de production, supervision avancée ou déploiement de GLPI dans l’entreprise n’est revendiqué. Les droits de tous les comptes, la sauvegarde/restauration et l’exécution technique des demandes externes restent à étayer.

Voir l’[index des preuves](preuves/README.md) et le [compte rendu des compléments](compte-rendu-coherence.md).

## Chronologie par rapport au stage

Selon la précision apportée par l’auteur le 24 octobre 2026, le stage a commencé le **18 août 2026**. Le travail GLPI présenté dans ce dépôt a été réalisé **avant le stage**, alors que l’auteur partageait déjà les bureaux de l’entreprise. Les commits antérieurs au 18 août sont cohérents avec cette chronologie et leurs dates sont conservées.

Ce travail antérieur est présenté comme tel. Il ne doit pas être comptabilisé comme une activité effectuée pendant le stage. Toute activité ultérieure réellement réalisée pendant le stage doit être décrite séparément avec ses dates et preuves ; aucune n’est déduite automatiquement des fichiers existants.
