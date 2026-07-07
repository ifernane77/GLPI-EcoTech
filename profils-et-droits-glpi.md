# Profils et droits GLPI — GLPI EcoTech

## Objectif

Ce document prépare les profils et droits qui seront utilisés dans GLPI EcoTech.

Le but est de ne pas donner les mêmes droits à tous les utilisateurs.

---

## Profils prévus

| Profil | Rôle simple |
|---|---|
| Super-admin | Configuration complète de GLPI |
| Technicien | Traitement des tickets |
| Demandeur | Création et suivi de ses tickets |
| Observateur | Consultation de certaines informations |

---

## Super-admin

Le profil Super-admin pourra gérer toute la configuration GLPI.

Il sera utilisé pour :

- créer les utilisateurs ;
- créer les groupes ;
- créer les catégories ;
- ajouter les équipements ;
- configurer les profils.

Ce profil doit être limité au compte administrateur.

---

## Technicien

Le profil Technicien servira au support informatique.

Il pourra :

- lire les tickets ;
- répondre aux demandes ;
- modifier le statut d’un ticket ;
- associer un ticket à un équipement ;
- clôturer un ticket.

---

## Demandeur

Le profil Demandeur sera utilisé par les employés.

Il pourra :

- créer un ticket ;
- suivre ses demandes ;
- ajouter une précision ;
- consulter les réponses.

Il ne doit pas modifier la configuration de GLPI.

---

## Observateur

Le profil Observateur pourra servir aux gérants.

Il permettra de consulter certaines informations sans modifier toute la configuration.

---

## Tableau simple des droits

| Action | Demandeur | Observateur | Technicien | Super-admin |
|---|---|---|---|---|
| Créer un ticket | Oui | Oui | Oui | Oui |
| Suivre ses tickets | Oui | Oui | Oui | Oui |
| Traiter un ticket | Non | Non | Oui | Oui |
| Clôturer un ticket | Non | Non | Oui | Oui |
| Ajouter un équipement | Non | Non | Limité | Oui |
| Créer un utilisateur | Non | Non | Non | Oui |
| Modifier la configuration | Non | Non | Non | Oui |

---

## Remarque personnelle

Cette répartition me permet de préparer une gestion plus sécurisée.

Chaque utilisateur aura seulement les droits utiles à son rôle.