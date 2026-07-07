
---

# 3. Fichier : `groupes-utilisateurs-glpi.md`

Copie-colle uniquement ce bloc dans `groupes-utilisateurs-glpi.md`.

```md
# Groupes utilisateurs GLPI — GLPI EcoTech

## Objectif

Ce document prépare les groupes utilisateurs qui seront créés plus tard dans GLPI.

Cette semaine, les leçons parlent des utilisateurs et des groupes.

J’utilise donc cette logique pour organiser les futurs utilisateurs GLPI d’EcoTech.

---

## Groupes prévus

| Groupe | Utilisateurs concernés | Rôle prévu |
|---|---|---|
| Gérants | Les 2 gérants associés | Suivi des demandes et décisions |
| Employés | Employé administratif et employé terrain | Création de tickets et demandes |
| Prestataires | Prestataires terrain si besoin | Signalement limité |
| Support informatique | Technicien ou administrateur GLPI | Traitement des tickets |
| Administration GLPI | Compte administrateur | Configuration de GLPI |

---

## Groupe Gérants

Les gérants pourront :

- suivre les tickets importants ;
- consulter l’état du parc ;
- demander une intervention ;
- suivre les problèmes récurrents.

---

## Groupe Employés

Les employés pourront :

- déclarer un incident ;
- faire une demande ;
- suivre leurs tickets ;
- ajouter des précisions si besoin.

Exemples :

- imprimante indisponible ;
- document introuvable ;
- accès Google Drive ;
- problème sur un poste.

---

## Groupe Prestataires

Les prestataires ne sont pas prioritaires dans la première version.

Si besoin, ils pourront être ajoutés plus tard avec des droits limités.

---

## Groupe Support informatique

Le support informatique pourra :

- recevoir les tickets ;
- qualifier les demandes ;
- associer un ticket à un équipement ;
- ajouter une solution ;
- clôturer un ticket.

---

## Groupe Administration GLPI

Ce groupe sera réservé à la configuration.

Il pourra gérer :

- les utilisateurs ;
- les profils ;
- les groupes ;
- les catégories ;
- les équipements.

---

## Remarque personnelle

Je ne veux pas donner trop de droits à tous les utilisateurs.

Je prépare donc des groupes simples pour séparer les rôles de chacun.