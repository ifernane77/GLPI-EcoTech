# GLPI EcoTech — présentation pour le portfolio

## Contexte

J’ai réalisé une simulation de support informatique adaptée au contexte d’EcoTech, petite entreprise du BTP à Saint-Pierre, La Réunion. L’objectif est de centraliser un parc, des utilisateurs, des tickets et des procédures dans GLPI.

## Réalisation

J’ai documenté l’installation de GLPI sur une VM Debian 11 avec Apache, PHP et MariaDB. J’ai également documenté un client Debian équipé de GLPI Agent et conservé une capture de sa remontée d’inventaire, ainsi que des captures de ses logiciels et composants.

Dans le scénario EcoTech, les preuves montrent une entité, cinq comptes EcoTech, quatre groupes et neuf fiches d’équipements simulés. Le compte support dispose du profil Technician dans EcoTech.

La liste de support comporte huit tickets : six clos, un résolu et un en cours. Les captures détaillées des incidents imprimante et Internet montrent les actions et solutions saisies jusqu’à la clôture. Le problème Wi-Fi du téléphone terrain reste en cours dans la preuve disponible.

Une procédure explique comment déclarer un ticket. Un article d’accès Google Drive apparaît aussi dans la base de connaissances.

## Ce que je peux démontrer

- Recenser et organiser des ressources informatiques dans GLPI.
- Tracer la prise en charge et la résolution d’incidents dans une simulation.
- Documenter la mise à disposition d’un service et l’inventaire par agent.
- Produire une procédure pour les utilisateurs et versionner la documentation avec Git.

## Limites connues

Les neuf fiches EcoTech sont des données de simulation. Elles ne doivent pas être confondues avec le client Debian inventorié automatiquement, visible séparément dans l’entité racine. Les captures ne certifient pas un déploiement en production dans l’entreprise.

Les détails de cinq tickets, les habilitations de tous les utilisateurs, la composition des groupes et une restauration testée restent à conserver. Je ne présente pas ces points comme validés.

[Preuves sélectionnées](preuves-portfolio.md) — [préparation orale](script-oral-glpi.md) — [compléments à apporter](../compte-rendu-coherence.md).

## Chronologie par rapport au stage

Mon stage a commencé le **18 août 2026**. J’avais réalisé le travail GLPI présenté ici avant cette date, alors que je partageais déjà les bureaux de l’entreprise. Je le présente comme un travail antérieur au stage, contextualisé chez EcoTech. Les activités effectuées pendant le stage doivent être identifiées séparément et étayées par leurs propres preuves. Les dates des commits historiques sont conservées.
