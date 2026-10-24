# Organisation constatée dans GLPI

## Entités

L’entité `EcoTech` est créée sous l’entité racine. Son commentaire décrit une simulation de gestion du parc et du support interne. Les fiches du parc et les tickets EcoTech sont visibles dans ce périmètre.

## Groupes et utilisateurs

Quatre groupes figurent dans la capture de liste : `EcoTech - Employés`, `EcoTech - Gérants`, `EcoTech - Prestataires`, `EcoTech - Support informatique`. Leur entité affichée est **Entité racine**. Leur présence ne prouve pas leur portée récursive ni la composition de chacun.

Cinq comptes EcoTech sont visibles, en plus du compte `glpi`. Voir [utilisateurs et droits](utilisateurs-et-droits.md).

## Équipements et services

Le [registre du parc](inventaire-parc.md) décrit neuf fiches simulées. L’[inventaire par agent](agent-glpi/installation.md) concerne séparément le client `Debian-Client-GLPI-Agent` dans l’entité racine. Ne pas présenter les neuf fiches comme issues de cet agent.

GLPI centralise des fiches d’équipements, des tickets et des procédures. Google Drive est un service évoqué par un ticket et un article ; aucune intégration automatique avec Google Drive n’est démontrée.

## Preuves

[Entités, comptes, groupes et habilitation](preuves/utilisateurs-profils/README.md), [parc](preuves/parc/README.md), [tickets](preuves/tickets/README.md).
