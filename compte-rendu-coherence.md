# Compte rendu de cohérence et compléments E5

Révision documentaire : 24 octobre 2026. Base examinée : commit `661422d` du 16 août 2026. Aucune intervention dans l’application GLPI n’a été effectuée lors de cette révision.

## Corrections effectuées

- Remplacement des annonces « installation future » par l’état documenté du laboratoire.
- Alignement des comptes, groupes et équipements sur les noms visibles dans les captures.
- Remplacement des huit scénarios prévisionnels par le registre des huit tickets effectivement visibles, sans confondre existence, statut et détail de traitement.
- Distinction entre six tickets clos, un résolu et un en cours.
- Distinction entre neuf équipements simulés et le client Debian inventorié par agent dans l’entité racine.
- Remplacement du journal hebdomadaire par une chronologie des commits, sans inventer dates ou heures d’intervention.
- Classement des 37 images originales par thème, suppression des dossiers hebdomadaires vides et correction des liens.
- Conservation des captures historiques de cadrage avec une explication de leur portée.
- Neutralisation du mot de passe SQL dans le texte courant ; signalement de sa présence dans l’historique et de l’alerte sur les comptes par défaut.
- Création d’un parcours portfolio et d’un fil conducteur oral fondés sur les preuves disponibles.

## Compléments prioritaires et mode opératoire

| Priorité | Preuve manquante ou partielle | Comment la compléter | Emplacement conseillé |
|---|---|---|---|
| 1 | Tickets 5, 6, 7, 9 et 11, détails absents | Ouvrir chaque ticket ; conserver description, type, catégorie, acteurs, suivis/tâches, solution, matériel éventuel et dates. Utiliser plusieurs captures ou un export lisible si nécessaire. | preuves/tickets/ |
| 1 | Habilitations des demandeurs et gérants | Administration → Utilisateurs → compte → Habilitations ; capturer profil, entité, récursivité. Le nom admin.ecotech ne suffit pas à prouver des droits administrateur. | preuves/utilisateurs-profils/ |
| 1 | Tests des droits | Se connecter avec un demandeur et le support ; créer/suivre un ticket de test, vérifier les accès autorisés et refusés. Consigner compte, date, résultat réel et capture ; identifier le ticket comme test. | preuves/utilisateurs-profils/ |
| 1 | Secrets et comptes par défaut | Vérifier les comptes par défaut. Si l’ancien secret SQL a été utilisé, le changer dans MariaDB et la configuration GLPI, puis tester l’accès. Aucune capture ne doit montrer un secret. | regles-securisation-equipements.md et preuves/installation-serveur/ |
| 2 | Membres et portée des groupes | Administration → Groupes → groupe : capturer les utilisateurs, l’entité et la récursivité ; vérifier la cohérence avec EcoTech avant de revendiquer la portée souhaitée. | preuves/utilisateurs-profils/ |
| 2 | Catégories et types des demandes | Ouvrir la configuration des catégories et capturer l’arborescence ; ouvrir les demandes 6, 9 et 11 pour montrer leur type effectif. | preuves/tickets/ |
| 2 | Détails des équipements associés | Ouvrir imprimante, Livebox et téléphone terrain ; conserver fiche, localisation, utilisateur/responsable éventuel et onglet Tickets ; exporter la liste du parc. | preuves/parc/ |
| 2 | Source et date du client inventorié | Ouvrir Debian-Client-GLPI-Agent ; relever la source d’inventaire, l’agent, la dernière remontée et l’entité ; effectuer un nouvel envoi si nécessaire. Documenter un éventuel rattachement à EcoTech sans le présumer déjà fait. | preuves/inventaire-agent/ |
| 2 | Versions et accès actuel | Démarrer le laboratoire ; relever Debian, PHP, MariaDB, GLPI et agent ; vérifier l’accès depuis le client ; dater le test. Compléter aussi la provenance du dépôt PHP si elle peut être retrouvée. | environnement-debian.md et preuves/installation-serveur/ |
| 2 | Article Google Drive et diffusion des procédures | Ouvrir l’article complet ; capturer son contenu et ses cibles. Tester sa lecture avec un demandeur autorisé. Pour revendiquer un partage Drive effectué, conserver une preuve externe anonymisée et autorisée. | preuves/base-connaissances/ |
| 2 | Sauvegarde et restauration | Sauvegarder base MariaDB et fichiers/configuration GLPI nécessaires, hors du dépôt public. Restaurer dans un environnement isolé, ouvrir GLPI et vérifier tickets, parc et articles ; consigner commandes, dates et résultat réel. | Nouveau thème preuves/sauvegarde-restauration/ lorsque des preuves existent |
| Selon résultat | Ticket 10 encore en cours | Si le traitement est effectué, ajouter les résultats des tests et la solution, puis conserver le nouvel état ; sinon garder explicitement En cours. | preuves/tickets/ |
| Selon résultat | Ticket 11 résolu sans clôture démontrée | Vérifier son état ; conserver la clôture uniquement si elle existe ou si elle intervient selon la procédure retenue. | preuves/tickets/ |

## Règle d’ajout des nouvelles preuves

1. Effectuer ou vérifier l’action dans le laboratoire.
2. Conserver une image lisible ou un export sans secrets, par exemple `ticket-06-detail-AAAA-MM-JJ.png`.
3. Ajouter un lien dans le README du thème et dans le registre concerné.
4. Décrire le résultat obtenu, la date de vérification et les limites ; ne pas rétrodater une intervention.
5. Mettre à jour le backlog et enregistrer un commit décrivant les preuves ajoutées.

## Présentation défendable aujourd’hui

Le dossier permet de présenter une installation GLPI documentée, une remontée d’inventaire par agent et une simulation EcoTech comprenant utilisateurs, groupes, parc, tickets et procédures. Les incidents 4 et 8 constituent les dossiers de traitement les plus détaillés. Le ticket 10 illustre un suivi en cours.

Les captures ne certifient pas un déploiement en production ni l’exécution physique de toutes les interventions. Les demandes visibles seulement en liste, l’ensemble des droits, la composition des groupes et une restauration testée ne sont pas présentés comme validés. Le dossier est harmonisé pour la présentation, mais ces preuves complémentaires restent à recueillir avant de revendiquer les résultats correspondants.
