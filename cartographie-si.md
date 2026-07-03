# Cartographie du système d’information — GLPI EcoTech

## Objectif

Ce document présente une cartographie simple du système d’information cible d’EcoTech dans le cadre du projet GLPI EcoTech.

L’objectif est de préparer l’intégration future des équipements dans GLPI et de produire une preuve exploitable pour l’épreuve E5.

## Équipements identifiés

Le parc informatique cible est composé de :

- 2 PC fixes ;
- 2 PC portables ;
- 2 machines Windows ;
- 2 machines Mac ;
- 3 téléphones professionnels ;
- 1 imprimante / scanner ;
- 1 Livebox ;
- des emails professionnels ;
- un stockage actuel réparti entre Google Drive, PC personnels, mails et WhatsApp.

## Schéma simplifié du système d’information

```mermaid
flowchart TD
    Internet[Internet] --> Livebox[Livebox]
    Livebox --> PCFixe1[PC fixe administratif 1]
    Livebox --> PCFixe2[PC fixe administratif 2]
    Livebox --> Portable1[PC portable gérant 1]
    Livebox --> Portable2[PC portable gérant 2]
    Livebox --> Imprimante[Imprimante / Scanner]
    Tel1[Téléphone pro 1] --> Internet
    Tel2[Téléphone pro 2] --> Internet
    Tel3[Téléphone pro 3] --> Internet
    PCFixe1 --> Drive[Google Drive]
    PCFixe2 --> Drive
    Portable1 --> Drive
    Portable2 --> Drive
    Tel1 --> WhatsApp[WhatsApp]
    Tel2 --> WhatsApp
    Tel3 --> WhatsApp
    GLPI[GLPI EcoTech] --> Parc[(Inventaire du parc)]
    GLPI --> Tickets[(Tickets incidents / demandes)]
    GLPI --> BaseCo[(Base de connaissances)]