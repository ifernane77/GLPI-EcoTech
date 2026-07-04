# Tickets GLPI prévisionnels — EcoTech

## Objectif du document

Ce document prépare 8 tickets réalistes qui seront ensuite saisis dans GLPI.

Ces tickets sont liés au contexte d’EcoTech et permettent de préparer l’épreuve E5 du BTS SIO.

## Liste des tickets prévus

| N° | Type | Titre | Priorité | Équipement ou service concerné |
|---:|---|---|---|---|
| 1 | Incident | PC administratif lent au démarrage | Moyenne | PC-ADM-01 |
| 2 | Incident | Imprimante / scanner indisponible | Haute | IMP-SCAN-01 |
| 3 | Demande | Accès à un dossier Google Drive | Moyenne | Google Drive |
| 4 | Incident | Problème d’accès à l’application EcoTech | Haute | Application EcoTech |
| 5 | Incident | Téléphone professionnel abîmé | Moyenne | TEL-PRO-02 |
| 6 | Demande | Devis introuvable pour un chantier | Moyenne | Documents chantier |
| 7 | Incident | Connexion Internet instable via Livebox | Haute | BOX-01 |
| 8 | Demande | Mise en place d’une sauvegarde régulière | Haute | Documents entreprise |

---

# Ticket 1 — PC administratif lent au démarrage

## Type

Incident

## Demandeur

Employé administratif

## Catégorie

Poste de travail

## Équipement concerné

PC-ADM-01

## Priorité

Moyenne

## Description

L’employé administratif signale que le PC fixe utilisé pour la gestion des documents est très lent au démarrage. L’ouverture des fichiers et du navigateur prend plusieurs minutes.

## Impact

La lenteur ralentit le traitement des documents administratifs, des devis et des factures.

## Première analyse

Causes possibles :

- trop de programmes au démarrage ;
- manque d’espace disque ;
- mises à jour en attente ;
- problème matériel ;
- antivirus ou logiciel de sécurité à vérifier.

## Action prévue

- vérifier l’espace disque ;
- vérifier les programmes au démarrage ;
- vérifier les mises à jour ;
- redémarrer le poste ;
- proposer un nettoyage simple du système.

## Preuve à produire plus tard dans GLPI

- capture du ticket créé ;
- capture du statut du ticket ;
- capture de la résolution.

---

# Ticket 2 — Imprimante / scanner indisponible

## Type

Incident

## Demandeur

Employé administratif

## Catégorie

Impression

## Équipement concerné

IMP-SCAN-01

## Priorité

Haute

## Description

L’imprimante / scanner ne répond plus depuis un poste administratif. L’utilisateur ne peut plus imprimer ni scanner certains documents de chantier.

## Impact

Le traitement des documents administratifs est bloqué.

## Première analyse

Causes possibles :

- imprimante hors ligne ;
- câble ou connexion réseau ;
- file d’attente bloquée ;
- pilote d’impression ;
- redémarrage nécessaire.

## Action prévue

- vérifier l’alimentation ;
- vérifier la connexion ;
- vider la file d’attente ;
- relancer l’imprimante ;
- tester une impression depuis un autre poste.

## Preuve à produire plus tard dans GLPI

- capture du ticket ;
- capture de l’équipement associé ;
- capture de clôture du ticket.

---

# Ticket 3 — Demande d’accès à un dossier Google Drive

## Type

Demande

## Demandeur

Gérant

## Catégorie

Accès / droits

## Service concerné

Google Drive

## Priorité

Moyenne

## Description

Un employé doit accéder à un dossier Google Drive contenant des documents liés à un chantier en cours.

## Impact

Sans accès au dossier, l’employé ne peut pas consulter certains documents utiles au suivi du chantier.

## Première analyse

La demande concerne les droits d’accès à un dossier partagé.

## Action prévue

- identifier le dossier concerné ;
- vérifier la personne autorisée à donner l’accès ;
- attribuer l’accès nécessaire ;
- éviter de donner plus de droits que nécessaire.

## Preuve à produire plus tard dans GLPI

- capture du ticket de demande ;
- capture de la catégorie accès ;
- capture de la résolution.

---

# Ticket 4 — Problème d’accès à l’application EcoTech

## Type

Incident

## Demandeur

Gérant

## Catégorie

Application

## Service concerné

EcoTech Suivi Chantier

## Priorité

Haute

## Description

Un utilisateur ne parvient pas à se connecter à l’application EcoTech Suivi Chantier. Le message indique que les identifiants sont incorrects.

## Impact

L’utilisateur ne peut pas consulter les informations de chantier.

## Première analyse

Causes possibles :

- mot de passe oublié ;
- compte désactivé ;
- erreur de saisie ;
- rôle mal configuré ;
- problème de session.

