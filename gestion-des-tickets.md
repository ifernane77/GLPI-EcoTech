# Registre des tickets observés

La liste conservée montre huit tickets de la simulation EcoTech. Les numéros ci-dessous sont les identifiants GLPI, pas les numéros de l’ancienne liste prévisionnelle.

| ID | Sujet | Statut observé | Niveau de preuve |
|---:|---|---|---|
| 4 | Impossible d’imprimer depuis le poste administratif | Clos | Description, intervention, solution, dates et imprimante associée visibles |
| 5 | Lenteur importante sur le PC administratif | Clos | Ligne dans la liste ; détail non conservé |
| 6 | Demande d’accès au dossier Google Drive chantier | Clos | Ligne dans la liste ; exécution du partage non démontrée |
| 7 | Mot de passe oublié pour le compte utilisateur | Clos | Ligne dans la liste ; réinitialisation non démontrée |
| 8 | Coupure Internet au bureau EcoTech | Clos | Description, intervention, solution, dates et Livebox associée visibles |
| 9 | Création d’un compte GLPI pour un utilisateur terrain | Clos | Ligne dans la liste ; aucun technicien affiché sur cette ligne |
| 10 | Smartphone terrain impossible à connecter au Wi-Fi | En cours (Attribué) | Description, premières vérifications, support et téléphone associé visibles |
| 11 | Besoin d’une procédure simple pour déclarer un ticket | Résolu | Ligne dans la liste ; procédure lisible séparément ; clôture non démontrée |

## Incidents détaillés

- **4 — Impression** : tâche de vérification de l’imprimante, contrôle de connexion, redémarrage, réajout sur le poste et essai. La solution saisie indique un test réussi. Le ticket est clos et associé à `ECO-IMP-ADM-01`.
- **8 — Internet** : vérifications des voyants et de l’étendue de l’incident, redémarrage de la box et tests. La solution saisie indique une connexion rétablie. Le ticket est clos et associé à `ECO-NET-LIVEBOX-01`.
- **10 — Wi-Fi** : vérification du mot de passe, proximité de la box et comparaison avec un autre appareil. Aucune solution finale n’est visible. Équipement : `ECO-TEL-TER-01`.

Ces traces prouvent le traitement enregistré dans une simulation. Un statut clos ne démontre pas à lui seul une action sur un service externe ni une intervention sur du matériel physique.

## Catégories effectivement visibles

`Matériel / Imprimante`, `Matériel / Ordinateur`, `Réseau / Internet`, `Documents / Google Drive`, `Accès / Compte utilisateur`, `Application / GLPI`. La liste complète des catégories et les types Incident/Demande des tickets 5, 6, 7, 9 et 11 restent à capturer.

## Ancien prévisionnel

Les scénarios application EcoTech inaccessible, téléphone abîmé, devis introuvable et sauvegarde régulière ne sont pas démontrés dans les tickets disponibles. Ils ne sont pas nécessaires pour décrire les huit tickets ci-dessus et ne sont pas présentés comme réalisés.

[Captures et compléments](preuves/tickets/README.md).
