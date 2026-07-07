# Entités GLPI prévues — GLPI EcoTech

## Objectif

Ce document prépare les entités qui seront utilisées plus tard dans GLPI EcoTech.

À cette étape, je ne crée pas encore forcément les entités dans GLPI.

Je prépare d’abord l’organisation pour rester cohérent avec les leçons sur les utilisateurs, groupes et droits.

---

## Entité principale prévue

| Entité | Rôle |
|---|---|
| EcoTech | Entité principale pour gérer le parc, les utilisateurs et les tickets |

---

## Pourquoi une seule entité ?

EcoTech est une petite entreprise.

Pour une première version BTS, une seule entité est suffisante.

Elle permettra de regrouper :

- les utilisateurs ;
- les équipements ;
- les tickets ;
- les demandes ;
- les catégories ;
- la base de connaissances.

---

## Organisation prévue

```text
EcoTech
├── Gérants
├── Employés
├── Prestataires
└── Support informatique