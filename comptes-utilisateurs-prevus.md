# Comptes utilisateurs prévus — GLPI EcoTech

## Objectif

Ce document liste les comptes utilisateurs qui pourront être créés plus tard dans GLPI.

Les noms restent fictifs pour le projet BTS.

Aucun mot de passe réel ne doit être écrit dans GitHub.

---

## Comptes prévus

| Compte prévu | Groupe | Profil GLPI prévu | Utilisation |
|---|---|---|---|
| gerant1.ecotech | Gérants | Observateur / demandeur | Suivre les tickets importants |
| gerant2.ecotech | Gérants | Observateur / demandeur | Suivre les tickets importants |
| admin.ecotech | Employés | Demandeur | Déclarer des demandes administratives |
| terrain.ecotech | Employés | Demandeur | Signaler des problèmes terrain |
| support.ecotech | Support informatique | Technicien | Traiter les tickets |
| glpi.admin | Administration GLPI | Super-admin | Configurer GLPI |

---

## Gérants

Les deux gérants doivent pouvoir suivre les demandes importantes.

Ils n’ont pas besoin d’avoir tous les droits d’administration GLPI.

---

## Employé administratif

L’employé administratif peut créer des tickets liés :

- aux documents ;
- aux devis ;
- aux factures ;
- à Google Drive ;
- à l’imprimante ;
- aux postes fixes.

---

## Employé terrain

L’employé terrain peut créer des tickets liés :

- aux téléphones professionnels ;
- aux photos de chantier ;
- aux problèmes d’accès ;
- aux demandes liées au terrain.

---

## Support informatique

Le compte support est prévu pour traiter les tickets.

Il pourra :

- lire les tickets ;
- répondre ;
- changer le statut ;
- associer un équipement ;
- clôturer la demande.

---

## Administrateur GLPI

Le compte administrateur GLPI sert uniquement à configurer l’outil.

Il ne doit pas être utilisé comme compte quotidien pour déclarer des tickets.

---

## Règle importante

Les mots de passe ne doivent jamais être écrits dans le dépôt GitHub.

Si un mot de passe est utilisé en test, il doit rester local et ne pas apparaître dans les fichiers Markdown.