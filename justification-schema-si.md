# Justification du schéma SI — GLPI EcoTech

## Objectif

Ce document explique les choix réalisés pour le schéma du système informatique EcoTech.

Il permet de justifier le lien entre le contexte de l’entreprise, les équipements et l’utilisation prévue de GLPI.

---

## Pourquoi faire un schéma du SI ?

Le schéma du SI permet de visualiser les éléments importants du système informatique.

Il permet de comprendre :

- quels équipements sont utilisés ;
- quels utilisateurs utilisent quels équipements ;
- quels services numériques sont utilisés ;
- où GLPI intervient ;
- quels éléments peuvent être liés à des tickets.

---

## Choix des équipements représentés

Les équipements représentés correspondent au contexte réel d’EcoTech :

| Élément | Justification |
|---|---|
| PC fixes | Utilisés pour l’administratif, les documents, devis et factures |
| PC portables | Utilisés par les gérants pour le suivi et les échanges |
| Téléphones professionnels | Utilisés pour les appels, WhatsApp et les photos de chantier |
| Imprimante / scanner | Utilisée pour les documents administratifs |
| Livebox | Point central de l’accès Internet |
| Google Drive | Stockage actuel des documents |
| Emails professionnels | Communication professionnelle |
| WhatsApp | Échanges terrain et photos |
| Serveur GLPI de test | Simulation du service de support informatique |

---

## Pourquoi intégrer GLPI ?

GLPI permet de structurer le support informatique.

Dans le projet EcoTech, GLPI servira à :

- inventorier les équipements ;
- classer les incidents ;
- suivre les demandes ;
- documenter les solutions ;
- créer une base de connaissances ;
- améliorer le suivi du parc informatique.

---

## Lien avec les problèmes EcoTech

EcoTech rencontre un problème de centralisation.

Les informations sont dispersées entre :

- Google Drive ;
- les PC personnels ;
- les mails ;
- WhatsApp ;
- les échanges oraux.

Le schéma permet de montrer que GLPI peut apporter une organisation plus claire pour la partie support informatique.

---

## Simplicité volontaire

Le schéma reste simple.

Il ne présente pas :

- de VLAN ;
- de pare-feu avancé ;
- d’Active Directory ;
- de serveur physique complexe ;
- de supervision réseau ;
- de haute disponibilité.

Ces éléments seraient trop ambitieux pour le contexte actuel.

Le but est de produire une simulation professionnelle réaliste et compréhensible pour un niveau BTS SIO.

---

## Lien avec l’épreuve E5

Cette semaine prépare plusieurs compétences E5 :

- gérer le patrimoine informatique ;
- répondre aux incidents et demandes ;
- mettre à disposition un service informatique ;
- travailler en mode projet.

Le schéma aide à expliquer le contexte technique avant de présenter GLPI.

---

## Conclusion

Le schéma SI EcoTech permet de comprendre l’environnement informatique de l’entreprise.

Il prépare la future saisie des équipements, catégories, tickets et procédures dans GLPI.