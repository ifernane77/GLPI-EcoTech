# Utilisateurs et droits — GLPI EcoTech

## Objectif

Ce document prépare l’organisation des utilisateurs, groupes et droits dans GLPI.

## Groupes prévus

| Groupe | Rôle |
|---|---|
| Gérants | Suivi global |
| Employés | Création de tickets |
| Prestataires | Accès limité si besoin |
| Support informatique | Traitement des tickets |

## Comptes prévus

| Compte | Profil prévu | Utilisation |
|---|---|---|
| gerant01 | Responsable | Suivi global |
| gerant02 | Responsable | Suivi global |
| administratif01 | Demandeur | Tickets administratifs |
| terrain01 | Demandeur | Tickets terrain |
| support01 | Technicien | Traitement des tickets |

## Droits simples

| Profil | Créer un ticket | Suivre ses tickets | Traiter les tickets | Gérer le parc |
|---|---:|---:|---:|---:|
| Demandeur | Oui | Oui | Non | Non |
| Technicien | Oui | Oui | Oui | Partiellement |
| Responsable | Oui | Oui | Oui | Oui |

## Règles retenues

- Les droits restent simples.
- Chaque utilisateur a un rôle clair.
- Les mots de passe ne sont pas stockés dans GitHub.
- Les tests seront faits avec au moins un demandeur et un technicien.