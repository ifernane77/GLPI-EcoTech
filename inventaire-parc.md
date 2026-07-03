## Fichier `inventaire-parc.md`

# Inventaire prévisionnel du parc informatique — EcoTech

## Objectif

Ce document prépare l’inventaire du parc informatique qui sera ensuite intégré dans GLPI.

Il sert à identifier les équipements, leurs usages et les informations importantes à conserver.

## Matériel recensé

| Type de matériel | Quantité | Utilisation prévue | Intégration GLPI |
|---|---:|---|---|
| PC fixes | 2 | Gestion administrative et documents | Oui |
| PC portables | 2 | Utilisation par les gérants ou employés | Oui |
| Machines Windows | 2 | Postes utilisateurs | Oui |
| Machines Mac | 2 | Postes utilisateurs | Oui |
| Téléphones professionnels | 3 | Appels, photos de chantier, échanges terrain | Oui |
| Imprimante / scanner | 1 | Impression et numérisation de documents | Oui |
| Livebox | 1 | Accès Internet de l’entreprise | Oui |
| Emails professionnels | Non précisé | Communication professionnelle | À documenter |
| Google Drive | Non précisé | Stockage de documents | À documenter |

## Informations à renseigner plus tard dans GLPI

Pour chaque équipement, il faudra idéalement renseigner :

- nom de l’équipement ;
- type ;
- utilisateur principal ;
- système d’exploitation ;
- état ;
- date d’ajout ;
- localisation ;
- remarques ;
- incidents associés.

## Exemple de nommage des équipements

| Équipement | Nom possible dans GLPI |
|---|---|
| PC fixe administratif 1 | PC-ADM-01 |
| PC fixe administratif 2 | PC-ADM-02 |
| PC portable gérant 1 | PC-GER-01 |
| PC portable gérant 2 | PC-GER-02 |
| Téléphone professionnel 1 | TEL-PRO-01 |
| Téléphone professionnel 2 | TEL-PRO-02 |
| Téléphone professionnel 3 | TEL-PRO-03 |
| Imprimante / scanner | IMP-SCAN-01 |
| Livebox | BOX-01 |

## Problèmes identifiés

Les problèmes possibles sont :

- absence d’inventaire centralisé ;
- absence de suivi clair des incidents ;
- antivirus inconnu ;
- absence de politique de sauvegarde formalisée ;
- utilisation de plusieurs supports de stockage ;
- documentation technique limitée.

## Lien avec GLPI

GLPI permettra de créer une base centralisée du parc informatique et de relier les équipements à des tickets d’incidents ou de demandes.

Cette étape prépare la compétence E5 liée à la gestion du patrimoine informatique.