## Action prévue

- vérifier l’existence du compte ;
- vérifier le rôle attribué ;
- réinitialiser le mot de passe si nécessaire ;
- tester la connexion ;
- documenter l’intervention.

## Preuve à produire plus tard dans GLPI

- ticket incident ;
- capture du compte utilisateur ;
- capture de résolution.

---

# Ticket 5 — Téléphone professionnel abîmé

## Type

Incident

## Demandeur

Employé terrain

## Catégorie

Matériel mobile

## Équipement concerné

TEL-PRO-02

## Priorité

Moyenne

## Description

Un téléphone professionnel utilisé sur chantier est abîmé. L’écran est fissuré et l’utilisateur signale des difficultés pour prendre des photos.

## Impact

La prise de photos de chantier devient difficile, ce qui peut limiter le suivi visuel de l’avancement.

## Première analyse

L’équipement doit être vérifié pour savoir s’il reste utilisable ou s’il doit être remplacé.

## Action prévue

- vérifier l’état de l’écran ;
- vérifier l’appareil photo ;
- sauvegarder les photos importantes ;
- proposer réparation ou remplacement ;
- mettre à jour l’état de l’équipement dans GLPI.

## Preuve à produire plus tard dans GLPI

- ticket incident ;
- fiche de l’équipement ;
- statut mis à jour.

---

# Ticket 6 — Devis introuvable pour un chantier

## Type

Demande

## Demandeur

Gérant

## Catégorie

Documents

## Service concerné

Documents chantier

## Priorité

Moyenne

## Description

Un devis lié à un chantier n’est pas retrouvé rapidement. Il peut se trouver dans les mails, Google Drive ou sur un PC personnel.

## Impact

L’équipe perd du temps pour retrouver un document important.

## Première analyse

La demande montre le problème de dispersion des documents.

## Action prévue

- rechercher le devis dans les supports connus ;
- vérifier les mails ;
- vérifier le Drive ;
- vérifier les dossiers locaux ;
- documenter l’emplacement retrouvé ;
- recommander une centralisation dans l’application EcoTech.

## Preuve à produire plus tard dans GLPI

- ticket de demande ;
- résolution indiquant où le document a été retrouvé ;
- lien avec le besoin de centralisation EcoTech.

---

# Ticket 7 — Connexion Internet instable via Livebox

## Type

Incident

## Demandeur

Gérant

## Catégorie

Réseau

## Équipement concerné

BOX-01

## Priorité

Haute

## Description

La connexion Internet de l’entreprise est instable. Les utilisateurs rencontrent des coupures lors de l’accès aux mails, à Google Drive et aux outils en ligne.

## Impact

Le travail administratif et les échanges de documents sont perturbés.

## Première analyse

Causes possibles :

- problème Livebox ;
- problème fournisseur ;
- Wi-Fi instable ;
- redémarrage nécessaire ;
- surcharge ou mauvaise couverture.

## Action prévue

- redémarrer la Livebox ;
- vérifier les voyants ;
- tester la connexion depuis plusieurs appareils ;
- vérifier si le problème vient du Wi-Fi ou de l’accès Internet ;
- contacter le fournisseur si nécessaire.

## Preuve à produire plus tard dans GLPI

- ticket incident réseau ;
- équipement BOX-01 associé ;
- suivi de résolution.

---

# Ticket 8 — Mise en place d’une sauvegarde régulière

## Type

Demande

## Demandeur

Gérant

## Catégorie

Sauvegarde

## Service concerné

Documents entreprise

## Priorité

Haute

## Description

L’entreprise souhaite mettre en place une sauvegarde plus régulière de ses documents importants, notamment les devis, factures, photos et documents de chantier.

## Impact

Une absence de sauvegarde claire peut entraîner une perte de données en cas de panne, suppression accidentelle ou problème d’accès.

## Première analyse

L’entreprise utilise plusieurs supports : Google Drive, PC personnels, mails et WhatsApp. Une stratégie simple de sauvegarde doit être proposée.

## Action prévue

- identifier les documents critiques ;
- définir un emplacement de stockage principal ;
- proposer une sauvegarde régulière ;
- documenter la procédure ;
- sensibiliser l’équipe.

## Preuve à produire plus tard dans GLPI

- ticket de demande ;
- procédure de sauvegarde ;
- base de connaissances associée.

---

# Synthèse E5

Ces tickets permettront de travailler les compétences E5 suivantes :

- répondre aux incidents ;
- traiter les demandes d’assistance ;
- gérer le patrimoine informatique ;
- mettre à disposition un service informatique ;
- documenter les interventions.

## Statut actuel

Ces tickets sont préparés au format documentaire.

Ils seront plus tard saisis dans GLPI pour produire des captures d’écran exploitables dans le portfolio.